[💬 Send feedback on this page](https://github.com/codepic/StarCitizen.Mining.Mole/issues/new?template=feedback.yml&title=Feedback+on+C-Tier-Effect.md&page=C-Tier-Effect.md)  

# The Impact of A-Tier ore Mass-to-SCU Ratio on Value per Mole

## About A-Tier ore Modifiers

1. **Modifiers Affect Profitability**: [A-Tier ores](https://regolith.rocks/survey/ores?ot=A) have properties that influence the behavior of rocks during mining. Since these ores will constitute the majority of the mass, their modifiers—such as Mass to SCU ratio, resistance, and instability—play a crucial role in determining the efficiency and profitability of mining operations.

2. **Cherry-Picking Favorable Modifiers**: By focusing on [A-Tier ores](https://regolith.rocks/survey/ores?ot=A) with favorable modifiers, miners can ensure that the rocks they target are easier to break, safer to handle, and more efficient to extract. This strategic selection minimizes risks and maximizes yields.

3. **Abundance**: [A-Tier ores](https://regolith.rocks/survey/ores?ot=A) are the most abundant, meaning most rocks will contain them. This abundance makes them a reliable indicator for identifying viable mining locations.

Even though these ores may ultimately be discarded, their impact on the overall mining process makes them a factor in choosing the right location.

| Material 🪨 | Clustering 🔗 | Explosion Strength 💥 | Instability ⚡ | Resistance 🛡️ | Green Zone Thinness 🟩 | Mass to SCU ⚖️ |
|:-----------|-------------:|---------------------:|-------------:|------------:|----------------------:|---------------:|
| Bexalite   |            5 |                 ✅ 100  |          600 |         ✅ 60% |                 ✅ +40% |          ✅ 231 |
| Taranite   |           ✅ 10 |                 240  |          700 |         50% |                 +60% |          340 |
| Gold       |            5 |                 100  |          ✅ 550 |         50% |                +210% |          644 |

### Explanation of Table Columns

- **Material 🪨**: The type of ore or resource being mined.
- **Clustering 🔗**: Indicates how well each type of mineral tends to stick together. Higher values mean cleaner splits, where the valuable minerals remain in their own breaks and the less valuable ones in theirs. **Higher values are more profitable**.
- **Explosion Strength 💥**: Represents the intensity of potentially explosive reactions during mining. **Lower values are safer**.
- **Instability ⚡**: Instability measures how erratic the energy input/output curve is during mining. High instability means the energy bar will fluctuate wildly, making it harder to keep the rock in the optimal green zone. **Lower values are easier**.
- **Resistance 🛡️**: Resistance is how much energy the rock absorbs before it starts to fracture. Higher resistance means you’ll need more powerful lasers or longer charge times to break it apart. **Lower values are easier**.
- **Green Zone Thinness 🟩**: This affects how narrow the “sweet spot” is for maintaining energy during fracturing. A thinner green zone demands more precision and control to avoid overcharging or undercharging. **Lower values are easier**.
- **Mass to SCU ⚖️**: The mass of the resource required to fill one Standard Cargo Unit (SCU). **Lower values are more profitable**.

## How Does A-Tier ore Mass to SCU Affect Profitability?

The mass-to-SCU ratio determines how much ore is needed to fill a cargo unit. Lower ratios mean you fill your hold with less mass, increasing profit per SCU. The following section explores how [A-Tier ore](https://regolith.rocks/survey/ores?ot=A)’s mass-to-SCU impacts mining returns.

*Source: Calculations made with [Regolith's Cluster Calculator](https://regolith.rocks/cluster)*

### Table Column Explanation

- **Total Mass**: The mass of the rock being analyzed (same for all).
- **Stileron % / Taranite % / C-Tier %**: The percentage of each ore type in the rock.
- **A-Tier ore**: The specific [A-Tier ore](https://regolith.rocks/survey/ores?ot=A) in that column.
- **Value (aUEC)**: The total in-game value of the rock, in aUEC (Star Citizen’s currency).
- **Moles Filled**: How many Mole mining ship cargo holds the rock would fill.
- **Value per Mole (aUEC)**: The value of ore that fits in one Mole’s cargo hold.
- **% best**: How each ore’s value per Mole compares to the best (highest) value in the row (Iron, in this case, is 100%).

## With S-Tier Ore (Stileron)

The following table compares rocks with the presence of S-Tier Ore (`Stileron`), same total mass, and same B-Tier Ore (`Laranite`), but different [A-Tier ores](https://regolith.rocks/survey/ores?ot=A). Each column represents a different [A-Tier ore](https://regolith.rocks/survey/ores?ot=A) and its effect on `Value per Mole`.

**Purpose:** The table below shows how the choice of [A-Tier ore](https://regolith.rocks/survey/ores?ot=A) affects value and efficiency, in the presence of S-Tier ores.

| Property              | Gold      | Taranite | Bexalite |
|:----------------------|:---------:|:--------:|:--------:|
| Total Mass            | 50,000    | 50,000   | 50,000   |
| Stileron %            | 10%       | 10%      | 10%      |
| Laranite %            | 20%       | 20%      | 20%      |
| A-Tier ore            | Laranite  | Beryl    | Agricium |
| A-Tier %              | 30%       | 30%      | 30%      |
| Value (aUEC)          | 1,500,000 | 1,400,000| 1,600,000|
| Moles Filled          | 1.3       | 1.5      | 1.8      |
| Value per Mole (aUEC) | 1,153,846 | 933,333  | 888,889  |
| % best                | 100%      | 81%      | 77%      |

---

## With B-Tier Ore (Laranite)

The following table is otherwise same as the `S-Tier Ore` table above, but `S-Tier Ore` removed.

**Purpose:** The table below shows how the choice of [A-Tier ore](https://regolith.rocks/survey/ores?ot=A) affects value and efficiency, in the presence of B-Tier ores.

| Property              | Taranite | Bexalite | Gold      |
|:---------------------:|:--------:|:--------:|:---------:|
| Total Mass            | 50,000   | 50,000   | 50,000    |
| Laranite %            | 20%      | 20%      | 20%       |
| A-Tier ore            | Laranite | Borase   | Beryl     |
| A-Tier %              | 30%      | 30%      | 30%      |
| Value (aUEC)          | 729,000  | 736,000  | 370,000   |
| Moles Filled          | 1.3      | 1.6      | 0.9       |
| Value per Mole (aUEC) | 560,769  | 460,000  | 411,111   |
| % best                | 100%     | 82%      | 73%       |

---

## With C-Tier Ore (Quartz)

The following table is otherwise same as the `B-Tier Ore` table above, but `B-Tier Ore` replaced with a `C-Tier Ore (Quartz)`.

**Purpose:** The table below shows how the choice of [A-Tier ore](https://regolith.rocks/survey/ores?ot=A) affects value and efficiency, then the A-Tier ore is the highest ore present in the rock.

| Property              | Taranite   | Bexalite   | Gold       |
|:---------------------:|:----------:|:----------:|:----------:|
| Total Mass            |   50,000   |   50,000   |   50,000   |
| Quartz %              |    20%     |    20%     |    20%     |
| A-Tier ore            |   Beryl    |   Borase   |  Laranite  |
| A-Tier %              |    30%     |    30%     |    30%     |
| Value (aUEC)          |  889,000   |  961,000   |  378,000   |
| Moles Filled          |    1.9     |    2.5     |    1.1     |
| Value per Mole (aUEC) | 468,947    | 384,400    | 343,636    |
| % best                | 100%       | 82%        | 73%        |
