# 2. Ship Radar & Scanning for Resources

## 2.0 Newcomer Motivation: Why This Page Matters

If you've ever struggled to find rocks, salvage, or other resources while mining or exploring in Star Citizen, you're not alone! Many players miss out on valuable finds simply because they don't understand how ship radar and scanning really work. This page is here to help you turn that around.

**Why should you read this page?**
- **Ship choice matters:** In space, a ship like the Reclaimer can only detect about 13% of the maximum possible resource volume compared to a Dragonfly. If you're using the wrong ship, you might be missing out on most of the rocks!
- **Radar specs are critical:** Even ships that look similar can have very different radar sensitivity. For example, the MSR can scan 10% more space than a MOLE, just because of its radar. Even though this doesn't make sense at all.
- **Surface vs. space scanning:** The area or volume you can scan changes dramatically depending on whether you're in space or on a planet. Knowing the difference helps you plan your search and avoid frustration.
- **No more guesswork:** With the formulas and tables on this page, you'll know exactly what your ship can (and can't) do. This means less time wandering and more time finding valuable resources.
- **Confidence and efficiency:** Understanding these basics will make you a more effective miner, scout, or salvager—and make your time in the 'verse much more rewarding!

**Bottom line:** If you've ever felt unlucky or frustrated while searching for resources, the real problem might be your ship or your scanning technique—not your luck. Read on to learn how to make the most of your radar and never miss a find again!

## 2.1 Introduction to Ship Radar
Ship radar in Star Citizen is the primary tool for detecting mineable resources, salvage panels, derelict ships, and more. Unlike EM, CS, or IR signatures, resource detection relies on a different formula and is especially important for mining and salvage crews.

## 2.2 The Detection Formula Explained

The formula used to determine whether a resource is detected by your ship's radar is:

> **DetectedSignature = (EmittedSignature - (Ambience × (1 - RadarPierce))) × RadarSensitivity**

Because the ambience in vacuum is zero, the formula simplifies to:

> **DetectedSignature = EmittedSignature × RadarSensitivity**

This means that in space, only the emitted signature of the target and your radar's sensitivity matter for detection—radar pierce and ambience have no effect in a true vacuum.

If **DetectedSignature ≥ DistanceToTarget**, you will see the target on radar or ping.

### 2.2.1 Example RS Signature Sensitivity Values by Ship

> **Note:** The scanned volume calculations below apply to space, where resources can be detected within a sphere around the ship. This represents the maximum 3D volume in which a resource can be detected, assuming no obstructions.

| Ship Name         | RS Signature Sensitivity (%) | Detection Range (m) | Scanned Volume (km³) | % of Max Volume |
|-------------------|-----------------------------|---------------------|----------------------|-----------------|
| Dragonfly         | 100%                        | 20,000              | 33,510               | 100%            |
| Mantis            | 90%                         | 18,000              | 24,429               | 73%             |
| MSR               | 85%                         | 17,000              | 20,579               | 61%             |
| MOLE              | 80%                         | 16,000              | 17,157               | 51%             |
| Vulture           | 80%                         | 16,000              | 17,157               | 51%             |
| Prospector        | 80%                         | 16,000              | 17,157               | 51%             |
| Carrack           | 75%                         | 15,000              | 14,137               | 42%             |
| Reclaimer         | 50%                         | 10,000              | 4,189                | 13%             |

> **Note:** Detection range is calculated as EmittedSignature × RS Sensitivity (e.g., 20,000 × 0.85 = 17,000 m for MSR). Scanned volume is calculated as 4/3 × π × (DetectionRange/1000)³ and rounded to the nearest whole number. For the latest and full list, visit [SC Ships Performances Viewer](https://www.spviewer.eu/performance).

### 2.2.2 Example RS Signature Sensitivity Values by Ship (Surface Scanning)

When scanning for resources on a planetary or moon surface, detection is limited to a 2D area (a circle) rather than a 3D volume. The scanned area is calculated as:

> **Area (km²) = π × (DetectionRange/1000)²**

| Ship Name   | RS Signature Sensitivity (%) | Detection Range (m) | Scanned Area (km²) | % of Max Area |
|-------------|-----------------------------|---------------------|--------------------|---------------|
| Dragonfly   | 100%                        | 20,000              | 1,257              | 100%          |
| Mantis      | 90%                         | 18,000              | 1,018              | 81%           |
| MSR         | 85%                         | 17,000              | 908                | 72%           |
| MOLE        | 80%                         | 16,000              | 804                | 64%           |
| Vulture     | 80%                         | 16,000              | 804                | 64%           |
| Prospector  | 80%                         | 16,000              | 804                | 64%           |
| Carrack     | 75%                         | 15,000              | 707                | 56%           |
| Reclaimer   | 50%                         | 10,000              | 314                | 25%           |

> **Note:** Scanned area is calculated as π × (DetectionRange/1000)² and rounded to the nearest whole number. This represents the maximum flat area on a surface where a resource can be detected. Percentages are relative to the maximum area (Dragonfly).

- **EmittedSignature:** The actual signal strength emitted by the target (e.g., asteroid, salvage panel). Based on surveys I conducted on the Aaron-Halo asteroid belt, a value of 20,000 meters is an accurate working estimate for asteroids and salvage panels.
- **Ambience:** The environmental background noise. In space (vacuum), this is typically 0, so it can often be ignored.
- **RadarPierce:** How well your radar can penetrate environmental interference. If Ambience is 0, this has no effect.
- **RadarSensitivity:** The sensitivity of your ship's radar, usually expressed as a percentage (e.g., 85% for MSR, 100% for Dragonfly). Higher sensitivity means better detection range.

**In practice:**
- If Ambience is 0 (as in space), the formula simplifies to:
  > **DetectedSignature = EmittedSignature × RadarSensitivity**
- If your DetectedSignature is greater than or equal to the distance to the target, you will see it on your radar or ping.

**Source:** [CIG Dev Formula](https://robertsspaceindustries.com/spectrum/community/SC/forum/50259/thread/what-do-the-numbers-on-right-of-hud-ir-cs-em-value/4685582)

## 2.3 Effective Scanning Volume

The effective volume of space you can scan is determined by how far your radar can detect a signature. The formula for the scanned volume is:

> **Volume (km³) = 4/3 × π × (DetectedSignature / 1000)³**

This means that even a small increase in detection range results in a much larger increase in the volume of space you can scan.

**Example:**
- MSR (RadarSensitivity = 85%) detects at ~15.9 km → ~16,743 km³ scanned
- Dragonfly (RadarSensitivity = 100%) detects at ~19 km → ~28,600 km³ scanned
- The MSR scans about 59% of the volume that the Dragonfly can, matching theoretical predictions.

## 2.4 Practical Scanning Procedure

To effectively use your ship's radar for finding resources, follow these steps:

1. **Know Your Ship's Specs:** Understand your ship's RS Signature Sensitivity and calculate its detection range and scanned volume.
2. **Plan Your Route:** When exploring or mining, plan your route to maximize the area covered by your radar. Consider the limitations of your ship's radar compared to others.
3. **Adjust Your Speed:** Slower speeds allow for more accurate scanning and less missed resources. Consider the trade-off between speed and detection.
4. **Use Ping Wisely:** Utilize the ping function to get a quick overview of the resources in your vicinity. Remember the difference between space and surface pinging.
5. **Analyze Readings:** Learn to quickly analyze the radar or ping readings to determine the location and quantity of resources.
6. **Practice Makes Perfect:** The more you use and understand your ship's radar, the more effective you'll become at locating resources.

## 2.5 Key Takeaways
- **RS Signature Sensitivity of your radar is critical:** Higher sensitivity means more resources detected at greater distances.
- **Ambience is usually negligible in space:** So RadarPierce rarely affects detection in vacuum.
- **Detection is binary:** If DetectedSignature ≥ DistanceToTarget, you see the resource; otherwise, you don't.
- **Volume scales fast:** Small improvements in detection range yield much larger scanning volumes.

## 2.6 References & Further Reading
- [CIG Dev Formula Discussion](https://robertsspaceindustries.com/spectrum/community/SC/forum/50259/thread/what-do-the-numbers-on-right-of-hud-ir-cs-em-value/4685582)
- [SC Ships Performances Viewer (RS Sensitivity)](https://www.spviewer.eu/performance?ship=drak_vulture)

---

*This section is a work in progress. If you have suggestions or want to see a specific topic covered, let us know!*
