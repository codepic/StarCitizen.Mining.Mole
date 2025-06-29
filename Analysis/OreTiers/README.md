# The Relationship between Mass-to-SCU Ratio and Value per Mole in Star Citizen Mining

## Abstract

This study investigates whether the mass-to-SCU (Standard Cargo Unit) ratio of mineable ores influences mining profitability in Star Citizen. Using controlled scenario modeling, in-game data, and community-sourced calculations, we examine how ore density impacts value-per-trip efficiency across different rock compositions. Contrary to popular belief, the results reveal that **mass-to-SCU alone is not a reliable predictor of profitability**. Instead, profitability is shaped by contextual interactions between ore types, their intrinsic values, and role-specific mining constraints. These findings challenge density-first heuristics and lay the foundation for more nuanced, context-aware mining strategies.

---

## Background and Hypothesis

### Background

With the release of Star Citizen Alpha 3.19, the mining system underwent a significant shift: the standardized conversion rate of 1 SCU equaling 50 mass was replaced by ore-specific density values. Now, each ore fills cargo space based on its own mass-to-SCU ratio, introducing variability in how rocks translate to haulable volume and value. This change has added complexity to mining strategies, as two rocks of equal mass and percentage composition can now yield vastly different SCU depending on the density of their materials.

This density-driven cargo behavior fundamentally alters how miners assess profitability. Where once all rocks offered roughly equivalent value per weight, miners must now account for how “dense” an ore is in filling cargo—and whether that density helps or hinders profits per trip.

### Community Hypotheses

Two dominant player-driven hypotheses have emerged from community discussions in response to these changes:

1. **Density-Efficiency Hypothesis**  
   Lower mass-to-SCU ores are more profitable because they fill cargo space with less mass. This allows for fewer trips, higher sellable volume, and better value-per-trip metrics. As a result, players have gravitated toward lighter ores such as Bexalite, Beryl, and Quantanium, while deprioritizing heavier ores like Gold and Agricium.  
   *Source: [Reddit - Mass to SCU values in 3.19 (Mining)](https://www.reddit.com/r/starcitizen/comments/13hko27/mass_to_scu_values_in_319_mining/)*

2. **B-Tier Targeting Hypothesis**  
   Because B-Tier ores commonly appear in rocks across Stanton and Pyro, some mining guides recommend using the mass-to-SCU properties of B-Tier ores as the primary lens for assessing profitability. In this strategy, choosing a mining location or target rock hinges on how favorable the B-Tier ore composition is.  
   *Source: [YouTube - Star Citizen Mining Guide](https://www.youtube.com/watch?v=-7KyJ8NsOUc&t=2168s)*

### Study Hypothesis

This study evaluates whether the mass-to-SCU ratio of mineable ores is a reliable predictor of mining profitability in Star Citizen. The hypothesis, drawn from community consensus, asserts that ores with lower mass-to-SCU values allow for more efficient cargo utilization and thus yield higher value per mining trip.

To test this, the study examines value-per-Mole outcomes across multiple rock configurations (S-, A-, and C-Tier pairings), holding total rock mass and ore percentages constant. This controlled approach isolates the impact of ore density on trip efficiency, allowing for a focused investigation into whether lighter ores consistently outperform their denser counterparts in profitability.

Ultimately, the goal is to verify whether **mass-to-SCU alone** can serve as a dependable mining heuristic, or if ore profitability is driven by more complex, context-sensitive interactions.

---

## Scope

This study focuses exclusively on evaluating the direct relationship between the mass-to-SCU ratio of Tiered ores and their contribution to value-per-trip profitability in Star Citizen. The analysis isolates the impact of ore density by controlling for total rock mass and ore composition across all scenarios, allowing us to assess value per Mole as the primary efficiency metric.

Importantly, this scope does not include downstream systems such as refining yield, processing duration, travel logistics, or fuel costs. While these factors certainly influence real-world profitability, they fall outside the parameters of this density-focused analysis and are identified as areas for future research.

By narrowing the scope in this way, the study aims to establish a clear foundational understanding of how ore density—in isolation—affects unrefined cargo value and trip efficiency. This allows for more targeted insights that can later be expanded upon with broader, system-level modeling.

---

## Methodology

This study uses scenario-based simulation to evaluate the effect of ore mass-to-SCU ratios on mining profitability, specifically in the context of value-per-trip efficiency. The analysis draws from both in-game mechanics and community-calculated data, employing a consistent framework across multiple ore tiers to isolate density as the primary variable.

- **Data Sources**: All mass-to-SCU values, ore percentages, and per-unit sale prices were derived from a combination of live game observations and trusted community tools, such as Regolith's Cluster Calculator. These tools provide granular data on material densities and value per SCU, reflecting mechanics current to Star Citizen 4.1.1.

- **Controlled Variables**: To isolate the effect of ore density, each scenario fixed the total rock mass and ore composition percentages. Only the identity of the targeted ore was varied in each test case, enabling direct comparison of how mass-to-SCU ratios influence trip value.

- **Scenario Construction**: Each experiment modeled a three-ore rock composition, drawing from S-, A-, B-, or C-Tier ores depending on the tier under study. These compositions were selected to reflect realistic in-game spawning patterns while still enabling variable control.

- **Reference Vessel**: The ARGO Mole was used as the reference ship for all value-per-trip calculations. As a staple of group mining operations, the Mole provides a consistent mining and cargo baseline while illustrating how ore density affects volume-filling efficiency.

- **Metrics Calculated**:
  - *Value per Mole*: Estimated haul value assuming full cargo loads of rocks with a specific composition.
  - *% Best*: Relative efficiency of each ore setup, indexed against the most profitable configuration within that scenario.
  - *SCU Filled per Rock*: Derived from the ore’s mass-to-SCU ratio and its share of rock mass.

- **Assumptions**:
  - All rocks modeled share an identical mass (typically 50,000 kg) with fixed percentage distributions among ores.
  - No post-mining processes (e.g. refining losses, haul time, pricing variation) were modeled.
  - Mining difficulty, gadget use, and multi-laser considerations were held constant or excluded from scope.

By structuring the methodology in this way, the study ensures internal consistency while preserving meaningful comparability across ore tiers and compositions.

---

## A-Tier Ore Analysis: Findings vs. Hypothesis

A prevailing hypothesis within the mining community suggests that **ores with a lower mass-to-SCU ratio should yield greater profitability**, as they require less mass to fill cargo space—thus, delivering higher value per trip. This logic forms the backbone of a density-first mining strategy, especially relevant for mass-constrained ships like the Mole.

However, the analysis of A-Tier ores challenges this assumption.

### A-Tier Ore Comparison Table

This table summarizes how each A-Tier ore performed across three rock compositions, showing how context influences profitability beyond raw density values.

| Ore        | Mass-to-SCU ⚖️ | Value per Mole (Stileron) | % Best | Value per Mole (Laranite) | % Best | Value per Mole (Quartz) | % Best |
|------------|----------------|----------------------------|--------|---------------------------|--------|--------------------------|--------|
| Bexalite   | ✅ 231         | 727,273                    | 77%    | 914,286                   | 88%    | 962,963                  | 90%    |
| Taranite   | 340            | 763,636                    | 81%    | 952,381                   | 92%    | 1,000,000                | 93%    |
| Gold       | 644            | 944,444                    | 100%   | 1,035,714                 | 100%   | 1,075,472                | 100%   |

**Note:** While Gold (highest mass-to-SCU) dominates in the Stileron scenario, its advantage fades relative to Taranite and Bexalite when paired with denser ores. This emphasizes the contextual nature of ore performance.

---

Across three rock configurations—paired with S-Tier (Stileron), B-Tier (Laranite), and C-Tier (Quartz) ores—the correlation between mass-to-SCU and value per Mole does not consistently hold:

- In the Stileron scenario, **higher mass-to-SCU ores like Gold** surprisingly delivered the highest value per Mole.
- In the Laranite and Quartz scenarios, **lower-density ores like Taranite outperformed Gold**, despite the latter’s theoretically higher density-to-value potential.

These results indicate that **mass-to-SCU ratio alone is not a reliable predictor of profitability**. Instead, the ore composition of the surrounding rock appears to influence the outcome—suggesting that profitability is a contextual interaction, not a standalone attribute.

This finding prompts a reassessment of “density-efficient” mining and underscores the need to evaluate ore combinations holistically rather than in isolation.

---

## B-Tier Ore Analysis: Findings vs. Hypothesis

The working hypothesis asserts that **lower mass-to-SCU ores should result in greater mining profitability**, assuming that less mass required to fill a cargo unit equates to higher value concentration per trip. This concept aligns with the idea of density-efficient mining—especially relevant when B-Tier ores make up the majority of rock mass.

However, the findings across all three scenarios—paired with S-, A-, and C-Tier ores—complicate this narrative:

### B-Tier Ore Comparison Table

This table summarizes how B-Tier ores perform in terms of value-per-trip efficiency across three different rock compositions, highlighting the contextual volatility of mass-to-SCU as a predictive metric.

| Ore           | Mass-to-SCU ⚖️ | Value per Mole (Stileron) | % Best | Value per Mole (Taranite) | % Best | Value per Mole (Quartz) | % Best |
|---------------|----------------|----------------------------|--------|---------------------------|--------|--------------------------|--------|
| Beryl         | ✅ 92          | 694,444                    | 78%    | 820,000                   | 87%    | 862,069                  | 86%    |
| Hephaestanite | 107            | 694,444                    | 78%    | 866,667                   | 91%    | 920,690                  | 92%    |
| Borase        | 150            | 805,556                    | 91%    | 914,286                   | 96%    | 1,000,000                | 100%   |
| Agricium      | ❌ 240         | 888,889                    | 100%   | 952,381                   | 100%   | 931,034                  | 93%    |
| Laranite      | ❌ 384         | 763,636                    | 86%    | 914,286                   | 96%    | 827,586                  | 83%    |

**Note:** Despite Beryl having the lowest mass-to-SCU, it consistently underperforms in value per Mole, while higher-density ores like Agricium and Borase dominate. These findings further erode the assumption that lower mass automatically translates to higher profitability.

---

- In the S-Tier setup, **Agricium**, despite having one of the *highest* mass-to-SCU ratios (240), delivered the highest value per Mole.
- **Beryl**, the *lowest* density ore (92 mass-to-SCU), consistently underperformed in value-per-Mole across multiple rock compositions.
- **Borase**, with a middling density (150), frequently emerged as the top performer when B-Tier ores were the primary value driver.

These outcomes indicate that **mass-to-SCU is not a reliable predictor of profitability for B-Tier ores**. The interaction with co-occurring ores—especially when B-Tier is the dominant component—introduces variance that overrides the expected linear relationship between density and efficiency.

Taken together with the A-Tier analysis, this data supports a revised interpretation: **ore profitability is context-dependent**, and density-based strategies should be applied selectively, with consideration for the full composition of the rock rather than any one tier in isolation.

---

## C-Tier Ore Analysis: Findings vs. Hypothesis

The working hypothesis contends that **lower mass-to-SCU C-Tier ores should lead to higher profitability**, on the assumption that rocks composed of lighter filler materials leave more room for high-value ores—improving value density and trip efficiency.

Yet, across all configurations—paired with S-, A-, and B-Tier ores—this hypothesis once again fails to hold:

### C-Tier Ore Comparison Table

This table summarizes the relative efficiency of C-Tier ores across three rock configurations—highlighting how heavier ores like Iron and Tungsten often defy expectations by outperforming lighter options.

| Ore        | Mass-to-SCU ⚖️ | Value per Mole (Stileron/Taranite) | % Best | Value per Mole (Taranite Only) | % Best | Value per Mole (Beryl) | % Best |
|------------|----------------|-------------------------------------|--------|-------------------------------|--------|-------------------------|--------|
| Ice        | ✅ 34          | 758,621                             | 98%    | 335,714                        | 96%    | 136,207                 | 100%   |
| Titanium   | ⚠️ 150         | 772,727                             | 99%    | 328,500                        | 94%    | 120,303                 | 88%    |
| Quartz     | ✅ 89          | 760,000                             | 98%    | 328,696                        | 94%    | 119,762                 | 88%    |
| Aluminum   | ✅ 90          | 760,000                             | 98%    | 321,739                        | 92%    | 112,143                 | 82%    |
| Iron       | ❌ 263         | 777,778                             | 100%   | 319,375                        | 92%    | 116,522                 | 86%    |
| Tungsten   | ❌ 644         | 751,818                             | 97%    | 348,889                        | 100%   | 134,545                 | 99%    |
| Silicon    | ✅ 78          | 730,769                             | 94%    | 312,500                        | 90%    | 106,667                 | 78%    |

**Note:** Iron (highest value in S-Tier scenario) and Tungsten (top in A-Tier) outperform many lighter ores. This supports the conclusion that value-per-Mole is driven more by ore interactions and intrinsic value than by mass-to-SCU alone.

---

- In the S-Tier pairing, **Iron**, one of the *heaviest* ores (263 mass-to-SCU), paradoxically delivers the *highest value per Mole*, outperforming lighter alternatives like Ice and Quartz.
- With A-Tier ores, **Tungsten** (644⚠️)—the densest material in the table—ranks first in value per Mole, while Silicon (78✅) finishes last.
- Even when B-Tier ore is held constant (Beryl), **Ice** performs best, but **Tungsten ranks second**, suggesting that even high-density ores can compete or surpass lighter ones in value-per-trip efficiency.

These findings reinforce the emerging theme: **mass-to-SCU is not a reliable standalone predictor of profitability**. In practice, an ore’s *intrinsic value*, *percentage composition*, and *interactions within a given rock* can easily override theoretical density advantages. The C-Tier results emphasize that even in bulk filler roles, ore choice shapes mining returns in complex, non-linear ways.

Thus, miners chasing efficiency must evaluate not just ore density, but the broader context of **rock makeup, value stacking, and expected output**, making nuanced strategic targeting far more effective than rigid density-driven heuristics.

---

## Conclusion

This study set out to evaluate whether the mass-to-SCU ratio of mineable ores predicts mining profitability in Star Citizen, with a focus on value per Mole across A-, B-, and C-Tier compositions. Contrary to popular belief, the results demonstrated that **mass-to-SCU alone is not a reliable indicator of profitability**. Instead, the economic efficiency of a mining trip is shaped by the complex interaction of ore value, composition percentage, and rock pairing context.

Across all tiers, heavier ores frequently outperformed lighter ones in value-per-trip metrics—challenging density-first mining strategies and highlighting the need for more nuanced decision-making.

These findings lay the groundwork for broader explorations into refining impacts, travel dynamics, and real-time yield optimization, which are addressed in the Discussion section.

---

## Discussion

The results of this study challenge the commonly accepted belief that lower mass-to-SCU ores inherently lead to higher mining profitability. Across all ore tiers, the expected inverse relationship between density and value per Mole was found to be inconsistent, context-dependent, and in some cases, entirely inverted. These findings raise doubts about the utility of mass-to-SCU as a universal predictor of mining efficiency.

However, it would be premature to entirely dismiss the value of the mass-to-SCU ratio in practical applications. As a quick heuristic, it remains useful—particularly when considering the **physical feasibility of breaking a rock**. Denser ores increase the total rock mass significantly, which can make rocks mechanically unmineable, especially for solo players using smaller mining lasers or unsupported platforms. This highlights the need for **role-specific predictors**: what may be an efficient target for a group Mole crew may be completely unviable for a solo Prospector pilot. Universal efficiency metrics fail to account for these situational limitations.

Additionally, at smaller rock sizes (e.g., 15,000 kg), even modest volume percentages of high-mass-to-SCU ores dominate the mass composition. In such cases, the presence of a dense material—especially when paired with a high SCU contribution—can dramatically shape both the practical minability and the profitability profile of the rock. This adds yet another layer of context sensitivity, especially in gameplay scenarios involving fast scans or high-throughput mining.

Another avenue for future research involves examining **value-to-mass-to-scu ratios**, which may offer a more precise measure of how economically efficient a material is, independent of cargo constraints. Furthermore, this study excluded refining costs, time-to-sale, and travel overhead—factors which, if included, could amplify or mute some of the observed outcomes.

Lastly, the study emphasizes the importance of evaluating rocks **as value compositions**, not as a sum of isolated parts. High-value ores can mitigate the inefficiencies introduced by lower-tier fillers, but only when their combined behavior aligns with player capabilities and mission intent.

In summary, while mass-to-SCU should not be treated as a standalone efficiency metric, it does retain value as a **situational filter**—especially when interpreted through the lens of miner role, rock mass, and ore distribution. Developing adaptable heuristics that incorporate context-aware variables may be the key to truly optimizing mining strategies within Star Citizen’s evolving economy.

---

## Limitations

- **Dynamic Game Environment**: This study is grounded in Star Citizen's mechanics and ore data as of version 3.19. Future patches may adjust core systems, including ore compositions, values, or mining physics—potentially impacting the relevance of these findings.

- **Assumed Constants**: The methodology holds variables such as total rock mass and percentage composition constant to isolate the mass-to-SCU factor. While this strengthens internal validity, it may not reflect the variability of organic rock spawns encountered in the game.

- **No Refining or Logistics Consideration**: The study excludes downstream processes such as refinery yields, processing duration, travel time, fuel cost, and market fluctuations. These real-world constraints likely affect profitability and decision-making but are out of scope here.

- **Miner Type Constraints**: The study does not differentiate between different miner types. Some rocks included in the analysis may be impractical for solo miners due to mass thresholds or fracture resistance. What is profitable for one miner profile may be infeasible for another.

- **Limited Rock Size Modeling**: All scenarios assume a fixed rock mass (typically 50,000 kg). In practice, smaller rocks (e.g., 15,000 kg) alter how ore mass distribution behaves—particularly when high mass-to-SCU materials dominate SCU contributions.

- **Simulation, Not Field Testing**: All conclusions are drawn from theoretical modeling. While every effort was made to reflect in-game realities, field testing and practical mining trials are still needed to validate the simulation logic and profitability outcomes.

---

## Community Impact

The findings of this study have meaningful implications for Star Citizen’s player community—particularly for those building or relying on resource extraction projections, economic modeling tools, and strategic mining guides.

By rigorously debunking the assumption that mass-to-SCU is a dependable universal predictor of profitability, this research provides a new foundation for refining how miners assess and prioritize ore targets. Developers of mining tools, calculators, or efficiency heuristics can now integrate these findings to improve their algorithms, especially when modeling real-world profitability beyond surface-level density metrics.

For mining-focused organizations and solo players alike, the results encourage a shift away from rigid rules-of-thumb and toward context-sensitive decision-making. Rather than assuming that “lighter is better,” the community now has evidence that rock composition, ore pairing, and miner role significantly affect outcomes—opening the door for more nuanced training, scouting evaluation, and on-the-fly strategy adjustments.

Additionally, this study highlights the importance of simulation and data-driven experimentation within a virtual economy. As mining continues to evolve with patch changes and economic balancing, the ability for players to question established beliefs and validate theories through analysis will be key to maintaining competitiveness—and deepening the metagame for resource extraction at scale.

---

## Further Research

This study opens several avenues for continued exploration into mining profitability and decision-making within Star Citizen’s evolving economy. While the results clearly demonstrate that mass-to-SCU alone is not a sufficient predictor of mining efficiency, a number of unresolved questions remain:

- **Value-to-Mass Efficiency**: A potential next step is analyzing the relationship between ore *value per kilogram* and profitability. This could reveal whether value-weighted density metrics offer better predictive power than raw SCU efficiency.

- **Refining Yield and Time Analysis**: Including refinery performance—both in terms of material losses and processing duration—may reshape the profitability landscape. High-density ores that refine quickly could ultimately outperform lighter alternatives in time-constrained mining loops.

- **Transport and Logistics Modeling**: Factoring in travel time, jump distances, and ship-specific cargo capacities may shift the equation. Understanding how logistics scale with ore composition could provide role-specific insights for solo miners, group crews, or industrial orgs.

- **Dynamic Pricing and Market Behavior**: Incorporating trade route analysis, dynamic price volatility, and location-based demand could help determine which ores are most profitable *at the time of sale*—not just at the point of extraction.

- **Rock Detection and Spawn Behavior**: Future studies could include an analysis of how often specific rock compositions appear in the wild. If the most “profitable” rocks are statistically rare or hard to find, that affects the overall strategy miners should adopt.

- **Heuristic Development by Role**: Rather than seeking a single universal mining metric, further research should aim to create **role-based heuristics** for solo players, duos, and full crews. Efficiency looks different depending on time constraints, gear loadouts, and risk tolerance.

- **Simulation Tools and Decision Models**: Finally, development of real-time simulation or decision-support tools could help miners optimize targets on the fly, integrating mass, value, ship capacity, refining availability, and player-specific constraints.

These areas offer fertile ground for more granular, context-sensitive mining analytics—and would help move the community from simple heuristics toward data-driven strategies that reflect the full complexity of Star Citizen’s mining ecosystem.

---