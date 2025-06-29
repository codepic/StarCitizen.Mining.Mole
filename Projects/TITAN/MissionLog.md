[💬 Send feedback on this page](https://github.com/codepic/StarCitizen.Mining.Mole/issues/new?template=feedback.yml&title=Feedback+on+MissionLog.md&page=MissionLog.md)

# 1. Project TITAN: Tactical Integrated Terrain Analysis Network

## Table of Contents

- [1. Project TITAN: Tactical Integrated Terrain Analysis Network](#1-project-titan-tactical-integrated-terrain-analysis-network)
  - [Table of Contents](#table-of-contents)
- [Project TITAN Survey Route Summary](#project-titan-survey-route-summary)
- [1. Project TITAN: Tactical Integrated Terrain Analysis Network](#1-project-titan-tactical-integrated-terrain-analysis-network-1)
  - [1.1 Mission Overview and Strategic Rationale](#11-mission-overview-and-strategic-rationale)
  - [1.2 Adir Lunar Statistics](#12-adir-lunar-statistics)
  - [1.3 📐 Zone Definitions: Cap and Ring Surveys](#13--zone-definitions-cap-and-ring-surveys)
  - [1.4 Survey Objectives and Data Goals](#14-survey-objectives-and-data-goals)
  - [1.4 Tactical Methodology: Zoning, Anchoring, and Data Feedback](#14-tactical-methodology-zoning-anchoring-and-data-feedback)
    - [1.4.1 Modular Survey Zones and Logistics](#141-modular-survey-zones-and-logistics)
    - [1.4.2 Orbital Marker as Operational Nodes](#142-orbital-marker-as-operational-nodes)
    - [1.4.3 Empirical Data-Driven Expansion](#143-empirical-data-driven-expansion)
    - [1.4.4 From Resource Mapping to Infrastructure Planning](#144-from-resource-mapping-to-infrastructure-planning)
    - [1.4.5 Coordinated Multi-OM Operations](#145-coordinated-multi-om-operations)
  - [1.5 Why TITAN’s Approach Is Tactical](#15-why-titans-approach-is-tactical)
  - [1.6 System Integration: Linking Orbital, Surface, and Teamwork](#16-system-integration-linking-orbital-surface-and-teamwork)
    - [1.6.1 Orbital-Surface Coordination for Precision](#161-orbital-surface-coordination-for-precision)
    - [1.6.2 Standardized Mapping and Data Consistency](#162-standardized-mapping-and-data-consistency)
    - [1.6.3 Unified Tools and Logging Frameworks](#163-unified-tools-and-logging-frameworks)
    - [1.6.4 Organization-Wide Protocol Adoption](#164-organization-wide-protocol-adoption)
    - [1.6.5 Macro and Micro Data Synergy](#165-macro-and-micro-data-synergy)
  - [1.7 Why TITAN’s Integration Matters](#17-why-titans-integration-matters)
  - [1.8 Network Model: TITAN as a Lunar Mesh](#18-network-model-titan-as-a-lunar-mesh)
    - [1.8.1 Distributed Node Coverage and Grid Expansion](#181-distributed-node-coverage-and-grid-expansion)
    - [1.8.2 Repeatable Protocols for Scalable Operations](#182-repeatable-protocols-for-scalable-operations)
    - [1.8.3 Centralized Data, Decentralized Action](#183-centralized-data-decentralized-action)
    - [1.8.4 Team Interoperability and Data Integrity](#184-team-interoperability-and-data-integrity)
    - [1.8.5 Strategic Connectivity and Corridor Planning](#185-strategic-connectivity-and-corridor-planning)
  - [1.9 Why TITAN Is a True Network](#19-why-titan-is-a-true-network)
  - [1.10 Project Scope: Metrics and Totals](#110-project-scope-metrics-and-totals)
  - [1.11 Survey Coverage, Overlap, and Area Analysis](#111-survey-coverage-overlap-and-area-analysis)
  - [1.12 South Polar Survey Results: Yield, Value, and Density](#112-south-polar-survey-results-yield-value-and-density)
  - [1.13 OM-Wide Coverage and Value Projection](#113-om-wide-coverage-and-value-projection)
  - [2. 🤝 Contributing to Project TITAN](#2--contributing-to-project-titan)
    - [2.1 🔧 Step-by-Step Survey Contribution](#21--step-by-step-survey-contribution)
    - [2.2 📎 Survey Etiquette](#22--survey-etiquette)

---

# Project TITAN Survey Route Summary

- **Project TITAN** is a systematic, tactical approach to surveying and mining the lunar surface of Moon Adir, using a network of standardized survey zones centered on orbital markers (OMs) and poles.
- The survey is organized into concentric radial zones around each anchor point (OM or pole):
  - **Cap**: 0–30 km from the center (high-resolution, inner core)
  - **Ring 1**: 30–60 km (primary expansion)
  - Additional rings (Ring 2, Ring 3, etc.) expand coverage further out in 30 km increments.
- **Survey Route Execution:**
  1. The surveyor coordinates with the project leader to get the OM, radius, and starting coordinates.
  2. The survey origin is established by leaving a ship as a fixed marker directly under the OM or at the designated point.
  3. The mining vessel is deployed to this origin.
  4. The surveyor then flies outward from the origin to the required radial distance (e.g., 30 km for Cap, 60 km for Ring 1), typically toward the opposite pole.
  5. At the correct distance, the surveyor circumnavigates the origin in a clockwise direction, maintaining a constant radius (i.e., flying a perfect circle around the anchor point).
  6. While circling, the surveyor scans rock clusters within 15 km laterally of the route, only logging those within the defined band.
  7. Findings are recorded in a standardized format and submitted for integration into the project’s data network.

- The approach ensures:
  - Repeatability and consistency across all OMs and poles.
  - Modular, scalable expansion of surveyed areas.
  - Data comparability and integration into a larger lunar resource model.

**In essence:** Survey routes are precise, circular sweeps at fixed distances from anchor points, designed to create a mesh of non-overlapping, standardized data zones across the lunar surface. Each sweep strengthens the overall network and contributes to a comprehensive, tactical mapping of resources.

---

# 1. Project TITAN: Tactical Integrated Terrain Analysis Network

## 1.1 Mission Overview and Strategic Rationale

*In the shadowed depths and sunlit arcs of Moon Adir, a systematic cartographic and resource extraction initiative is set to reshape the way we see lunar exploitation. Project TITAN represents a bold step in lunar-scale surveying: a synchronized sweep of lunar terrain conducted around each orbital marker, beginning with polar Cap and Ring traversals.*

Leveraging empirical data from the South Pole sector—where initial expeditions yielded over **39,000 SCU** and **€53 million aUEC** from just two zones—**TITAN** aims to replicate and expand this success. Each orbital marker becomes an anchor point for dual-zone surface scans covering **~14,300 km²**. Together, the network forms a lattice of logistical outposts, geological intelligence, and mining frontiers.

---

## 1.2 Adir Lunar Statistics

| Statistic         | Value                |
|-------------------|---------------------|
| Radius (r)        | 431 km              |
| Diameter (d)      | 862 km              |
| Circumference (C) | 2,709.7 km          |
| Surface Area (A)  | 2,336,964 km²       |
| Volume (V)        | 335,636,964 km³     |

**Calculation Formulas:**
- **Diameter (d):** 2 × r = 2 × 431 = 862 km
- **Circumference (C):** 2 × π × r ≈ 2 × 3.1416 × 431 ≈ 2,709.7 km
- **Surface Area (A):** 4 × π × r² ≈ 4 × 3.1416 × (431)² ≈ 2,336,964 km²
- **Volume (V):** (4/3) × π × r³ ≈ (4/3) × 3.1416 × (431)³ ≈ 335,636,964 km³

---

## 1.3 📐 Zone Definitions: Cap and Ring Surveys

All TITAN survey zones are defined radially from a **fixed surface anchor point**—either a **Pole** or a **designated Orbital Marker (OM)**. Each zone corresponds to a specific **distance band** from that central point, measured in kilometers:

| Zone Name | Distance from Center | Survey Radius Band | Description                                   |
|-----------|----------------------|---------------------|-----------------------------------------------|
| Cap       | 0–30 km              | Inner core          | High-resolution scan closest to the anchor    |
| Ring 1    | 30–60 km             | First outer band    | Primary expansion zone around the Cap         |
| Ring 2    | 60–90 km             | Secondary band      | Broadening coverage—start of interzone reach |
| Ring 3+   | etc.                 | Concentric bands    | Further layers expanding lunar grid coverage |

> 🔍 **Clarification**: “30 km” refers to radial distance from the Cap's centerpoint (e.g. OM location), **not latitude or planetary coordinate arcs**.

This radial structure ensures:
- Repeatability across any OM or pole
- Modular, scalable expansion per phase
- Consistency in data analysis and yield comparisons

All zones, regardless of location, follow this **0–30–60 km segmentation logic**, allowing TITAN to become a seamless, planet-wide terrain intelligence protocol.

---

## 1.4 Survey Objectives and Data Goals

- Execute **Cap (0–30 km)** and **Ring 1 (30–60 km)** surveys around each primary orbital marker on Adir  
- Log and compare yield and value metrics across surveyed zones  
- Generate a lunar-scale resource density model  
- Identify optimal sites for future operations and infrastructure

---

## 1.4 Tactical Methodology: Zoning, Anchoring, and Data Feedback

Project TITAN isn't just exploration—it's **methodical lunar domination**. Here's what makes it truly tactical:

---

### 1.4.1 Modular Survey Zones and Logistics

TITAN divides Moon Adir into standardized, repeatable survey units—**Cap (0–30 km)** and **Ring 1 (30–60 km)**—around each orbital marker. This modular approach enables:

- Predictable logistics
- Efficient route planning
- Comparable metrics between regions

> 🧠 Tactical Advantage: Establishes a uniform operational framework adaptable to any lunar body.

---

### 1.4.2 Orbital Marker as Operational Nodes

Using orbital markers (OMs) as **fixed nodes** ensures global symmetry and coverage:

- Guarantees surface reach across every hemisphere
- Synchronizes operations with orbital logistics
- Reduces navigation ambiguity in low-visibility terrain

> 🛰️ Tactical Advantage: Turns orbital infrastructure into surface-level intelligence grid.

---

### 1.4.3 Empirical Data-Driven Expansion

TITAN builds its expansion plan on **empirical data** from the South Pole:

- ~€53M aUEC value from first two zones
- SCU/km² and Value/km² metrics drive efficiency
- Survey priorities shift to high-density targets

> 📈 Tactical Advantage: Feedback loops refine future zone selection with each pass.

---

### 1.4.4 From Resource Mapping to Infrastructure Planning

TITAN zones are precursors to **infrastructure nodes**:

- High-yield zones become candidates for refineries, outposts, or hubs
- Geological intelligence supports longer-term habitation or transit use

> 🏗️ Tactical Advantage: Converts resource mapping into lunar control strategy.

---

### 1.4.5 Coordinated Multi-OM Operations

A single MOLE becomes a **lunar survey unit**, contributing to a hex-grid-like network of extraction and navigation corridors.

- Enables parallel deployment across multiple OMs
- Supports org-level operations with centralized oversight
- Scales beyond Adir for future lunar campaigns

> 🧭 Tactical Advantage: From lunar pilot to interlunar protocol.

---

## 1.5 Why TITAN’s Approach Is Tactical

Project TITAN is tactical because it blends **operational discipline**, **predictive mapping**, and **strategic exploitation**—not just to find resources, but to **claim and shape a world**.

---

## 1.6 System Integration: Linking Orbital, Surface, and Teamwork

Project TITAN isn't a disconnected set of lunar expeditions—it's a fully integrated lunar system. Its strength lies in linking diverse components into one cohesive, operational network.

---

### 1.6.1 Orbital-Surface Coordination for Precision

- Each **orbital marker (OM)** acts as a command node for surface operations
- Surface coverage zones (Cap + Ring 1) are centered on these orbital anchors
- Results in high spatial coordination between orbital logistics and ground routes

> 📡 Integration Benefit: Orbital systems guide surface scans, enabling precision landfall and consistent route geometry.

---

### 1.6.2 Standardized Mapping and Data Consistency

- Every zone uses identical radial bands (0–30 km, 30–60 km)
- Uniform mapping procedures allow clean data overlay and zone comparison
- Resource yields, densities, and values follow the same analytical pipeline

> 🧮 Integration Benefit: All teams speak the same data language—no recalibration needed from pole to equator.

---

### 1.6.3 Unified Tools and Logging Frameworks

- Navigation (Murphy’s Tool), mapping (Copilot Tables), and mission logs are unified
- All zones use common templates for statistics, value metrics, and density calculations
- Visuals, logs, and projections update seamlessly across systems

> 🧩 Integration Benefit: Engineering, logistics, and analytics teams operate on shared frameworks.

---

### 1.6.4 Organization-Wide Protocol Adoption

- TITAN isn’t limited to one crew—it's a scalable protocol across the organization
- Members can adopt TITAN zones, update shared logs, and sync findings
- New OMs can be deployed in parallel without disrupting others

> 🤝 Integration Benefit: One unified mission, many mobile outposts—like a lunar mesh network of minds.

---

### 1.6.5 Macro and Micro Data Synergy

- TITAN sees both the **zoomed-out planet** and the **zoomed-in ore vein**
- Macro statistics (per OM) and micro data (per find) live side by side
- Facilitates decisions from navigation routes to base placement to finance

> 🧠 Integration Benefit: Every scan echoes throughout the network, informing the big picture.

---

## 1.7 Why TITAN’s Integration Matters

Project TITAN is integrated because it doesn't treat mining as a series of isolated trips. It connects orbital infrastructure, standardized tools, synchronized methods, and shared organizational vision—into a **planet-spanning strategic web**.

---

## 1.8 Network Model: TITAN as a Lunar Mesh

Project TITAN is more than a mining campaign—it's an **interconnected, lunar framework** designed to function like a mesh of coordinated nodes. Here's what qualifies it as a true network:

---

### 1.8.1 Distributed Node Coverage and Grid Expansion

- Every **orbital marker (OM)** becomes a localized node in TITAN’s expanding grid  
- Each node conducts consistent survey routines (Cap + Ring 1)  
- The result: a **geospatial constellation** of exploration zones forming a surface-wide web

> 🔗 Network Quality: Multiple independent zones feeding into a unified spatial model

---

### 1.8.2 Repeatable Protocols for Scalable Operations

- Identical zone sizes and metrics across all markers  
- Each ring logs consistent data types: yield, value, density  
- Enables **plug-and-play scalability** across the lunar surface

> 📐 Network Quality: Each unit is modular yet interoperable—just like nodes in a digital network

---

### 1.8.3 Centralized Data, Decentralized Action

- Every survey feeds into a central mission log  
- Tables, maps, and values are recorded in universal formats (Markdown, CSV, GeoJSON if needed)  
- Data comparisons and statistical models span across all OMs

> 📊 Network Quality: Centralized data that reflects decentralized operations

---

### 1.8.4 Team Interoperability and Data Integrity

- Multiple survey teams (or org members) can operate at different OMs simultaneously  
- Common procedures ensure findings integrate smoothly  
- Expansion doesn’t fragment data integrity—it **scales it**

> 🤝 Network Quality: Human teams mirror the structure of a decentralized system

---

### 1.8.5 Strategic Connectivity and Corridor Planning

- Cumulative findings guide high-level resource planning  
- Surveyed areas form **contiguous corridors** for travel, mining, or infrastructure  
- The “network effect” increases with each additional zone added

> 🧭 Network Quality: TITAN doesn’t just explore—it connects what it surveys

---

## 1.9 Why TITAN Is a True Network

TITAN is a network because it turns isolated surface scans into an integrated, collaborative lunar lattice. Every orbital marker is a node. Every ring is a spoke. And together, they compose **a lunar-scale intelligence grid**.

---

## 1.10 Project Scope: Metrics and Totals

| Metric                | Estimated Total      |
|-----------------------|----------------------|
| Orbital Zones         | 6 (incl. both poles) |
| Area Surveyed         | ~85,758 km²          |
| Total Yield           | ~236,472 SCU         |
| Total Value           | ~€318 million aUEC   |

**Calculation Formulas:**
- **Area Surveyed:** Sum of all OM region areas covered (see OM-Wide Coverage table).
- **Total Yield:** Sum of estimated yields from all OM regions.
- **Total Value:** Sum of estimated values from all OM regions.

---

## 1.11 Survey Coverage, Overlap, and Area Analysis

_Assumptions:_
- Total surface area of Adir ≈ **37,930,000 km²**
- Each phase represents one OM region expanding through concentric rings
- Overlap increases with ring size due to adjacent OM convergence
- Cumulative coverage subtracts estimated overlap to reflect **unique area** surveyed

| Phase    | Ring Zone (km)   | Zone Area (km²) | Est. Overlap (km²) | Net Area Added (km²) | Cumulative Area (km²) | Area Remaining (km²) | % Remaining |
|----------|------------------|------------------|---------------------|------------------------|------------------------|------------------------|-------------|
| Phase 1  | Cap (0–30)       | ~5,763           | 0                   | ~5,763                 | ~5,763                 | ~37,924,237            | ~99.98%     |
| Phase 2  | Ring 1 (30–60)   | ~8,530           | 0                   | ~8,530                 | ~14,293                | ~37,915,707            | ~99.96%     |
| Phase 3  | Ring 2 (60–90)   | ~10,980          | ~500                | ~10,480                | ~24,773                | ~37,905,227            | ~99.93%     |
| Phase 4  | Ring 3 (90–120)  | ~12,950          | ~1,800              | ~11,150                | ~35,923                | ~37,894,077            | ~99.91%     |
| Phase 5  | Ring 4 (120–150) | ~14,370          | ~3,300              | ~11,070                | ~46,993                | ~37,883,007            | ~99.88%     |
| Phase 6  | Ring 5 (150–180) | ~15,240          | ~5,100              | ~10,140                | ~57,133                | ~37,872,867            | ~99.85%     |

**Calculation Formulas:**
- **Zone Area (km²):** π × (outer radius² − inner radius²) for each ring (radii in km).
- **Est. Overlap (km²):** Estimated area of overlap with adjacent OM regions (empirical or geometric estimate).
- **Net Area Added (km²):** Zone Area − Est. Overlap.
- **Cumulative Area (km²):** Sum of Net Area Added for all phases up to current.
- **Area Remaining (km²):** Total surface area of Adir − Cumulative Area.
- **% Remaining:** (Area Remaining ÷ Total surface area of Adir) × 100.

---

## 1.12 South Polar Survey Results: Yield, Value, and Density

| Zone        | Distance from Pole (km) | Route Length (km) | Area Covered (km²) | Finds | Total Yield (SCU) | Total Value (aUEC) | SCU/km² | Value/km² (aUEC) | Explored   | Time Required (hrs) |
|-------------|--------------------------|--------------------|---------------------|-------|--------------------|---------------------|---------|------------------|-------------|---------------------|
| Cap         | 0–30                     | ~188.2             | ~5,763              | 15    | ~7,334             | ~€11.3M             | ~1.27   | ~€1,961          | 2025-06-26  | 3.5                |
| Ring 1      | 30–60                    | ~282.0             | ~8,530              | 49    | ~32,078            | ~€41.7M             | ~3.76   | ~€4,891          | 2025-06-27  | 7                   |
| Ring 2      | 60–90                    | ~376.0             | ~10,980             | —     | —                  | —                   | —       | —                | —           | ~9.3                |
| Ring 3      | 90–120                   | ~470.4             | ~12,950             | —     | —                  | —                   | —       | —                | —           | ~11.7               |
| Ring 4      | 120–150                  | ~563.5             | ~14,370             | —     | —                  | —                   | —       | —                | —           | ~14.0               |
| Ring 5      | 150–180                  | ~656.0             | ~15,240             | —     | —                  | —                   | —       | —                | —           | ~16.3               |
| Equator     | 180 (hemisphere mark)    | ~682.7             | —                   | —     | —                  | —                   | —       | —                | —           | ~16.9               |

**Calculation Formulas:**
- **Area Covered (km²):** π × (outer radius² − inner radius²) for each ring (radii in km).
- **SCU/km²:** Total Yield ÷ Area Covered.
- **Value/km² (aUEC):** Total Value ÷ Area Covered.
- **Route Length (km):** Circumference of the ring at average radius (2 × π × average radius).

---

## 1.13 OM-Wide Coverage and Value Projection

| OM Region      | Area Covered (km²) | Est. Total Yield (SCU) | Est. Value (aUEC) |
|----------------|---------------------|--------------------------|--------------------|
| OM1 (Pole)     | ~14,293             | ~39,412                  | ~€53M              |
| OM2 (Equator N)| ~14,293             | ~39,412                  | ~€53M              |
| OM3 (Equator S)| ~14,293             | ~39,412                  | ~€53M              |
| OM4 (Equator E)| ~14,293             | ~39,412                  | ~€53M              |
| OM5 (Equator W)| ~14,293             | ~39,412                  | ~€53M              |
| OM6 (Opp. Pole)| ~14,293             | ~39,412                  | ~€53M              |
| **Total**      | **~85,758**         | **~236,472**             | **~€318M**         |

**Calculation Formulas:**
- **Area Covered (km²):** Sum of Cap and Ring 1 areas for each OM region.
- **Est. Total Yield (SCU):** Extrapolated from South Polar survey results (SCU/km² × Area Covered).
- **Est. Value (aUEC):** Extrapolated from South Polar survey results (Value/km² × Area Covered).
- **Total:** Sum across all OM regions.

---

## 2. 🤝 Contributing to Project TITAN

Individuals and org members can contribute to Project TITAN by executing standardized Cap and Ring surveys around designated surface anchor points. These anchor points may be at the Poles or directly beneath Orbital Markers (OMs). All contributions follow a strict methodology to ensure data quality, integration into Murphy’s Navigation Tool, and consistency across phases.

---

### 2.1 🔧 Step-by-Step Survey Contribution

1. **Coordinate with the Project Leader**
   - Confirm which sweep requires coverage and receive the following:
     - **Server region and instance name** (e.g. `EU:motivated_exploration`)
     - **Orbital Marker ID** (e.g. `OM-1`)
     - **Survey band radius** from the centerpoint (e.g. 30 km for Cap, 60 km for Ring 1)
     - **Starting coordinates** of the route  
       *(optional: ending coordinates for symmetrical surveys)*

2. **Establish the Survey Origin**
   - Fly a ship directly underneath the target Orbital Marker or coordinate
   - **Suicide to leave your ship behind as a fixed landmark**
   - This ship serves as the **centerpoint** for measuring survey distance

3. **Deploy Your Mining Vessel**
   - Spawn and fly a mining-capable ship (e.g. MOLE, ROC) to the origin
   - Use your navigation tools to validate that you are properly aligned

4. **Position Yourself at the Correct Distance**
   - From the origin, fly directly toward the *opposite hemisphere’s pole*:
     - From a **northern OM**, fly toward `OM-2` (southern pole)
     - From a **southern OM**, fly toward `OM-1` (northern pole)
   - Stop at the designated **radial distance** from your abandoned ship marker

5. **Begin Circumnavigation Sweep**
   - **Circle the origin in a clockwise direction**
   - Maintain constant distance (Cap: 30 km; Ring 1: 60 km) throughout
   - Adjust course using in-ship markers, altimeter, or nav tools

6. **Scan Rock Clusters Along Your Route**
   - Survey **only rock clusters within 15 km laterally** of your circular path
   - You may divert slightly to investigate, but stay within the allowed scan band

7. **Record Findings in Regolith**
   - Create a new session for your survey using this naming format:  
     `Adir OM-3/60km (EU:motivated_exploration)`
   - Follow this structure carefully:  
     `[planet name] OM-[#]/[radius] ([REGION]: server_name)`

8. **Submit Survey Session**
   - Once the sweep is complete, **share the Regolith session** with the mission leader
   - Include route confirmation, key yields, and any anomalies worth noting

---

### 2.2 📎 Survey Etiquette

- Stay within your assigned band to avoid data redundancy
- Do not survey overlapping rings unless explicitly assigned
- Only log findings that fall within the zone’s defined radius
- Name and share your sessions promptly to ensure coordinated logging

---

Every complete sweep strengthens the TITAN grid—one clean arc at a time. From your nav computer to the mission archive, you're not just flying laps—you’re building a planetary lattice.

