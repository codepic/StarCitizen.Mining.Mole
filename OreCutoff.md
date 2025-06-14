# 7. Ore Cutoff Percentages & Rock Evaluation

*Background:*
Many times, I've tried to set myself a strict cutoff before going mining—only to realize that, in practice, I end up breaking my own "promise" here and there. This document was born from analyzing the factors that cause me (and likely others) to steer away from a predefined A-tier cutoff. By understanding these factors, we can treat a predefined cutoff not as a rigid rule, but as a dynamic target. This approach lets us adapt our decisions to the actual rock compositions we encounter, while still aiming for a consistent, reliable financial outcome over time.

> **Note:** While this document describes calculations you can make in the field, it's not intended that everyone mines with a calculator or spreadsheet in hand. Remember to have fun, relax, and review your decision-making process. At first, you might take a more rigid approach to mining decisions, but soon enough it should become a natural habit—knowing your choices are grounded in deterministic science and math, not just whim or guesswork.

Understanding which rocks are worth mining is a common question for both new and experienced miners. The answer depends on the composition of the rock, the value of its minerals, your own mining goals, your specific setup, crew, and other situational factors. This section provides practical guidelines for evaluating rocks based on ore cutoff percentages, using the S, A, B, and C tier system as described on [Regolith Rocks](https://regolith.rocks/survey/ores).

## 7.1 Ore Tiers Explained

Below are the most relevant mining ores, their acronyms, and approximate values (per SCU) as of June 2025. For a full, up-to-date list, see [Regolith Rocks Ore Survey](https://regolith.rocks/survey/ores) and [UEX Corp Commodities](https://uexcorp.space/commodities).

### S-Tier Ores
| Ore Name   | Acronym | Value (UEC/SCU) |
|------------|---------|-----------------|
| Quantanium | QUAN    | 22,000          |
| Stileron   | STIL    | 28,000          |
| Riccite    | RICC    | 21,000          |

### A-Tier Ores
| Ore Name  | Acronym | Value (UEC/SCU) |
|-----------|---------|-----------------|
| Taranite  | TARA    | 9,000           |
| Bexalite  | BEXA    | 7,000           |
| Gold      | GOLD    | 6,000           |

### B-Tier Ores
| Ore Name      | Acronym | Value (UEC/SCU) |
|---------------|---------|-----------------|
| Laranite      | LARA    | 3,000           |
| Borase        | BORA    | 3,000           |
| Beryl         | BERY    | 3,000           |
| Agricium      | AGRI    | 2,000           |
| Hephaestanite | HEPH    | 2,000           |

### C-Tier Ores
| Ore Name   | Acronym | Value (UEC/SCU) |
|------------|---------|-----------------|
| Tungsten   | TUNG    | 614             |
| Titanium   | TITA    | 451             |
| Silicon    | SILI    | 197             |
| Iron       | IRON    | 372             |
| Quartz     | QUAR    | 373             |
| Corundum   | CORU    | 356             |
| Copper     | COPP    | 351             |
| Tin        | TIN     | 319             |
| Aluminum   | ALUM    | 296             |
| Ice        | ICE     | 100             |

> **Note:** Values are approximate and fluctuate with the in-game market. Acronyms are community-standard.

## 7.2 Practical Cutoff Guidelines

Before diving into the details, let's introduce the concept of an **A-tier focus**. This approach is based on the idea that you can achieve reliable and repeatable results by prioritizing A-tier ores, rather than endlessly hunting for the elusive S-tier "unicorn." Chasing only S-tier rocks might occasionally lead to a big win, but more often you'll come back empty-handed. Focusing on A-tier makes mining more fun and consistent, and when you do find an S-tier rock, it feels like a cherry on top of the cake. Using a single cutoff percentage based on A-tier content helps maximize profit and efficiency, filling your cargo with the most valuable and commonly available ores, while keeping your mining decisions simple and effective. The cutoff percentage and most crew policies in this guide are explained with this A-tier focus in mind, and the following policies (for S-tier, B-tier, or inerts) are adjustments to this default approach.

### Mission Start: Crew Communication
At the beginning of each mining mission, discuss with your crew or event organizer:
- What the cutoff percentage will be for A-tier ores
- Whether B-tier ores will be refined or discarded
- What the policy is for C-tier ores (normally considered basically inert, contributing fully to waste)
- Each turret operator's inert filtering capabilities

This ensures everyone is aligned on what rocks are worth mining and prevents wasted effort. Some groups may want to target B-tier ores as well as A-tier ores. In these cases, discuss whether B-tier ores should contribute to the cutoff (e.g., at a reduced rate such as one third of their initial percentage).

Because this method uses a single cutoff value and an A-tier focus, the group can easily adjust the material gathering threshold by simply communicating a new cutoff. For example, if the initial cutoff is 40% and the policy is that B-tier contributes to the A-tier and C-tier is garbage, but then a Caterpillar with Argo MOLE bags arrives to supply new ore bags, the pilot or event organizer can announce a new cutoff (e.g., lowering it to fill more bags quickly). The rest of the policy remains the same, and everyone can align their mining decisions accordingly. This flexibility makes it easy to adapt to changing goals or resources during a mining session.

### A-Tier Cutoff and Adjustment Policies

The baseline rule is that a rock should contain at least **40% A-tier mineral** to be considered worth mining. This is a starting point, not a hard maximum—higher percentages can be great, but setting the cutoff too high may mean you leave too many good rocks behind and end up with empty bags. Ultimately, you're optimizing time versus money: if high-percentage rocks are rare, the pilot or crew may decide to lower the cutoff to fill bags faster and keep the operation moving. Adjust your cutoff as needed to balance efficiency and profit. The following policies adjust this cutoff:

#### S-Tier Bonus
If the rock contains any S-tier ore, **double its percentage value** and add it to any A-tier mineral present.

> **Example:** If a rock has 10% Riccite (S-tier), 20% Taranite (A-tier), and the rest is tin and inert materials, the calculation is: 10% × 2 (RICC) + 20% (TARA) = 40%. This meets the cutoff.

#### Inert Material Adjustment
Inert materials (e.g., Inert, Waste) reduce the overall value of the rock. When evaluating a rock, apply your extraction laser's inert bonus—typically, use a **0.6 multiplier for inerts** (see the [Base Setup](BaseSetup.md#52-inert-filtering--extraction-laser-bonus) for your setup specifics). This means you only count 60% of the reported proportion of inerts in your calculation, reflecting their lower impact on your profit compared to valuable minerals.

> **Example:** A rock with 33% Bexalite (A-tier) and 67% inert materials would be calculated as follows:
> - Adjusted Inert: 67% × 0.6 = 40%
> - Add 33% Bexalite + 40% Adjusted Inert = 73%
> - The proportion of Bexalite in the adjusted total: 33% / 73% ≈ 45%
> - So, your initial 33% Bexalite is effectively 45% of the valuable content, making it worth mining.

#### B-Tier Contribution
If your group decides to target B-tier ores in addition to A-tier, you may count B-tier ores toward the cutoff at a reduced rate.

> **Example:** If the cutoff for A-tier is 40%, but a rock has 30% A-tier and 30% B-tier, you can count one third of the B-tier percentage toward the cutoff: 30% (A) + (30% × 1/3) = 30% + 10% = 40%. This makes the rock meet the cutoff. Always clarify this policy with your crew before starting the mining session.

### Example Evaluation
Rock composition: 32% Taranite (A-tier), 20% Tin (B-tier), 48% Inert
- Adjusted Inert: 48% × 0.6 = 28.8%
- Effective valuable content: 32% (A) + 20% (B) + 28.8% (Adjusted Inert) = 80.8%
- The proportion of Taranite in the adjusted total: 32% / 80.8% ≈ 40%

Here, the initial A-tier is right at the 40% cutoff after inert adjustment, making this rock a borderline but valid candidate for mining with the base setup. This demonstrates how inert filtering can make a borderline rock more attractive for mining.

## 7.3 Other Considerations

- **Cargo Space:** Only mine rocks that maximize your profit per SCU. Avoid filling your hold with low-value C-tier or inert-heavy rocks.
- **Time vs. Value:** Sometimes, a slightly lower cutoff is acceptable if you are in a hurry or want to fill your hold quickly.
- **Market Fluctuations:** Ore prices can change. Adjust your cutoffs if the market shifts.

## 7.4 References

- [Regolith Rocks Ore Survey](https://regolith.rocks/survey/ores)
- [Star Citizen Mining Discords & Community Resources](ResourcesReferences.md)

---

**Summary:**
- Aim for 40%+ A-tier, adjust for inerts, and always check the rest of the rock’s content. Treat your cutoff as a dynamic target, and adapt your strategy as the market, your crew, and your goals change.
