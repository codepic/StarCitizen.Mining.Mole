[💬 Send feedback on this page](https://github.com/codepic/StarCitizen.Mining.Mole/issues/new?template=feedback.yml&title=Feedback+on+C-Tier-Effect.md&page=C-Tier-Effect.md)  

# The Impact of B-Tier ore Mass-to-SCU Ratio on Value per Mole

## About B-Tier Ore Modifiers

1. **Modifiers Affect Profitability**: [B-Tier ores](https://regolith.rocks/survey/ores?ot=B) have properties that influence the behavior of rocks during mining. Since these ores will constitute the majority of the mass, their modifiers—such as Mass to SCU ratio, resistance, and instability—play a crucial role in determining the efficiency and profitability of mining operations.

2. **Cherry-Picking Favorable Modifiers**: By focusing on [B-Tier ores](https://regolith.rocks/survey/ores?ot=B) with favorable modifiers, miners can ensure that the rocks they target are easier to break, safer to handle, and more efficient to extract. This strategic selection minimizes risks and maximizes yields.

3. **Abundance**: [B-Tier ores](https://regolith.rocks/survey/ores?ot=B) are the most abundant, meaning most rocks will contain them. This abundance makes them a reliable indicator for identifying viable mining locations.

Even though these ores may ultimately be discarded, their impact on the overall mining process makes them a factor in choosing the right location.

| Material 🪨     | Clustering 🔗 | Explosion Strength 💥 | Instability ⚡ | Resistance 🛡️ | Green Zone Thinness 🟩 | Mass to SCU ⚖️ |
|:---------------|:-------------:|:---------------------:|:-------------:|:-------------:|:---------------------:|:---------------:|
| Beryl          |      40       |        ✅ 20           |    ✅ 350     |    ✅ 65%     |      ✅ +150%         |      ✅ 92      |
| Hephaestanite  |     ✅ 50     |        100            |     550       |     50%       |      ✅ +50%          |      107        |
| Borase         |     ✅ 40     |        100            |      40       |     30%       |      +150%            |      150        |
| Agricium       |      20       |         4             |     350       |     50%       |      +200%            |     ❌ 240      |
| Laranite       |      40       |        200            |     400       |     50%       |      +50%             |     ❌ 384      |

### Explanation of Table Columns

- **Material 🪨**: The type of ore or resource being mined.
- **Clustering 🔗**: Indicates how well each type of mineral tends to stick together. Higher values mean cleaner splits, where the valuable minerals remain in their own breaks and the less valuable ones in theirs. **Higher values are more profitable**.
- **Explosion Strength 💥**: Represents the intensity of potentially explosive reactions during mining. **Lower values are safer**.
- **Instability ⚡**: Instability measures how erratic the energy input/output curve is during mining. High instability means the energy bar will fluctuate wildly, making it harder to keep the rock in the optimal green zone. **Lower values are easier**.
- **Resistance 🛡️**: Resistance is how much energy the rock absorbs before it starts to fracture. Higher resistance means you’ll need more powerful lasers or longer charge times to break it apart. **Lower values are easier**.
- **Green Zone Thinness 🟩**: This affects how narrow the “sweet spot” is for maintaining energy during fracturing. A thinner green zone demands more precision and control to avoid overcharging or undercharging. **Lower values are easier**.
- **Mass to SCU ⚖️**: The mass of the resource required to fill one Standard Cargo Unit (SCU). **Lower values are more profitable**.

## How Does B-Tier Ore Mass to SCU Affect Profitability?

The mass-to-SCU ratio determines how much ore is needed to fill a cargo unit. Lower ratios mean you fill your hold with less mass, increasing profit per SCU. The following section explores how [B-Tier ore](https://regolith.rocks/survey/ores?ot=B)’s mass-to-SCU impacts mining returns.

*Source: Calculations made with [Regolith's Cluster Calculator](https://regolith.rocks/cluster)*

### Table Column Explanation

- **Total Mass**: The mass of the rock being analyzed (same for all).
- **Stileron % / Taranite % / C-Tier %**: The percentage of each ore type in the rock.
- **B-Tier Ore**: The specific [B-Tier ore](https://regolith.rocks/survey/ores?ot=B) in that column.
- **Value (aUEC)**: The total in-game value of the rock, in aUEC (Star Citizen’s currency).
- **Moles Filled**: How many Mole mining ship cargo holds the rock would fill.
- **Value per Mole (aUEC)**: The value of ore that fits in one Mole’s cargo hold.
- **% best**: How each ore’s value per Mole compares to the best (highest) value in the row (Iron, in this case, is 100%).

## With S-Tier Ore (Stileron)

The following table compares rocks with the presence of S-Tier Ore (`Stileron`), same total mass, and same A-Tier Ore (`Taranite`), but different [B-Tier ores](https://regolith.rocks/survey/ores?ot=B). Each column represents a different [B-Tier ore](https://regolith.rocks/survey/ores?ot=B) and its effect on `Value per Mole`.

**Purpose:** The table below shows how the choice of [B-Tier ore](https://regolith.rocks/survey/ores?ot=B) affects value and efficiency, in the presence of S-Tier ores.

| Property              | Agricium | Beryl    | Laranite | Borase   | Hephaestanite |
|:----------------------|:--------:|:--------:|:--------:|:--------:|:-------------:|
| Total Mass            | 50,000   | 50,000   | 50,000   | 50,000   | 50,000        |
| Stileron %            | 10%      | 10%      | 10%      | 10%      | 10%           |
| Taranite %            | 20%      | 20%      | 20%      | 20%      | 20%           |
| B-Tier Ore            | Agricium | Beryl    | Laranite | Borase   | Hephaestanite |
| B-Tier %              | 30%      | 30%      | 30%      | 30%      | 30%           |
| Value (aUEC)          | 1,600,000| 2,200,000| 1,300,000| 1,900,000| 2,000,000     |
| Moles Filled          | 1.8      | 2.5      | 1.5      | 2.2      | 2.4           |
| Value per Mole (aUEC) | 888,889  | 880,000  | 866,667  | 863,636  | 833,333       |
| % best                | 100%     | 99%      | 97%      | 97%      | 93%           |

---

## With A-Tier Ore (Taranite)

The following table is otherwise same as the `S-Tier Ore` table above, but `S-Tier Ore` removed.

**Purpose:** The table below shows how the choice of [B-Tier ore](https://regolith.rocks/survey/ores?ot=B) affects value and efficiency, in the presence of A-Tier ores.

| Property              |   Borase   |  Laranite  |   Beryl    | Hephaestanite |  Agricium  |
|:---------------------:|:----------:|:----------:|:----------:|:-------------:|:----------:|
| Total Mass            |   50,000   |   50,000   |   50,000   |    50,000     |   50,000   |
| Taranite %            |    20%     |    20%     |    20%     |     20%       |    20%     |
| B-Tier Ore            |   Borase   |  Laranite  |   Beryl    | Hephaestanite |  Agricium  |
| B-Tier %              |    30%     |    30%     |    30%     |     30%       |    30%     |
| Value (aUEC)          |  945,000   |  580,000   | 1,000,000  |   947,000     |  726,000   |
| Moles Filled          |    2.0     |    1.3     |    2.3     |     2.2       |    1.7     |
| Value per Mole (aUEC) | 472,500    | 446,154    | 434,783    | 430,455       | 427,059    |
| % best                | 100%       | 94%        | 92%        | 91%           | 90%        |

---

## With C-Tier Ore (Tin)

The following table is otherwise same as the `A-Tier Ore` table above, but `A-Tier Ore` removed.

**Purpose:** The table below shows how the choice of [B-Tier ore](https://regolith.rocks/survey/ores?ot=B) affects value and efficiency, then the B-Tier Ore is the highest ore present in the rock.

| Property              |   Borase   |   Beryl    |  Laranite  |  Agricium  | Hephaestanite |
|:---------------------:|:----------:|:----------:|:----------:|:----------:|:-------------:|
| Total Mass            |   50,000   |   50,000   |   50,000   |   50,000   |    50,000     |
| Tin %                 |    20%     |    20%     |    20%     |    20%     |     20%       |
| B-Tier Ore            |   Borase   |   Beryl    |  Laranite  |  Agricium  | Hephaestanite |
| B-Tier %              |    30%     |    30%     |    30%     |    30%     |     30%       |
| Value (aUEC)          |  468,000   |  497,000   |  227,000   |  291,000   |   400,000     |
| Moles Filled          |    2.6     |    3.2     |    1.5     |    2.0     |     3.0       |
| Value per Mole (aUEC) | 180,000    | 155,313    | 151,333    | 145,500    | 133,333       |
| % best                | 100%       | 86%        | 84%        | 81%        | 74%           |
