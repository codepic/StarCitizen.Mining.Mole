# 3. Ship Radar & Scanning for Resources

> **Summary:** This guide explores the mechanics of ship radar and scanning in Star Citizen, focusing on resource detection techniques and radar formulas. It provides practical insights for players aiming to improve their mining and exploration efficiency.

> **Geek-Out Warning:** This guide dives into the nitty-gritty of radar formulas and scanning techniques. But don't worry—it's all grounded in common sense, so even if math isn't your thing, you'll find it easy to follow and super rewarding!

> **Quick Note:** Even if mining isn't your thing and you're more into the pew-pew action, you might actually learn something useful here. After all, understanding radar mechanics can give you an edge in any scenario!

## 3.1 Mandatory Graph

> **Summary:** A visual representation of radar and scanning concepts, illustrating their interconnections and key topics covered in the guide.

```mermaid
graph TD
    A[Ship Radar & Scanning] --> B[Space Scanning]
    A --> C[Surface Scanning]
    B --> D[Detection Formula]
    C --> E[Altitude Impact]
    D --> F[Detected Signature]
    E --> G[Scanned Area]
    F --> H[Emitted Signature]
    F --> I[Radar Sensitivity]
    G --> J[Circle Radius]
    G --> K[Ambience]
```

## 3.2 Why This Guide Matters

If you've ever struggled to find rocks, salvage, or other resources while mining or exploring in Star Citizen, you're not alone! Many players miss out on valuable finds simply because they don't fully understand how ship radar and scanning work. This guide is here to help you change that.

Before we dive into the technical details, let's set the stage with what you'll gain from this guide:

**What You'll Learn:**
- **Choosing the Right Ship:** Some ships, like the Reclaimer, can only detect a small fraction of resources compared to others like the Dragonfly. Using the right ship makes a huge difference!
- **Understanding Radar Specs:** Even similar-looking ships can have very different radar sensitivity. For example, the MSR can scan 10% more space than a MOLE, just because of its radar.
- **Space vs. Surface Scanning:** The area or volume you can scan changes dramatically depending on whether you're in space or on a planet. Knowing the difference helps you plan your search and avoid frustration.
- **No More Guesswork:** With the formulas and tables in this guide, you'll know exactly what your ship can (and can't) do. This means less time wandering and more time finding valuable resources.
- **Confidence and Efficiency:** Understanding these basics will make you a more effective miner, scout, or salvager—and make your time in the 'verse much more rewarding!

**Bottom line:** Whether you're a seasoned veteran or just starting your journey, this guide will help you make the most of your radar and scanning techniques, ensuring you never miss a valuable find again!

## 3.3 What Is Ship Radar?

Ship radar uses formulas to detect resources and ship signatures. Resource detection values are static, while ship signatures vary based on modules and energy distribution. Understanding these basics is key to effective scanning.

### 3.3.1 Similarities and Differences Between EM, IR, RS Scanning

- **EmittedSignature:** The signal strength emitted by the target. For resource scanning, RS signature is used, while other signatures like EM and IR are specific to ships and vary dynamically based on ship modules and energy distribution.
- **Ambience:** The environmental background noise. Ambience affects surface scanning but is zero in space, simplifying detection formulas.
- **RadarPierce:** Determines the focus or width of the scanning cone. It has no impact in space due to zero ambience. More research is needed to figure out the actual values of Ambience on planetary body surfaces. If figuring out such details is your suit, consider applying for the Cornerstone Star Citizen organization and its `analysis` pillar. Learn more and join at [Cornerstone Organization](https://robertsspaceindustries.com/en/orgs/CSTONE).
- **RadarSensitivity:** Represents the percentage of the maximum detection range. In this document, we concentrate exclusively on RS Signature Sensitivity, which is specific to resource scanning and determines how effectively resources can be detected.

**In practice:**
- In space, the formula simplifies to:
  > **DetectedSignature = EmittedSignature × RadarSensitivity**
- If DetectedSignature ≥ DistanceToTarget, the target appears on radar or ping.

**Source:** [CIG Dev Formula](https://robertsspaceindustries.com/spectrum/community/SC/forum/50259/thread/what-do-the-numbers-on-right-of-hud-ir-cs-em-value/4685582)

---

## 3.4 How Detection Works (The Formula)

Ready to geek out? Here's where we dive into the mechanics of detection. Don't worry if formulas aren't your thing—we'll break them down step by step and show you how they apply in real scenarios.

To know if your ship can detect a resource, use this formula:

> **DetectedSignature = (EmittedSignature - (Ambience × (1 - RadarPierce))) × RadarSensitivity**

But in space, ambience is zero, so it simplifies to:

> **DetectedSignature = EmittedSignature × RadarSensitivity**

This means that in space, only the emitted signature of the target and your radar's sensitivity matter for detection—radar pierce and ambience have no effect in a true vacuum. This has been confirmed through experimentation in the [Aaron-Halo asteroid belt](https://cstone.space/resources/knowledge-base/65-aaron-halo-detailed-shape-and-density-survey), where detection results matched the simplified formula and showed no influence from radar pierce or ambience.

If **DetectedSignature ≥ DistanceToTarget**, you will see the target on radar or ping.

### 3.4.1 Example: Ship Radar Sensitivity

> **Note:** The following table shows how much space different ships can scan in space. The higher the sensitivity, the more resources you can find!

| Ship Name         | RS Sensitivity (%) | Detection Range (m) | Scanned Volume (km³) | % of Max Volume |
|-------------------|-------------------|---------------------|----------------------|-----------------|
| Dragonfly         | 100%              | 20,000              | 33,510               | 100%            |
| Mantis            | 90%               | 18,000              | 24,429               | 73%             |
| MSR               | 85%               | 17,000              | 20,579               | 61%             |
| MOLE              | 80%               | 16,000              | 17,157               | 51%             |
| Vulture           | 80%               | 16,000              | 17,157               | 51%             |
| Prospector        | 80%               | 16,000              | 17,157               | 51%             |
| Carrack           | 75%               | 15,000              | 14,137               | 42%             |
| Reclaimer         | 50%               | 10,000              | 4,189                | 13%             |

> **Note:** Detection range is calculated as EmittedSignature × RS Sensitivity. Scanned volume is calculated as 4/3 × π × (DetectionRange/1000)³.

> **Tip:** Clusters of rocks will show a higher RS value on your HUD. If you notice a sudden jump in RS signature while scanning, it often means you've found a rich area with multiple deposits close together. Focus your search in these spots for the best mining opportunities.
> 
> **Tip:** Adjust your ship's speed while scanning—flying slower increases your chances of detecting smaller or more distant rocks, as it gives your radar more time to pick up faint signals.
>
> **Tip:** Use slow, overlapping scan passes when covering an area. This helps ensure you don't miss small deposits that might fall between scan sweeps, especially when searching for valuable or rare resources.

### 3.4.2 Example: Surface Scanning

When scanning on a planet or moon, detection is limited to a 2D area (a circle) instead of a 3D volume. The scanned area is:

> **Area (km²) = π × (DetectionRange/1000)²**

> **Assumption:** This example assumes an altitude of 0 meters.

| Ship Name   | RS Sensitivity (%) | Detection Range (m) | Scanned Area (km²) | % of Max Area |
|-------------|-------------------|---------------------|--------------------|---------------|
| Dragonfly   | 100%              | 20,000              | 1,257              | 100%          |
| Mantis      | 90%               | 18,000              | 1,018              | 81%           |
| MSR         | 85%               | 17,000              | 908                | 72%           |
| MOLE        | 80%               | 16,000              | 804                | 64%           |
| Vulture     | 80%               | 16,000              | 804                | 64%           |
| Prospector  | 80%               | 16,000              | 804                | 64%           |
| Carrack     | 75%               | 15,000              | 707                | 56%           |
| Reclaimer   | 50%               | 10,000              | 314                | 25%           |

> **Note:** Scanned area is calculated as π × (DetectionRange/1000)².

- **EmittedSignature:** The signal strength emitted by the target (e.g., asteroid, salvage panel). Based on individual surveys, a value of 20,000 meters is a good working estimate for asteroids and salvage panels. This estimate is independent of the linked [Aaron-Halo asteroid belt survey](https://cstone.space/resources/knowledge-base/65-aaron-halo-detailed-shape-and-density-survey), which focuses on other aspects of the belt.
- **Ambience:** The environmental background noise. At the moment, the exact values for ambience on planet or moon surfaces are largely unknown. If figuring out such details is your suit, consider applying for the Cornerstone Star Citizen organization and its `analysis` pillar. Learn more and join at [Cornerstone Organization](https://robertsspaceindustries.com/en/orgs/CSTONE).
- **RadarPierce:** The angle of the radar scan, determining how focused or wide the scanning cone is. According to the formula provided by CIG developers, if Ambience = 0, RadarPierce is effectively canceled out and has no impact on DetectedSignature.
- **RadarSensitivity:** Effectively the percentage of the maximum 20 kilometers your radar can detect a signature in vacuum.

**In practice:**
- If Ambience is 0 (as in space), the formula simplifies to:
  > **DetectedSignature = EmittedSignature × RadarSensitivity**
- If your DetectedSignature is greater than or equal to the distance to the target, you will see it on your radar or ping.

**Source:** [CIG Dev Formula](https://robertsspaceindustries.com/spectrum/community/SC/forum/50259/thread/what-do-the-numbers-on-right-of-hud-ir-cs-em-value/4685582)

## 3.5 How Much Can You Scan? (Effective Scanning Volume)

The farther your radar can detect, the more space you can scan. The formula is:

> **Volume (km³) = 4/3 × π × (DetectedSignature / 1000)³**

Even a small increase in detection range means a much larger increase in the volume you can scan!

**Example:**
- Reclaimer (RadarSensitivity = 50%) detects at ~10 km → ~4,189 km³ scanned
- Dragonfly (RadarSensitivity = 100%) detects at ~20 km → ~33,510 km³ scanned
- The Reclaimer scans about 12.5% of the volume that the Dragonfly can, which explains why you can't find much panels with a Reclaimer.

## 3.6 How to Use Your Radar (Practical Steps)

1. **Know Your Ship's Specs:** Learn your ship's RS Signature Sensitivity and calculate its detection range and scanned volume.
2. **Plan Your Route:** When exploring or mining, plan your route to maximize radar coverage. Consider your ship's radar limitations.
3. **Adjust Your Speed:** Slower speeds allow for more accurate scanning and less missed resources. Balance speed and detection.
4. **Use Ping Wisely:** Use the ping function to quickly check for resources nearby. Remember the difference between space and surface pinging.
5. **Analyze Readings:** Learn to quickly interpret radar or ping readings to find the location and quantity of resources.
6. **Practice Makes Perfect:** The more you use and understand your ship's radar, the better you'll get at finding resources.

## 3.7 Surface Scanning vs. Altitude

### Understanding Surface Scanning

When scanning for resources on a planet or moon, the scanned area forms a circular intersection between the radar's spherical detection range and the surface. As altitude increases, the radius of this circle decreases, reducing the scanned area.

### Surface Scanning Area Table

Below is a table illustrating how the scanned surface area changes with altitude for a ship with a maximum scanning radius of 20,000 meters (100% RS Signature Sensitivity) and 17,000 meters (85% RS Signature Sensitivity):

| Altitude (h) in m | Circle Radius √(r² - h²) (m) (100%) | Scanned Area (km²) (100%) | Circle Radius √(r² - h²) (m) (85%) | Scanned Area (km²) (85%) |
|-------------------|------------------------------------|---------------------------|------------------------------------|--------------------------|
| 0                 | 20,000                            | 1,256.6                   | 17,000                            | 907.9                    |
| 2,000             | 19,798                            | 1,229.2                   | 16,798                            | 884.7                    |
| 4,000             | 19,595                            | 1,173.4                   | 16,595                            | 859.7                    |
| 6,000             | 19,390                            | 1,089.1                   | 16,390                            | 832.9                    |
| 8,000             | 19,183                            | 976.2                     | 16,183                            | 804.3                    |
| 10,000            | 18,974                            | 834.5                     | 15,974                            | 774.0                    |
| 12,000            | 18,788                            | 663.5                     | 15,788                            | 742.0                    |
| 14,000            | 18,520                            | 462.4                     | 15,520                            | 708.2                    |
| 16,000            | 18,330                            | 230.4                     | 15,330                            | 672.7                    |
| 18,000            | 8,717                             | 23.9                      | 7,717                             | 187.0                    |
| 20,000            | 0                                 | 0                         | 0                                 | 0                        |

> **Note:** The scanned area is calculated using the formula **π × (r² - h²)**, where `r` is the radar's maximum scanning radius and `h` is the altitude above the surface.

> **Important:** The table assumes RS Signature Sensitivity of 100% and 85%, which represent theoretical and practical values respectively.

> **Caution:** The calculations assume Ambience=0, which is never true on a planet's surface.

## 3.8 Key Takeaways
- **Radar Sensitivity is Critical:** Higher sensitivity means more resources detected at greater distances.
- **Ambience is Usually Negligible in Space:** RadarPierce rarely affects detection in vacuum.
- **Detection is Binary:** If DetectedSignature ≥ DistanceToTarget, you see the resource; otherwise, you don't.
- **Volume Scales Fast:** Small improvements in detection range yield much larger scanning volumes.

## 3.9 Simple Rules Summary

1. The scanned volume increases by the cube of the radius.
2. The scanned surface area at 0 altitude increases by the square of the radius.
3. The scanned surface area decreases by the square of the altitude.

## 3.10 RS Signature Values by Resource Type

Each minable resource type in Star Citizen has its own Radar Signature (RS) value, which determines how detectable it is by your ship's radar. For example, a Granite Deposit has an RS signature of 1920, while a Hercules C2 Derelict ship has a signature of 2400. The RS signature you see on your ship's HUD may be a multiple of the base value, depending on how many of that resource are clustered together—e.g., 1920 for a single granite deposit, 3840 for two, 5760 for three, and so on.

> **Note:** RS signature detection works exactly the same way as IR, EM, or CS detection. The only difference is that RS values for resources are static (always the same for a given resource type), while ship signatures (IR/EM/CS) are dynamic and can change depending on what modules are active, ship state, or player actions.

For a comprehensive and up-to-date list of RS signature values for all minable resource types, see the [Regolith Rocks Rock Class Survey](https://regolith.rocks/survey/rock_class). If you hover your mouse over the RS signature on the linked page, you'll see the multiple signature values for each resource type.

### Common RS Signature Values for Minable Resource Types

Below are example RS signature values for common minable rocks and surface deposits. The value you see on your ship's HUD is the sum of all signatures in a cluster—e.g., 1920 for one Granite Deposit, 3840 for two, etc.

| Resource Type         | RS Signature (2) | RS Signature (3) | RS Signature (5) | RS Signature (7) | RS Signature (11) |
|----------------------|------------------|------------------|------------------|------------------|-------------------|
| Granite Deposit      | 3840             | 5760             | 9600             | 13,440           | 21,120            |
| Igneous Deposit      | 3900             | 5850             | 9750             | 13,650           | 21,450            |
| Quartzite Deposit    | 3640             | 5460             | 9100             | 12,740           | 19,880            |
| Shale Deposit        | 3460             | 5190             | 8650             | 12,110           | 18,830            |
| Atacamite Deposit    | 3600             | 5400             | 9000             | 12,600           | 19,800            |
| Felsic Deposit       | 3540             | 5310             | 8850             | 12,390           | 19,470            |
| Gneiss Deposit       | 3680             | 5520             | 9200             | 12,880           | 20,240            |
| Obsidian Deposit     | 3580             | 5370             | 8950             | 12,530           | 19,690            |
| Hercules C2 Derelict | 4800             | 7200             | 12,000           | 16,800           | 26,400            |

#### Example: Signature Multiples

If you scan a cluster of 3 Granite Deposits, the HUD will show:

| Number of Granite Deposits | Total RS Signature |
|---------------------------|--------------------|
| 1                         | 1920               |
| 2                         | 3840               |
| 3                         | 5760               |
| 5                         | 9600               |
| 7                         | 13,440             |
| 11                        | 21,120             |

This pattern applies to all minable resource types: simply multiply the base RS signature by the number of rocks or deposits in the cluster.

For a full and up-to-date list, see the [Regolith Rocks Rock Class Survey](https://regolith.rocks/survey/rock_class). If you hover your mouse over the RS signature on the linked page, you'll see the multiple signature values for each resource type.

---

## 3.11 Ship Minables vs. ROC/FPS Minables

### Understanding the Difference

Ship minables and ROC/FPS minables differ significantly in their `EmittedSignature` values. ROC/FPS minables generally have lower `EmittedSignature` values, making them harder to detect at longer ranges. This distinction is crucial when surface scanning for resources.

### Practical Insight

If you discover a deposit while surface scanning at a range of less than 5 km, it is most likely one of the following ROC/FPS minables:

- Janalite
- Hadanite
- Feynmeline
- Aphorite
- Beradom
- Dolivine
- Glacosite
- Carinite
- Jaclium
- Saldynium

> **Note:** These minables are typically smaller and have lower `RS Signature` values compared to ship minables, which are detectable at much greater distances.

## 3.12 References & Further Reading

- [CIG Dev Formula Discussion](https://robertsspaceindustries.com/spectrum/community/SC/forum/50259/thread/what-do-the-numbers-on-right-of-hud-ir-cs-em-value/4685582) — Official developer discussion explaining the meaning and mechanics behind HUD IR/CS/EM values and the detection formula in Star Citizen.
- [SC Ships Performances Viewer (RS Sensitivity)](https://www.spviewer.eu/performance?ship=drak_vulture) — Community-maintained tool for comparing ship radar sensitivity, detection ranges, and other performance metrics for all ships in Star Citizen.
- [Aaron Halo - Detailed Shape and Density Survey (CaptSheppard, Cornerstone)](https://cstone.space/resources/knowledge-base/65-aaron-halo-detailed-shape-and-density-survey) — A comprehensive, scientific survey of the Aaron-Halo asteroid belt by CaptSheppard (Cornerstone). This article details the methods, data, and findings on the belt's structure, density, and consistency across servers, and stands as a gold standard for community-driven research. CaptSheppard's marvellous work not only advanced our understanding of the Aaron-Halo, but also inspired me to join Cornerstone and later create this documentation.
- [Regolith Rocks Rock Class Survey](https://regolith.rocks/survey/rock_class) — A detailed, community-driven database of RS signature values for all rock and deposit types in Star Citizen. This resource is invaluable for identifying scanned objects and understanding the numbers shown on your ship's HUD.

---
