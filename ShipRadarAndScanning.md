# 2. Ship Radar & Scanning for Resources

## 2.0 Why This Guide Matters (For Newcomers)

If you've ever struggled to find rocks, salvage, or other resources while mining or exploring in Star Citizen, you're not alone! Many players miss out on valuable finds simply because they don't fully understand how ship radar and scanning work. This guide is here to help you change that.

**What You'll Learn:**
- **Choosing the Right Ship:** Some ships, like the Reclaimer, can only detect a small fraction of resources compared to others like the Dragonfly. Using the right ship makes a huge difference!
- **Understanding Radar Specs:** Even similar-looking ships can have very different radar sensitivity. For example, the MSR can scan 10% more space than a MOLE, just because of its radar.
- **Space vs. Surface Scanning:** The area or volume you can scan changes dramatically depending on whether you're in space or on a planet. Knowing the difference helps you plan your search and avoid frustration.
- **No More Guesswork:** With the formulas and tables in this guide, you'll know exactly what your ship can (and can't) do. This means less time wandering and more time finding valuable resources.
- **Confidence and Efficiency:** Understanding these basics will make you a more effective miner, scout, or salvager—and make your time in the 'verse much more rewarding!

**Bottom line:** If you've ever felt unlucky or frustrated while searching for resources, the real problem might be your ship or your scanning technique—not your luck. Read on to learn how to make the most of your radar and never miss a find again!

## 2.1 What Is Ship Radar?

Ship radar in Star Citizen is your main tool for detecting mineable resources, salvage panels, derelict ships, and more. Unlike other signals (like EM, CS, or IR), resource detection uses a special formula and is especially important for mining and salvage crews.

## 2.2 How Detection Works (The Formula)

To know if your ship can detect a resource, use this formula:

> **DetectedSignature = (EmittedSignature - (Ambience × (1 - RadarPierce))) × RadarSensitivity**

But in space, ambience is zero, so it simplifies to:

> **DetectedSignature = EmittedSignature × RadarSensitivity**

This means that in space, only the emitted signature of the target and your radar's sensitivity matter for detection—radar pierce and ambience have no effect in a true vacuum. This has been confirmed through experimentation in the [Aaron-Halo asteroid belt](https://cstone.space/resources/knowledge-base/65-aaron-halo-detailed-shape-and-density-survey), where detection results matched the simplified formula and showed no influence from radar pierce or ambience.

If **DetectedSignature ≥ DistanceToTarget**, you will see the target on radar or ping.

### 2.2.1 Example: Ship Radar Sensitivity

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

### 2.2.2 Example: Surface Scanning

When scanning on a planet or moon, detection is limited to a 2D area (a circle) instead of a 3D volume. The scanned area is:

> **Area (km²) = π × (DetectionRange/1000)²**

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

- **EmittedSignature:** The signal strength emitted by the target (e.g., asteroid, salvage panel). Based on surveys in the [Aaron-Halo asteroid belt](https://cstone.space/resources/knowledge-base/65-aaron-halo-detailed-shape-and-density-survey), a value of 20,000 meters is a good working estimate for asteroids and salvage panels.
- **Ambience:** The environmental background noise. In space, this is usually 0.
- **RadarPierce:** How well your radar can penetrate interference. If Ambience is 0, this has no effect.
- **RadarSensitivity:** The sensitivity of your ship's radar, usually a percentage (e.g., 85% for MSR, 100% for Dragonfly).

**In practice:**
- If Ambience is 0 (as in space), the formula simplifies to:
  > **DetectedSignature = EmittedSignature × RadarSensitivity**
- If your DetectedSignature is greater than or equal to the distance to the target, you will see it on your radar or ping.

**Source:** [CIG Dev Formula](https://robertsspaceindustries.com/spectrum/community/SC/forum/50259/thread/what-do-the-numbers-on-right-of-hud-ir-cs-em-value/4685582)

## 2.3 How Much Can You Scan? (Effective Scanning Volume)

The farther your radar can detect, the more space you can scan. The formula is:

> **Volume (km³) = 4/3 × π × (DetectedSignature / 1000)³**

Even a small increase in detection range means a much larger increase in the volume you can scan!

**Example:**
- MSR (RadarSensitivity = 85%) detects at ~15.9 km → ~16,743 km³ scanned
- Dragonfly (RadarSensitivity = 100%) detects at ~19 km → ~28,600 km³ scanned
- The MSR scans about 59% of the volume that the Dragonfly can, matching theory.

## 2.4 How to Use Your Radar (Practical Steps)

1. **Know Your Ship's Specs:** Learn your ship's RS Signature Sensitivity and calculate its detection range and scanned volume.
2. **Plan Your Route:** When exploring or mining, plan your route to maximize radar coverage. Consider your ship's radar limitations.
3. **Adjust Your Speed:** Slower speeds allow for more accurate scanning and less missed resources. Balance speed and detection.
4. **Use Ping Wisely:** Use the ping function to quickly check for resources nearby. Remember the difference between space and surface pinging.
5. **Analyze Readings:** Learn to quickly interpret radar or ping readings to find the location and quantity of resources.
6. **Practice Makes Perfect:** The more you use and understand your ship's radar, the better you'll get at finding resources.

## 2.5 Key Takeaways
- **Radar Sensitivity is Critical:** Higher sensitivity means more resources detected at greater distances.
- **Ambience is Usually Negligible in Space:** RadarPierce rarely affects detection in vacuum.
- **Detection is Binary:** If DetectedSignature ≥ DistanceToTarget, you see the resource; otherwise, you don't.
- **Volume Scales Fast:** Small improvements in detection range yield much larger scanning volumes.

## 2.6 RS Signature Values by Resource Type

Each minable resource type in Star Citizen has its own Radar Signature (RS) value, which determines how detectable it is by your ship's radar. For example, a Granite Deposit has an RS signature of 1920, while a Hercules C2 Derelict ship has a signature of 2400. The RS signature you see on your ship's HUD may be a multiple of the base value, depending on how many of that resource are clustered together—e.g., 1920 for a single granite deposit, 3840 for two, 5760 for three, and so on.

For a comprehensive and up-to-date list of RS signature values for all minable resource types, see the [Regolith Rocks Rock Class Survey](https://regolith.rocks/survey/rock_class). This resource provides detailed tables and explanations for each rock and deposit type, helping you identify what you're scanning based on the signature value displayed.

### Common RS Signature Values for Minable Resource Types

Below are example RS signature values for common minable rocks and surface deposits. The value you see on your ship's HUD is the sum of all signatures in a cluster—e.g., 1920 for one Granite Deposit, 3840 for two, etc.

| Resource Type         | RS Signature (Single) |
|----------------------|-----------------------|
| Granite Deposit      | 1920                  |
| Igneous Deposit      | 1950                  |
| Quartzite Deposit    | 1820                  |
| Shale Deposit        | 1730                  |
| Atacamite Deposit    | 1800                  |
| Felsic Deposit       | 1770                  |
| Gneiss Deposit       | 1840                  |
| Obsidian Deposit     | 1790                  |
| Hercules C2 Derelict | 2400                  |

#### Example: Signature Multiples

If you scan a cluster of 3 Granite Deposits, the HUD will show:

| Number of Granite Deposits | Total RS Signature |
|---------------------------|--------------------|
| 1                         | 1920               |
| 2                         | 3840               |
| 3                         | 5760               |
| 4                         | 7680               |

This pattern applies to all minable resource types: simply multiply the base RS signature by the number of rocks or deposits in the cluster.

For a full and up-to-date list, see the [Regolith Rocks Rock Class Survey](https://regolith.rocks/survey/rock_class).

---

## 2.7 References & Further Reading
- [CIG Dev Formula Discussion](https://robertsspaceindustries.com/spectrum/community/SC/forum/50259/thread/what-do-the-numbers-on-right-of-hud-ir-cs-em-value/4685582) — Official developer discussion explaining the meaning and mechanics behind HUD IR/CS/EM values and the detection formula in Star Citizen.
- [SC Ships Performances Viewer (RS Sensitivity)](https://www.spviewer.eu/performance?ship=drak_vulture) — Community-maintained tool for comparing ship radar sensitivity, detection ranges, and other performance metrics for all ships in Star Citizen.
- [Aaron Halo - Detailed Shape and Density Survey (CaptSheppard, Cornerstone)](https://cstone.space/resources/knowledge-base/65-aaron-halo-detailed-shape-and-density-survey) — A comprehensive, scientific survey of the Aaron-Halo asteroid belt by CaptSheppard (Cornerstone). This article details the methods, data, and findings on the belt's structure, density, and consistency across servers, and stands as a gold standard for community-driven research. CaptSheppard's marvellous work not only advanced our understanding of the Aaron-Halo, but also inspired me to join Cornerstone and later create this documentation.
- [Regolith Rocks Rock Class Survey](https://regolith.rocks/survey/rock_class) — A detailed, community-driven database of RS signature values for all rock and deposit types in Star Citizen. This resource is invaluable for identifying scanned objects and understanding the numbers shown on your ship's HUD.

---

*This section is a work in progress. If you have suggestions or want to see a specific topic covered, let us know!*
