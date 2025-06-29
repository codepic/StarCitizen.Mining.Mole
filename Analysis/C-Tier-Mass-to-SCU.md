[💬 Send feedback on this page](https://github.com/codepic/StarCitizen.Mining.Mole/issues/new?template=feedback.yml&title=Feedback+on+C-Tier-Effect.md&page=C-Tier-Effect.md)  

# The Impact of C-Tier ore Mass-to-SCU Ratio on Value per Mole

## About C-Tier Ore Modifiers

1. **Modifiers Affect Profitability**: [C-tier ores](https://regolith.rocks/survey/ores?ot=C) have properties that influence the behavior of rocks during mining. Since these ores will constitute the majority of the mass, their modifiers—such as Mass to SCU ratio, resistance, and instability—play a crucial role in determining the efficiency and profitability of mining operations.

2. **Cherry-Picking Favorable Modifiers**: By focusing on [C-tier ores](https://regolith.rocks/survey/ores?ot=C) with favorable modifiers, miners can ensure that the rocks they target are easier to break, safer to handle, and more efficient to extract. This strategic selection minimizes risks and maximizes yields.

3. **Abundance**: [C-tier ores](https://regolith.rocks/survey/ores?ot=C) are the most abundant, meaning most rocks will contain them. This abundance makes them a reliable indicator for identifying viable mining locations.

Even though these ores may ultimately be discarded, their impact on the overall mining process makes them a factor in choosing the right location.

| Material 🪨 | Clustering 🔗 | Explosion Strength 💥 | Instability ⚡ | Resistance 🛡️ | Green Zone Thinness 🟩 | Mass to SCU ⚖️ |
|:-----------|-------------:|---------------------:|-------------:|------------:|----------------------:|---------------:|
| Ice        |           69 |                ✅ -20 |         ✅ 0 |      ✅ -50% |                 +50% |      ✅ 34 |
| Silicon    |       ✅ 90 |                💥 +80  |           50 |      ✅ -20% |                 +50% |      ✅ 78 |
| Quartz     |       ✅ 90 |                 ✅ -20 |           50 |      ✅ -70% |                 +50% |      ✅ 89 |
| Aluminum   |           70 |                ✅ -36 |         ✅ 0 |      ✅ -40% |            ✅ -50% |      ✅ 90 |
| Corundum   |           70 |                  +36 |           50 |        +10% |            ✅ -50% |      ⚠️ 134 |
| Titanium   |       ✅ 90 |                 +20   |         ✅ 0 |        +10% |            ✅ -70% |      ⚠️ 150 |
| Tin        |           60 |                  +36 |        ✅ 0 |      ✅ -20% |                 +50% |      ⚠️ 193 |
| Iron       |           40 |                  +20 |           50 |      ✅ -40% |            ✅ -90% |      ❌ 263 |
| Copper     |           60 |                ✅ -20 |           50 |      ✅ -70% |            ✅ -90% |      ❌ 299 |
| Tungsten   |           40 |                💥 +80 |         ✅ 0 |      ✅ -40% |            ✅ -70% |      ❌ 644 |

### Explanation of Table Columns

- **Material 🪨**: The type of ore or resource being mined.
- **Clustering 🔗**: Indicates how well each type of mineral tends to stick together. Higher values mean cleaner splits, where the valuable minerals remain in their own breaks and the less valuable ones in theirs. **Higher values are more profitable**.
- **Explosion Strength 💥**: Represents the intensity of potentially explosive reactions during mining. **Lower values are safer**.
- **Instability ⚡**: Instability measures how erratic the energy input/output curve is during mining. High instability means the energy bar will fluctuate wildly, making it harder to keep the rock in the optimal green zone. **Lower values are easier**.
- **Resistance 🛡️**: Resistance is how much energy the rock absorbs before it starts to fracture. Higher resistance means you’ll need more powerful lasers or longer charge times to break it apart. **Lower values are easier**.
- **Green Zone Thinness 🟩**: This affects how narrow the “sweet spot” is for maintaining energy during fracturing. A thinner green zone demands more precision and control to avoid overcharging or undercharging. **Lower values are easier**.
- **Mass to SCU ⚖️**: The mass of the resource required to fill one Standard Cargo Unit (SCU). **Lower values are more profitable**.

## How Does C-Tier Ore Mass to SCU Affect Profitability?

The mass-to-SCU ratio determines how much ore is needed to fill a cargo unit. Lower ratios mean you fill your hold with less mass, increasing profit per SCU. This section explores how [C-Tier ore](https://regolith.rocks/survey/ores?ot=C)’s mass-to-SCU impacts mining returns.

*Source: Calculations made with [Regolith's Cluster Calculator](https://regolith.rocks/cluster)*

## With S-Tier Ore

This table compares rocks with the same total mass and high-value ore percentages, but different [C-Tier ores](https://regolith.rocks/survey/ores?ot=C). Each column represents a different [C-Tier ore](https://regolith.rocks/survey/ores?ot=C) (Iron, Titanium, Ice, etc.).

- **Total Mass**: The mass of the rock being analyzed (same for all).
- **Stileron % / Taranite % / C-Tier %**: The percentage of each ore type in the rock.
- **C-Tier Ore**: The specific [C-Tier ore](https://regolith.rocks/survey/ores?ot=C) in that column.
- **Value (aUEC)**: The total in-game value of the rock, in aUEC (Star Citizen’s currency).
- **Moles Filled**: How many Mole mining ship cargo holds the rock would fill.
- **Value per Mole (aUEC)**: The value of ore that fits in one Mole’s cargo hold.
- **% best**: How each ore’s value per Mole compares to the best (highest) value in the row (Iron, in this case, is 100%).

**Purpose:** This table shows how the choice of [C-Tier ore](https://regolith.rocks/survey/ores?ot=C) affects value and efficiency, even when all other factors are held constant.

| Property                | Iron      | Titanium  | Quartz    | Aluminum   | Ice        | Copper    | Tungsten   | Tin       | Corundum  | Silicon   |
|------------------------ |----------|-----------|----------|-----------|------------|-----------|------------|-----------|-----------|-----------|
| Total Mass              | 50,000   | 50,000    | 50,000   | 50,000   | 50,000     | 50,000    | 50,000     | 50,000    | 50,000    | 50,000    |
| Stileron %              | 10%      | 10%       | 10%      | 10%       | 10%        | 10%       | 10%        | 10%       | 10%       | 10%       |
| Taranite %              | 20%      | 20%       | 20%      | 20%       | 20%        | 20%       | 20%        | 20%       | 20%       | 20%       |
| C-Tier Ore              | Iron     | Titanium  | Quartz   | Aluminum  | Ice        | Copper    | Tungsten   | Tin       | Corundum  | Silicon   |
| C-Tier %                | 30%      | 30%       | 30%      | 30%       | 30%        | 30%       | 30%       | 30%       | 30%       | 30%       |
| Value (aUEC)            | 1,400,000| 1,700,000 | 1,900,000| 1,900,000 | 2,200,000  | 1,300,000 | 827,000    | 1,500,000 | 1,700,000 | 1,900,000 |
| Moles Filled            | 1.8      | 2.2       | 2.5      | 2.5       | 2.9        | 1.7       | 1.1        | 2.0       | 2.3       | 2.6       |
| Value per Mole (aUEC)   | 777,778  | 772,727   | 760,000  | 760,000   | 758,621    | 764,706   | 751,818    | 750,000   | 739,130   | 730,769   |
| % best                  | 100%     | 99%       | 98%      | 98%       | 98%        | 98%       | 97%        | 96%       | 95%       | 94%       |

This table compares ten rocks with identical mass and high-value ore percentages, but different [C-Tier ores](https://regolith.rocks/survey/ores?ot=C). The rock with Iron has the highest value per Mole, while Silicon has the lowest, highlighting the impact of C-Tier ore selection on mining profitability and efficiency.

## With A-Tier Ore

This table is similar to the S-Tier table, but uses a different set of ore values (A-Tier). The columns are sorted so that the highest value per Mole is on the left (Tungsten) and the lowest is on the right (Silicon).

- **Total Mass**: The mass of the rock (same for all).
- **Taranite % / C-Tier %**: The percentage of each ore type in the rock.
- **C-Tier Ore**: The specific [C-Tier ore](https://regolith.rocks/survey/ores?ot=C) in that column.
- **Value (aUEC)**: The total value of the rock.
- **Moles Filled**: How many Mole mining ship cargo holds the rock would fill.
- **Value per Mole (aUEC)**: The value of ore that fits in one Mole’s cargo hold.
- **% best**: The value per Mole as a percentage of the highest value in the row (Tungsten, 100%).

**Purpose:** This table lets you compare how different [C-Tier ores](https://regolith.rocks/survey/ores?ot=C) affect mining value and efficiency when paired with A-Tier ores, making it easy to see which ore combinations are most profitable.

| Property                | Tungsten  | Ice      | Quartz    | Titanium  | Tin      | Aluminum  | Iron     | Copper   | Corundum  | Silicon   |
|------------------------ |-----------|----------|----------|-----------|----------|-----------|----------|----------|-----------|-----------|
| Total Mass              | 50,000    | 50,000   | 50,000   | 50,000    | 50,000   | 50,000   | 50,000   | 50,000   | 50,000   | 50,000    |
| Taranite %              | 20%       | 20%      | 20%      | 20%       | 20%      | 20%       | 20%      | 20%      | 20%      | 20%       |
| C-Tier Ore              | Tungsten  | Ice      | Quartz   | Titanium  | Tin      | Aluminum  | Iron     | Copper   | Corundum  | Silicon   |
| C-Tier %                | 30%       | 30%       | 30%       | 30%       | 30%      | 30%       | 30%      | 30%      | 30%      | 30%       |
| Value (aUEC)            | 314,000   | 940,000  | 756,000  | 657,000   | 590,000  | 740,000   | 511,000  | 479,000  | 665,000   | 750,000   |
| Moles Filled            | 0.9       | 2.8      | 2.3      | 2.0       | 1.8      | 2.3       | 1.6      | 1.5      | 2.1       | 2.4       |
| Value per Mole (aUEC)   | 348,889   | 335,714  | 328,696  | 328,500   | 327,778  | 321,739   | 319,375  | 319,333  | 316,667   | 312,500   |
| % best                  | 100%      | 96%      | 94%      | 94%       | 94%      | 92%       | 92%      | 92%      | 91%       | 90%       |

## With B-Tier Ore

This table compares rocks with the same total mass and ore percentages, but with B-Tier ores included alongside [C-Tier ores](https://regolith.rocks/survey/ores?ot=C). Each column represents a different [C-Tier ore](https://regolith.rocks/survey/ores?ot=C), with Beryl as the B-Tier ore. The columns are sorted so that the highest mining value efficiency ("% best") is on the left and the lowest is on the right.

- **Total Mass**: The mass of the rock being analyzed (same for all).
- **Beryl % / C-Tier %**: The percentage of B-Tier and C-Tier ores in the rock.
- **C-Tier Ore**: The specific [C-Tier ore](https://regolith.rocks/survey/ores?ot=C) in that column.
- **Value (aUEC)**: The total in-game value of the rock, in aUEC (Star Citizen’s currency).
- **Moles Filled**: How many Mole mining ship cargo holds the rock would fill.
- **Value per Mole (aUEC)**: The value of ore that fits in one Mole’s cargo hold.
- **% best**: How each ore’s value per Mole compares to the best (highest) value in the row (Ice, in this case, is 100%).

**Purpose:** This table helps you see how the inclusion of B-Tier ores affects the value and efficiency of mining rocks, and how different [C-Tier ores](https://regolith.rocks/survey/ores?ot=C) compare in this context.

| Property                | Ice      | Tungsten  | Titanium  | Quartz    | Iron     | Tin      | Copper   | Corundum  | Aluminum  | Silicon   |
|------------------------ |----------|-----------|-----------|----------|----------|----------|----------|-----------|-----------|-----------|
| Total Mass              | 50,000   | 50,000    | 50,000    | 50,000     | 50,000    | 50,000    | 50,000    | 50,000    | 50,000    | 50,000    |
| Beryl %                 | 20%      | 20%       | 20%       | 20%      | 20%      | 20%      | 20%      | 20%       | 20%       | 20%       |
| C-Tier Ore              | Ice      | Tungsten  | Titanium  | Quartz   | Iron     | Tin      | Copper   | Corundum  | Aluminum  | Silicon   |
| C-Tier %                | 30%       | 30%       | 30%       | 30%       | 30%      | 30%       | 30%      | 30%      | 30%      | 30%       |
| Value (aUEC)            | 790,000  | 148,000   | 397,000   | 503,000  | 268,000  | 324,000  | 242,000  | 399,000   | 471,000   | 480,000   |
| Moles Filled            | 5.8      | 1.1       | 3.3       | 4.2      | 2.3      | 2.8      | 2.1      | 3.5       | 4.2       | 4.5       |
| Value per Mole (aUEC)   | 136,207  | 134,545   | 120,303   | 119,762  | 116,522  | 115,714  | 115,238  | 114,000   | 112,143   | 106,667   |
| % best                  | 100%     | 99%       | 88%       | 88%      | 86%      | 85%       | 85%      | 84%       | 82%       | 78%       |

---
