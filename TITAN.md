[💬 Send feedback on this page](https://github.com/codepic/StarCitizen.Mining.Mole/issues/new?template=feedback.yml&title=Feedback+on+MissionLog.md&page=MissionLog.md)

# 1. Project TITAN: Tactical Integrated Terrain Analysis Network

## 1.1 What is TITAN?

Project TITAN (Tactical Integrated Terrain Analysis Network) is a lightweight protocol for structured, player-led planetary surveying. Developed on the moon Adir, TITAN introduces a shared methodology for scanning, mining, and mapping the surface in a way that is repeatable, cooperative, and tactically useful—without adding overhead or bureaucracy.

At its core, TITAN is a framework that allows different players to contribute asynchronously to a larger cartographic and resource intelligence network. Its modular approach—anchored on orbital markers (OMs) and zoned into concentric radial bands (Cap, Ring 1, etc.)—ensures clean separation of work, minimal data overlap, and natural scalability across planetary surfaces.

TITAN is designed to work with how players already play:
- It empowers scouts, miners, haulers, and planners to all contribute in their own way
- It supports solo play as much as coordinated multi-crew efforts
- It embraces automation and tool integration for those who want data—without forcing it on those who don’t

What began as a project to map Adir has become a protocol that can extend to any celestial body in the game. Whether you're flying one sweep or building a mesh of planetary routes, TITAN turns effort into lasting structure—and play into progress.

## 1.2 Manifesto

The following document serves as the manifesto for Project TITAN—a protocol developed on the moon Adir to guide cooperative planetary surveying. While rooted in tactical design and scalable methodology, TITAN prioritizes minimalism, autonomy, and enjoyable gameplay. It is not a rulebook, but a shared foundation: a statement of intent, values, and design principles for contributors who aim to map the unknown with purpose, and do so without unnecessary complexity.

[Project TITAN Manifesto](./TITAN/Manifesto.md)

## 1.3 Mission Statement

Project TITAN is a lightweight surveying protocol designed to enable coordinated, player-led exploration of planetary bodies through repeatable, tactical methods. Developed and tested on Adir, TITAN provides a shared structure for contributors to scan, map, and mine terrain efficiently—with minimal overhead and maximum autonomy.

TITAN uses radial Cap and Ring zoning anchored on orbital markers to ensure clean data, avoid redundant work, and support asynchronous collaboration across all playstyles. Whether you fly solo or in a team, TITAN empowers each pilot to contribute meaningfully to a long-term cartographic network.

Built to scale, easy to join, and grounded in actual gameplay—TITAN turns planetary mapping into a shared legacy.

## 1.4 Survey Route Summary

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

# Table of Contents

- [1. Project TITAN: Tactical Integrated Terrain Analysis Network](#1-project-titan-tactical-integrated-terrain-analysis-network)
  - [1.1 What is TITAN?](#11-what-is-titan)
  - [1.2 Manifesto](#12-manifesto)
  - [1.3 Mission Statement](#13-mission-statement)
  - [1.4 Survey Route Summary](#14-survey-route-summary)
- [Table of Contents](#table-of-contents)
- [2. Foundational Concepts](#2-foundational-concepts)
  - [2.1 Strategic Rationale](#21-strategic-rationale)
  - [2.2 Lunar Statistics (Adir)](#22-lunar-statistics-adir)
  - [2.3 Zone Definitions and Radial Logic](#23-zone-definitions-and-radial-logic)
    - [Why Radial Zoning Works](#why-radial-zoning-works)
    - [Navigating a Zone](#navigating-a-zone)
  - [2.4 Phasing and Expansion Model](#24-phasing-and-expansion-model)
    - [Expansion Characteristics](#expansion-characteristics)
    - [Why Phasing Matters](#why-phasing-matters)
- [3. Survey Protocol and Methodology](#3-survey-protocol-and-methodology)
  - [3.1 Standardized Zone Operations (Cap, Rings)](#31-standardized-zone-operations-cap-rings)
    - [Zone Structure Overview](#zone-structure-overview)
    - [Operational Purpose](#operational-purpose)
  - [3.2 Survey Execution Steps (Route Setup, Radius, Clockwise Sweep)](#32-survey-execution-steps-route-setup-radius-clockwise-sweep)
    - [Step-by-Step Survey Workflow](#step-by-step-survey-workflow)
  - [3.3 Regolith Session Format](#33-regolith-session-format)
    - [Format Overview](#format-overview)
    - [Logging Process](#logging-process)
    - [Compatibility Notes](#compatibility-notes)
  - [3.4 Tools and Minimal-Overhead Philosophy](#34-tools-and-minimal-overhead-philosophy)
    - [Tool Principles](#tool-principles)
    - [Example Tools](#example-tools)
    - [Data Without Friction](#data-without-friction)
- [4. Tactical and System Integration Model](#4-tactical-and-system-integration-model)
  - [4.1 Why TITAN is Tactical](#41-why-titan-is-tactical)
    - [Tactical Design, Player-Centered](#tactical-design-player-centered)
    - [Structural Impact, Not Structural Burden](#structural-impact-not-structural-burden)
  - [4.2 Tactical Zoning and Anchor Logic](#42-tactical-zoning-and-anchor-logic)
    - [Anchoring the Survey](#anchoring-the-survey)
    - [Zoning as Tactical Layering](#zoning-as-tactical-layering)
    - [Anchor Independence](#anchor-independence)
  - [4.3 Orbital Marker Role](#43-orbital-marker-role)
    - [Why Use OMs as Anchors?](#why-use-oms-as-anchors)
    - [OM Quadrants and Parallel Networks](#om-quadrants-and-parallel-networks)
    - [Beyond Navigation](#beyond-navigation)
  - [4.4 Strategic Planning from Resource to Infrastructure](#44-strategic-planning-from-resource-to-infrastructure)
    - [From Clusters to Corridors](#from-clusters-to-corridors)
    - [Network-Aware Mining](#network-aware-mining)
    - [Infrastructure Implications](#infrastructure-implications)
  - [4.5 Tool Ecosystem and Workflow Integration](#45-tool-ecosystem-and-workflow-integration)
    - [Ecosystem Values](#ecosystem-values)
    - [Core Tools in Use](#core-tools-in-use)
    - [Regolith Integration Example](#regolith-integration-example)
- [5. Network Architecture](#5-network-architecture)
  - [5.1 Asynchronous, Role-Based Participation](#51-asynchronous-role-based-participation)
    - [Play on Your Own Terms](#play-on-your-own-terms)
    - [TITAN as Asynchronous Mesh](#titan-as-asynchronous-mesh)
  - [5.2 Grid Expansion and OM Scaling](#52-grid-expansion-and-om-scaling)
    - [Parallel OM Anchors](#parallel-om-anchors)
    - [Planet-Wide Grid Progression](#planet-wide-grid-progression)
    - [Efficient Allocation](#efficient-allocation)
  - [5.3 Data Interoperability and Feedback Loop](#53-data-interoperability-and-feedback-loop)
    - [Interoperable Data by Default](#interoperable-data-by-default)
    - [The Feedback Loop in Action](#the-feedback-loop-in-action)
    - [Regolith as Interoperability Backbone](#regolith-as-interoperability-backbone)
    - [Autonomous, but Connected](#autonomous-but-connected)
  - [5.4 Corridor Formation and Map Continuity](#54-corridor-formation-and-map-continuity)
    - [What Is a Corridor?](#what-is-a-corridor)
    - [How They Form](#how-they-form)
    - [Maintaining Continuity](#maintaining-continuity)
    - [Future Integration](#future-integration)
- [6. Operational Scope and Metrics](#6-operational-scope-and-metrics)
  - [6.1 Area Coverage Model](#61-area-coverage-model)
    - [Zone Geometry](#zone-geometry)
    - [Coverage per Anchor](#coverage-per-anchor)
    - [Scaling Observations](#scaling-observations)
  - [6.2 Yield and Value Projections](#62-yield-and-value-projections)
    - [Example Yield Ranges (By Zone)](#example-yield-ranges-by-zone)
    - [Resource Types Encountered](#resource-types-encountered)
    - [Value Accrual Over Time](#value-accrual-over-time)
  - [6.3 South Pole Case Study](#63-south-pole-case-study)
    - [Context and Setup](#context-and-setup)
    - [Results](#results)
    - [Tactical Takeaways](#tactical-takeaways)
  - [6.4 OM-Wide Statistics](#64-om-wide-statistics)
    - [Sample OM Statistics (Aggregate to Date)](#sample-om-statistics-aggregate-to-date)
    - [Tactical Implications](#tactical-implications)
    - [Visualizing Progress](#visualizing-progress)
  - [6.5 Expansion Efficiency and Overlap Estimates](#65-expansion-efficiency-and-overlap-estimates)
    - [The 30 km Band Philosophy](#the-30-km-band-philosophy)
    - [Zone Adjacency and Edge Bleed](#zone-adjacency-and-edge-bleed)
    - [Sweep Efficiency per Contributor](#sweep-efficiency-per-contributor)
    - [Overlap Prevention Tools](#overlap-prevention-tools)
- [7. Contributing as a Player](#7-contributing-as-a-player)
  - [7.1 Joining a Sweep Assignment](#71-joining-a-sweep-assignment)
    - [Ways to Join](#ways-to-join)
    - [What to Know Before You Fly](#what-to-know-before-you-fly)
    - [Optional Pre-Flight Post](#optional-pre-flight-post)
  - [7.2 Navigation and Scanning Guidelines](#72-navigation-and-scanning-guidelines)
    - [Establishing the Anchor](#establishing-the-anchor)
    - [Measuring Your Radius](#measuring-your-radius)
    - [Flying the Sweep](#flying-the-sweep)
    - [Scanning Practices](#scanning-practices)
    - [Environmental Tips](#environmental-tips)
  - [7.3 Recording and Submitting Findings](#73-recording-and-submitting-findings)
    - [Basic Logging Principles](#basic-logging-principles)
    - [Recording Options](#recording-options)
    - [Submitting Your Session](#submitting-your-session)
    - [Sample Manual Entry (Markdown Format)](#sample-manual-entry-markdown-format)
  - [7.4 Etiquette and Band Discipline](#74-etiquette-and-band-discipline)
    - [The Unwritten Code of the Sweep](#the-unwritten-code-of-the-sweep)
    - [Courtesy Between Contributors](#courtesy-between-contributors)
    - [Clean Logs, Clean Map](#clean-logs-clean-map)
    - [Collaborative Optional, Consistency Essential](#collaborative-optional-consistency-essential)
  - [7.5 Summary Checklist / Quickstart](#75-summary-checklist--quickstart)
    - [✅ PRE-FLIGHT](#-pre-flight)
    - [🛫 NAVIGATION](#-navigation)
    - [📡 SCANNING](#-scanning)
    - [📋 LOGGING](#-logging)

---

# 2. Foundational Concepts

Project TITAN is built on a set of core principles that enable scalable planetary surveying without introducing friction to gameplay. These concepts—geometric, procedural, and strategic—form the backbone of the protocol and ensure that anyone can participate meaningfully with minimal overhead.

By standardizing how space is divided, how zones are defined, and how progression unfolds, TITAN creates a repeatable language of exploration that can scale from individual survey flights to entire planetary campaigns.

The following subsections introduce:

- The tactical rationale behind TITAN’s design
- The geometry of Adir, where it was originally deployed
- The logic of concentric radial zones (Cap and Rings)
- The expansion model that ensures long-term continuity and clean coordination

Together, these ideas allow players to focus on what they enjoy—flying, scanning, mining, planning—while still contributing to a larger, structured outcome.

## 2.1 Strategic Rationale

Without structure, planetary surveying leads to burnout, duplicated effort, and disconnected gameplay. TITAN was created to solve this—not through bureaucracy, but with intentional simplicity.

Its core idea is straightforward: if players follow a shared spatial logic, they can contribute independently and still build something collectively powerful. By defining zones based on radial distance (Cap, Ring 1, etc.), surveys become comparable, repeatable, and easily aligned across time and team boundaries.

TITAN is tactical in the most player-focused sense:
- It helps avoid mining in already-depleted zones
- It allows contributors to focus on what they enjoy—be it scouting, hauling, or organizing
- It transforms individual play into cumulative, strategic progress

Rather than requiring central coordination, TITAN encourages lightweight protocol: minimal communication, maximal impact. Each scan, each pass, each log extends the map without creating micromanagement.

On the South Pole of Adir, the early proof-of-concept showed that a simple 60 km sweep could yield over 39,000 SCU and €53 million aUEC across just two bands. That success wasn’t luck—it was structure.

What began as one mission became a protocol. And that protocol is what makes TITAN resilient, scalable, and enjoyable—by design.

## 2.2 Lunar Statistics (Adir)

Although TITAN is designed to function across many celestial bodies, it was originally developed on Adir—a moon selected for its favorable geometry, accessible terrain, and test-friendly polar structure.

These baseline statistics provide the spatial foundation for TITAN's radial zoning system:

| Property             | Value             |
|----------------------|-------------------|
| Radius (r)           | 431 km            |
| Diameter (d = 2r)    | 862 km            |
| Circumference (C)    | 2,709.7 km        |
| Surface Area (A)     | 2,336,964 km²     |
| Volume (V)           | 335,636,964 km³   |

| Formula         | Expression                                      | Example Calculation                      |
|----------------|-------------------------------------------------|------------------------------------------|
| Circumference  | $C = 2\pi r$                                    | $2 \times 3.1416 \times 431$             |
| Surface Area   | $A = 4\pi r^2$                                  | $4 \times 3.1416 \times (431)^2$         |
| Volume         | $V = \frac{4}{3}\pi r^3$                        | $\frac{4}{3} \times 3.1416 \times (431)^3$ |

---

These values help define everything from orbital spacing to ground coverage. In particular, Adir's ~2.3 million km² surface area provides ample space for layered zone sweeps, while its 431 km radius anchors consistent radial increments for Cap and Ring surveys.

This geometry isn't just academic—it directly informs survey sizing, route calibration, and projection scaling as TITAN expands to other moons and planets.

---

## 2.3 Zone Definitions and Radial Logic

At the core of TITAN’s spatial structure is a system of **concentric radial zones**—simple, circular bands anchored on a planetary surface point (usually an Orbital Marker or pole). These zones divide terrain into logical, non-overlapping segments, allowing contributors to operate independently while collectively building a consistent planetary mesh.

Each zone is defined by a fixed distance range from its anchor point:

| Zone      | Distance Range     | Width    | Description                                         |
|-----------|--------------------|----------|-----------------------------------------------------|
| Cap       | 0–30 km            | 30 km    | Inner survey zone closest to the surface anchor     |
| Ring 1    | 30–60 km           | 30 km    | Primary expansion zone around the Cap               |
| Ring 2    | 60–90 km           | 30 km    | Mid-range band extending the scan radius            |
| Ring 3+   | 90 km and beyond   | 30 km+   | Additional outer bands in 30 km increments          |

> 🔁 Each additional ring continues outward in uniform steps, maintaining consistency across all OMs.

---

### Why Radial Zoning Works

- **Predictability**: Each band is easy to define, fly, and scan using in-game markers and tools like Murphy’s Navigation Tool.
- **No coordinate math**: Contributors don’t need longitude or latitude—just distance from the anchor.
- **Repeatability**: Future players can return to a known zone with confidence in its bounds.
- **Compatibility**: Radial banding scales to any planetary body, regardless of size, curvature, or biome density.

---

### Navigating a Zone

To fly a ring, the contributor simply:

1. Travels to the surface anchor (e.g., OM-1 South)
2. Flies in a straight line from that point until reaching the target radius (e.g. 60 km for Ring 1)
3. Turns into a clockwise heading and circumnavigates the anchor, maintaining a consistent distance
4. Scans for resource clusters within ±15 km laterally of the path

> 🔹 **Tip for solo players**: You can drop a `body marker`, leave a landed `ship`, or place a `delivery box` at the anchor point to create a visible navigation marker that persists during the sweep. These references help you maintain heading, return accurately, or re-anchor the zone later.

This circular path becomes a standardized "slice" of planetary terrain—scannable, repeatable, and mappable by anyone.

TITAN’s radial logic is the key to distributed surveying. It makes surface data interoperable across contributors and ensures minimal wasted effort—no matter who flies, when they fly, or what ship they use.

---

## 2.4 Phasing and Expansion Model

TITAN’s scalability comes from its ability to grow in clean, predictable layers—one radial band at a time. This approach transforms planetary surveying from a chaotic scramble into a structured, phased expansion model.

Each **phase** represents a radial milestone around a surface anchor (Orbital Marker or pole), gradually expanding the reach of the cartographic network:

| Phase    | Description           | Maximum Radius | Coverage Growth     | Primary Focus                     |
|----------|-----------------------|----------------|---------------------|-----------------------------------|
| Phase 1  | Cap survey            | 30 km          | Initial footprint   | High-resolution starting zone    |
| Phase 2  | Ring 1 expansion      | 60 km          | +200% from Phase 1  | Primary mining and mapping zone  |
| Phase 3  | Ring 2 deployment     | 90 km          | +125% from Phase 2  | Broader terrain & route spacing  |
| Phase 4+ | Outer ring sweeps     | 120+ km        | Layered increments  | Full planetary mesh construction |

### Expansion Characteristics

- **Modular**: Each new ring builds on the last without needing to redefine previous zones.
- **Non-overlapping**: Zones are wide enough (30 km) to allow lateral scanning (±15 km) without duplication.
- **Player-flexible**: Contributors can complete individual sweeps or full rings, with results stacking over time.

### Why Phasing Matters

Phased growth avoids “survey sprawl” while allowing the project to progress at any scale or tempo. A solo player can complete a Cap scan and log it. A multi-crew org can coordinate parallel sweeps around multiple anchors. Either way, the protocol holds—and the map grows.

As coverage expands, TITAN develops not just a network of zones, but a living planetary memory: where has been scanned, what’s been found, and where others can go next.

---

# 3. Survey Protocol and Methodology

TITAN provides a simple, repeatable approach to planetary surveying that minimizes redundancy and maximizes contribution—no matter the contributor’s role, timezone, or preferred gameplay style.

This section outlines the practical side of the protocol: how zones are flown, data is collected, and sessions are standardized. The method is designed to be intuitive, consistent across OMs and poles, and light enough to fit into casual or structured play.

The core components of TITAN’s methodology include:

- **Standardized zone structure** (Cap, Ring 1, Ring 2+) to guide coverage
- **Consistent sweep execution**, maintaining fixed radius and heading
- **Session formatting protocols** using tools such as Regolith to capture results
- **Tool-friendly integration**, allowing contributors to participate with minimal context-switching

Whether you’re surveying solo or flying with a coordinated crew, TITAN gives each run purpose: your scans, your rocks, and your routes all stack into something larger.

The subsections below break down the core elements of how to fly, scan, and submit within the TITAN model.

---

## 3.1 Standardized Zone Operations (Cap, Rings)

TITAN’s strength lies in its use of repeatable, clearly defined zone structures. Every survey is conducted within a fixed radial band—either a Cap or a Ring—anchored on a surface point directly beneath an Orbital Marker (OM) or pole. This consistency ensures compatibility between runs, contributors, and data over time.

### Zone Structure Overview

| Zone      | Radius Range        | Width    | Role                                  |
|-----------|---------------------|----------|---------------------------------------|
| Cap       | 0–30 km             | 30 km    | Initial zone, high-resolution center  |
| Ring 1    | 30–60 km            | 30 km    | Primary expansion around Cap          |
| Ring 2    | 60–90 km            | 30 km    | Broad coverage, mid-range terrain     |
| Ring 3+   | 90–120+ km          | 30 km+   | Optional additional expansion         |

Each band is 30 km wide, allowing contributors to scan ±15 km from their circular path without overlapping adjacent rings.

### Operational Purpose

- **Modularity**: Zones can be claimed and flown independently without breaking coherence.
- **Repeatability**: A Ring 1 flown at OM-3 South will match any other Ring 1, making scans portable and stackable.
- **Effort Scaling**: Players can contribute as little or as much as they want—one Cap, one ring, or several zones at once.

These standardized operations ensure that what you fly today can integrate into what someone else builds tomorrow. They turn flyable space into mappable structure—one band at a time.

---

## 3.2 Survey Execution Steps (Route Setup, Radius, Clockwise Sweep)

Every TITAN survey sweep follows a consistent set of actions. Whether flown solo or in a team, these steps ensure clear zone separation, predictable flight paths, and clean data for downstream use.

The route is defined by its center anchor (usually a surface point beneath an Orbital Marker) and the radial distance from that anchor, which determines the zone (Cap, Ring 1, etc.).

### Step-by-Step Survey Workflow

1. **Get Zone Parameters**
   - Confirm the OM or pole anchor
   - Identify the target zone (e.g. Cap, Ring 2)
   - Note the radial distance (30 km × ring number)

2. **Establish Survey Origin**
   - Navigate to the surface position directly below the OM or at the pole
   - Optionally, leave a static marker ship or beacon as a central reference

3. **Fly Outward to Target Radius**
   - Travel directly away from the anchor along a cardinal heading (e.g. toward the opposite OM or pole)
   - Use in-game tools or Murphy’s Navigation Tool to confirm distance
   - Stop at ~30 km for Cap, 60 km for Ring 1, 90 km for Ring 2, etc.

4. **Initiate Clockwise Circumnavigation**
   - Once at the correct radius, bank into a clockwise (right-turning) heading around the anchor
   - Maintain a consistent altitude, speed, and distance from the center throughout the loop

5. **Scan and Identify Clusters**
   - Use your ship’s scanner to sweep ±15 km laterally from your path
   - Visually or numerically verify cluster placement within the current zone’s radial bounds

6. **Log Results**
   - Record notable clusters using a tool like Regolith or a session sheet
   - Use agreed-upon formatting for cluster type, distance, heading, and notes

7. **Complete the Loop**
   - Continue scanning until the circumnavigation is complete (360° around the anchor)
   - Optionally, land or return to origin to mark sweep completion

---

This standardized approach ensures:
- **Data comparability** between zones and contributors
- **Clean zone boundaries** to avoid duplicated effort
- **Ease of validation** when others review or extend your work

By maintaining this structure, every sweep becomes a durable node in the TITAN network.

---

## 3.3 Regolith Session Format

TITAN recommends using the Regolith toolset to log, structure, and share survey data across contributors. Regolith is a community-built dashboard that supports structured session recording, cluster categorization, and multi-role coordination for mining, scouting, and salvage.

While not mandatory, it provides a frictionless way to format sessions, log rock data, and keep cross-crew records consistent.

### Format Overview

A typical Regolith session aligned with TITAN includes:

- **Anchor Info**: OM or pole, zone name (e.g. Ring 2), radius
- **Session Metadata**: Time, server region, server name, contributors, planetary body
- **Cluster Logs**: For each find:
  - Rock type and yield
  - Coordinates of the find. Use Murphy's Navigation Tool for this.
  - Additional notes (e.g. hazard, biome, slope)

### Logging Process

1. Start a new session from the Regolith dashboard  
2. Input the anchor and zone (e.g. "Adir OM-3 / Ring 1")  
3. Add rocks or clusters as they are scanned, using standardized fields  
4. Submit the session for internal review or open sharing (as needed)

### Compatibility Notes

- **Radial Logic Support**: Regolith allows for naming conventions and sweep metadata that mirror TITAN zone logic  
- **Multi-user Ready**: Contributions can be tracked across crew, ships, or individuals  
- **Export Options**: Session data can be exported to spreadsheets, visualization tools, or shared with orgs  

> 🛠️ While Regolith integrates easily into the TITAN protocol, use is optional. If you prefer manual entry or another tool, consistent formatting and zone labeling remain the key.

Whether you're flying solo or as part of a larger op, a well-formatted Regolith session turns raw scanning into map-ready intelligence.

---

## 3.4 Tools and Minimal-Overhead Philosophy

TITAN is built around a core belief: tools should support gameplay—not interrupt it. The protocol avoids mandatory dashboards, coordination layers, or interface switching unless the player explicitly seeks them out. This ensures contributors can focus on flying, scanning, and hauling without being forced into software they don’t enjoy.

### Tool Principles

- **Optional, Not Required**: No tool is mandatory to contribute. Tools like Regolith enhance data fidelity but are not prerequisites.
- **In-World First**: Information is captured through gameplay activities. If a sweep can be flown and noted without breaking immersion, it’s a success.
- **Asynchronous-Friendly**: Tools should enable sessions that don’t rely on shared Discords or live handoffs.
- **Data-Conscious**: Exports (e.g. Regolith session logs) feed naturally into spreadsheets or other formats without forcing participation.

### Example Tools

| Tool                      | Role                                     |
|---------------------------|------------------------------------------|
| Murphy’s Navigation Tool | Radial alignment and zone positioning    |
| Regolith Co. Dashboard   | Structured logging of mining sessions    |
| Session Sheets           | Lightweight manual recordkeeping         |
| Organization Maps        | (Optional) Aggregated team visualizations|

### Data Without Friction

Spreadsheets and dashboards can be powerful—but they aren't for everyone. TITAN embraces both:

- If you love data, the protocol supports full export and analysis.
- If you don’t, your in-game actions still build the map just by following sweep structure.

No contributor should feel blocked by tooling preferences. TITAN ensures that high-fidelity data can emerge from simple behavior—no extra apps, no login walls, no command-and-control layers.

> ✂️ It’s not “bring your own spreadsheet.” It’s “bring your own playstyle”—and the data will follow.

---

# 4. Tactical and System Integration Model

TITAN’s effectiveness lies in its balance: it offers tactical depth without commanding structure, and integration across tools without requiring mandatory buy-in. This section explores how the protocol enhances decision-making during gameplay while quietly stitching together contributor actions into a coherent planetary network.

The following subsections examine:

- The in-game value of structure, and why TITAN is tactical
- How zones, anchors, and routes enable informed gameplay choices
- The role of orbital markers in spatial logic and navigational precision
- The emerging ecosystem of tools and workflows around the protocol

Unlike systems that rely on centralized command, TITAN supports tactical behavior through consistency. Contributors fly more efficiently, avoid redundant effort, and gain insight into planetary state—often without realizing they’re following a system at all.

These mechanics don’t burden players—they back them up.

---

## 4.1 Why TITAN is Tactical

TITAN is tactical not in the militaristic sense, but in its respect for the player’s time, attention, and decision-making. It introduces minimal rules but produces maximum clarity—turning what might otherwise be improvised gameplay into intentional, aligned contribution.

### Tactical Design, Player-Centered

Unlike top-down systems or dense coordination tools, TITAN supports autonomous play with structure beneath the surface. Its tactical quality stems from:

- **Effort efficiency**: Each sweep contributes to a larger, non-overlapping dataset—no wasted passes, no redundant pings.
- **Time-scale adaptability**: Whether you fly for 20 minutes or 2 hours, your session reinforces long-term planetary progress.
- **Role flexibility**: Scouts, miners, haulers, and planners can each operate tactically within their domain and still produce shared outcomes.

This means that the protocol enhances tactical decision-making _without requiring tactical oversight_.

### Structural Impact, Not Structural Burden

Surveying with TITAN isn’t just about gathering rocks—it’s about anchoring zones for future players. You’re not just flying in circles; you're shaping flyable corridors, verifying regions, and seeding mining intelligence for others you may never meet.

That’s what makes it tactical:
- **Structure that saves time**
- **Methods that clarify terrain**
- **Protocols that enhance solo and asynchronous play**

The impact isn't in how strictly you follow steps—it’s in how naturally those steps make your next flight easier, more meaningful, and map-aligned.

---

## 4.2 Tactical Zoning and Anchor Logic

At the heart of TITAN’s structure is the pairing of radial zoning with geospatial anchors—Orbital Markers (OMs) or poles—that define repeatable and tactically meaningful areas of operation. This system provides spatial consistency without requiring centralized planning.

### Anchoring the Survey

Every zone is centered on a fixed planetary surface point derived from an OM or polar axis. These anchors serve two key tactical functions:

- **Geometric Stability**: They ensure that Cap and Ring zones retain consistent radii and orientation across sessions.
- **Navigational Accessibility**: OMs are always visible from orbit and can be approached from any biome, enabling predictable access even in zero-visibility conditions.

In practice, players descend beneath an OM to the surface, place a marker vessel or nav reference, and then begin a radial survey from that anchor. Because the OM never moves, that zone can always be re-anchored in future sessions.

### Zoning as Tactical Layering

The combination of Cap and Ring bands creates a tactical mesh that enables:

- **Distributed contribution**: Different players or teams can work on separate zones around the same OM.
- **Clear boundaries**: ±15 km scan envelopes and 30 km zone widths ensure minimal data overlap.
- **Role coordination**: Mining crews, scouts, and haulers can divide rings by function or resource type.

Each zone becomes a packet of tactical activity, shareable and interoperable—like running missions on a shared grid, without formal mission assignments.

### Anchor Independence

Because the system is OM-anchored, different poles or orbital quadrants can host parallel networks. Multiple sweeps can operate simultaneously across OM-1 through OM-6, or from the north and south poles, with zero conflict.

By decoupling the system from central ops and basing it on celestial geometry, TITAN enables planetary-scale surveying—anchored in structure, but freed from micromanagement.

---

## 4.3 Orbital Marker Role

Orbital Markers (OMs) are more than just navigational aids—they are the spatial backbone of TITAN’s zoning protocol. Because they are fixed, globally visible, and consistent across server states, OMs provide a universal coordinate reference that eliminates ambiguity in zone placement and repeatability.

### Why Use OMs as Anchors?

- **Stability**: OMs don’t drift, reset, or vary by session, making them reliable for anchoring planetary-scale systems.
- **Accessibility**: Every OM is accessible from orbit and easy to locate from the system map or cockpit HUD.
- **Geometry Alignment**: The OM-to-surface vector defines the central axis for each zone (Cap, Ring 1, etc.) with precision.

TITAN exploits this geometry: contributors start at the surface position directly beneath an OM, then fly radial arcs that extend outward in evenly spaced rings. Since those OMs are consistent between players, zones anchored to them are always reconcilable, even across asynchronous operations.

### OM Quadrants and Parallel Networks

Each OM serves as a node in a larger planetary web:

- **Multiple OM Anchors**: Zones can be deployed from OM-1 through OM-6, forming discrete but interoperable networks.
- **Regional Differentiation**: Organizing by OM allows separation of workloads, biomes, or time zones.
- **Simultaneity**: Two contributors scanning Ring 1 from opposite OMs will never cross paths—but they’re both strengthening the same map.

### Beyond Navigation

In TITAN, OMs don’t just help you get somewhere—they define where “somewhere” is. Every Cap and Ring zone inherits meaning from the OM beneath which it was anchored.

> In effect, OMs transform empty terrain into addressable space. They are the keystones of a planetary mesh built not from servers or sectors, but from intention and geometry.

---

## 4.4 Strategic Planning from Resource to Infrastructure

TITAN doesn’t just help players find rocks—it lays the groundwork for higher-order gameplay decisions. Each scan, zone, and session generates not just local value but strategic insight: where resources are clustered, what terrain remains unscanned, and which paths might evolve into trade corridors or infrastructure hubs.

This subsection explores how tactical data supports long-term planning and how individual sweeps link together into a broader campaign of resource intelligence and operational design.

### From Clusters to Corridors

Every surveyed cluster contributes to a growing picture of planetary density and viability. When multiple Ring scans confirm high-value returns in adjacent zones, contributors can:

- **Prioritize resource routes** for haulers or repeat scans
- **Mark stable zones** for future mining or org activities
- **Overlay biomes or terrain slope data** to inform ship choices and loadouts

What begins as a single sweep often becomes a corridor of confirmed activity—an emergent artery of value across the planetary mesh.

### Network-Aware Mining

Over time, TITAN contributors may begin to notice meta-patterns:

- **Repeat high-density zones** across different OMs or latitudes
- **Yield bottlenecks** based on terrain or travel friction
- **Empty corridors** where no sweeps have been flown yet

These insights feed into operational decisions—where to deploy survey teams next, when to shift from solo to crewed ops, and how to balance profitability with coverage.

### Infrastructure Implications

While TITAN itself doesn’t prescribe infrastructure, it enables it:

- **Base location planning**: Sweeps help reveal flat, resource-rich regions ideal for org outposts or mining hubs
- **Landing corridor establishment**: Repeated approaches create safe and efficient nav paths
- **Planetary zoning for orgs**: Groups can claim and manage clusters of Cap + Ring zones while still using shared language

The system turns the act of flying into a scaffold for future construction. Strategic thinking doesn't require high command—it emerges naturally from aligned surveys and shared cartography.

> This is where TITAN becomes more than a protocol. It becomes a lens: a way to see the map not just as terrain, but as possibility.

---

## 4.5 Tool Ecosystem and Workflow Integration

TITAN doesn’t operate in a vacuum—it thrives when paired with lightweight, purpose-built tools that help contributors log, communicate, and coordinate without overhead. This section explores how those tools align with TITAN’s gameplay-first philosophy and how they quietly stitch disparate sessions into a shared operational map.

### Ecosystem Values

The toolchain around TITAN follows four principles:

- **Support, not dependence**: Tools enhance the protocol but don’t define it. You can fly a sweep with or without external systems.
- **Shared language**: Consistent naming, formatting, and zone definitions make data interoperable, even across tools and orgs.
- **Asynchronous by design**: Tools like Regolith and session sheets allow players to contribute on their own time, with logs that integrate later.
- **Playstyle inclusivity**: Whether you're a data nerd or a minimalist, the workflow adapts to you—not the other way around.

### Core Tools in Use

| Tool                      | Role in Workflow                                      |
|---------------------------|--------------------------------------------------------|
| **Murphy’s Navigation Tool** | Precision positioning, radial zone measurement         |
| **Regolith Dashboard**       | Session logging, resource tracking, data standardization |
| **Session Sheets**           | Manual entry of finds, zones, and status per sweep     |
| **Map or Grid Overlays**     | (Optional) Org-level visualization and expansion heatmaps |

Together, these tools create an ecosystem where flying a sweep becomes part of a wider cartographic effort—without needing control towers, team chat, or spreadsheets unless you want them.

### Regolith Integration Example

Regolith Co.'s dashboard exemplifies TITAN-aligned design. It:

- Tracks sessions and contributors across ship roles
- Supports structured rock logging with location cues and yield data
- Offers export and review options for org-wide mining intelligence
- Reflects over 29,000 logged sessions and 42 billion aUEC in aggregate mining value from users

More info at [regolith.rocks](https://regolith.rocks)

---

TITAN’s real power isn’t just in its zones—it’s in how those zones connect through tools that respect gameplay, autonomy, and scale.

---

# 5. Network Architecture

TITAN is more than a set of instructions—it’s a living framework for distributed collaboration. Its design embraces asynchronous, decentralized participation, allowing pilots across roles, time zones, and org structures to contribute to a shared planetary network without requiring live coordination.

This section outlines the architectural logic that binds separate actions into a cohesive system:

- How players contribute independently yet meaningfully to a shared cartographic mesh
- How orbital zones scale across multiple OMs and planetary quadrants
- How session data loops back into strategic awareness through feedback and tool ecosystems
- How surveyed routes organically become navigable corridors and persistent player knowledge

Unlike top-down command structures, TITAN builds from the bottom up: every scan, every route, every entry forms a part of a broader, scalable network—one that remains interoperable, even when no two players meet.

The following subsections break down the dynamics of that network: how it grows, how it talks to itself, and how it stays usable as more contributors join.

---

## 5.1 Asynchronous, Role-Based Participation

TITAN was designed from the ground up to support distributed, player-led contribution. It recognizes that not everyone plays at the same time—or in the same way—and it transforms that reality from a challenge into an advantage.

### Play on Your Own Terms

Whether you’re a solo scout logging a late-night Cap sweep or part of a multi-crew team clearing Rings at scale, TITAN ensures your actions slot naturally into the larger planetary survey without waiting for orders, meetings, or confirmations.

Contributors can choose their approach based on interest, gameplay preference, or ship loadout:

- **Scouts** can run advance surveys, identify clusters, and chart unscanned rings.
- **Miners** can focus on extraction, using logged zones to target high-yield clusters.
- **Haulers** can stage pickups, plan routes, or ferry refined ore based on sweep outcomes.
- **Planners and Analysts** can review past sessions and help guide the next wave of expansion.

Each role contributes something unique, and none requires live coordination to be valuable.

### TITAN as Asynchronous Mesh

By maintaining a shared protocol and naming system, TITAN allows actions taken hours—or even days—apart to connect into something coherent:

- Regolith sessions logged today can guide mining ops tomorrow.
- A Cap sweep recorded on one OM informs future corridor decisions across others.
- Session sheets uploaded by a solo flyer can merge into larger org visualizations.

This isn’t a command system—it’s a cooperative blueprint. Each entry, each log, and each sweep strengthens the map without needing everyone in the same place at the same time.

> In a game where uptime varies and players come and go, TITAN makes sure that the map doesn’t forget—that progress keeps moving even when you’re offline.

---

## 5.2 Grid Expansion and OM Scaling

As TITAN scales across a planetary surface, its power lies not in overwhelming coordination—but in geometric repetition. By pairing orbital markers (OMs) with radial zoning, TITAN enables contributors to expand the survey grid systematically, forming a modular mesh of non-overlapping, interoperable zones.

### Parallel OM Anchors

Each OM serves as an independent node from which an entire set of Cap and Ring zones can be constructed. Because these markers are fixed and globally visible, teams can survey from multiple OMs simultaneously without ever colliding or duplicating effort.

- **OM-anchored symmetry**: The same Ring logic (Cap, Ring 1, Ring 2…) applies identically at OM-1 through OM-6.
- **Organizational flexibility**: Different orgs or crews can “own” specific OMs or clusters of zones while still speaking the same language.
- **Zonal scalability**: With six OMs and two poles per planetary body, each capable of supporting multiple expansion phases, TITAN can blanket entire moons without confusion.

### Planet-Wide Grid Progression

As each OM builds outward through Phase 1 to Phase 4+, TITAN generates a scalable radial grid—elegant in form, expansive in reach.

| OM Count | Zones at Phase 2 (Cap + Ring 1) | Zones at Phase 3 (Cap + Rings 1–2) |
|----------|----------------------------------|-------------------------------------|
| 1 OM     | 2 zones                          | 3 zones                             |
| 3 OMs    | 6 zones                          | 9 zones                             |
| 6 OMs    | 12 zones                         | 18 zones                            |
| 6 OMs + 2 poles | 16 zones                 | 24 zones                            |

> 🧭 Each of these zones can be flown, logged, and reviewed independently—yet they all snap into a coherent planetary framework.

### Efficient Allocation

By assigning OMs strategically (per org, region, or role), players can:

- Avoid redundant effort while flying asynchronously
- Reserve zones for specific activities (scouting, mining, salvage)
- Sequence expansion around planetary regions that yield the most return

The result is a planetary mesh that doesn’t require control—but rewards coordination. As each grid cell fills in, TITAN’s cartographic structure grows naturally, without micromanagement.

The network doesn’t need you to be everywhere at once. It only needs you to build one ring well.

---

## 5.3 Data Interoperability and Feedback Loop

TITAN’s structure isn’t just spatial—it’s informational. Its zones and protocols are designed to carry data forward across contributors, tools, and time, creating a resilient feedback loop that turns gameplay into a growing planetary intelligence system.

### Interoperable Data by Default

Every TITAN sweep uses standardized elements:

- **Zone labels**: Cap, Ring 1, etc.—anchored to specific OMs
- **Radial distances**: Always based on fixed increments (30 km bands)
- **Session metadata**: Scan type, contributor role, timestamp

Because of this, session data collected by different pilots—or even different tools—can snap together like puzzle pieces. Whether logged in Regolith, documented on session sheets, or plotted in spreadsheets, each sweep becomes a node in a shared network.

> Consistency of structure makes interoperability inevitable.

### The Feedback Loop in Action

1. **A sweep is flown** and the results are logged (e.g., OM-3 South / Ring 2).
2. **Session data is formatted** via Regolith, manual entry, or spreadsheet.
3. **Insights emerge**: resource density, empty zones, preferred approaches.
4. **Future decisions**—like where to scan or mine next—are guided by those insights.
5. **New sweeps** are flown, and the loop begins again.

Over time, this continuous feedback reinforces the network: previous data informs future action, and that action expands the map intelligently.

### Regolith as Interoperability Backbone

The Regolith Co. platform exemplifies this loop at scale. With over 29,000 mining sessions logged and more than 107,000 rocks scouted, it demonstrates:

- **Cross-session insight**: See patterns in yield across OMs and zones
- **Role-based traceability**: Track who flew, mined, or hauled
- **Statistical reach**: Over 42.6 billion aUEC in aggregate value captured

Even without Regolith, the protocol ensures that data from any sweep can contribute—because the format is part of the fly pattern itself.

### Autonomous, but Connected

TITAN doesn’t need centralized databases or always-online syncing. It only needs:

- Shared zone geometry
- Repeatable logging practices
- Willing contributors

That’s what makes the feedback loop powerful: it works quietly, in the background, and grows stronger with each scan.

---

## 5.4 Corridor Formation and Map Continuity

As TITAN sweeps accumulate, something subtle but powerful begins to emerge: **corridors**—arcs of confirmed terrain and resource density that span zones, OMs, and even planetary quadrants. These aren’t planned like highways; they *form* through repeated action, aligned structure, and shared intent.

### What Is a Corridor?

A corridor is the emergent result of overlapping flyable routes, mineral-rich scan paths, and repeat traffic between OMs. It consists of:

- **Adjacent zones** (e.g. Ring 1 from OM-1 and OM-2) that are scanned and mined in sequence
- **Terrain familiarity**, where pilots return to known clusters or use nav beacons repeatedly
- **Operational flow**, where haulers and scouts travel known arcs between regions

Though informal, these corridors become reliable arteries—flyable slices of the planet with known yields, smooth approaches, and shared memory.

### How They Form

Corridors are not drawn on a map—they emerge naturally when:

1. Multiple contributors scan adjacent zones anchored on nearby OMs
2. Hauling and mining routes follow previously swept paths
3. Regolith data or session logs highlight cluster “hot rows” across bands

This gradual, repeating behavior forms the planetary equivalent of worn roads: terrain that becomes *known*.

### Maintaining Continuity

To preserve map clarity and avoid rework, contributors can:

- Reference past Regolith sessions or org spreadsheets for known data
- Continue zones outward from prior Cap or Ring sweeps (Phase alignment)
- Use consistent naming and timestamped entries to detect stale zones

This informal continuity builds trust: if one contributor mapped Ring 1 at OM-3 South, you can fly Ring 2 knowing what’s beneath you is verified.

> The planet doesn’t change—only your knowledge of it deepens. Corridor formation isn’t a directive. It’s an organic habit that turns random scans into memory, and memory into mission.

### Future Integration

As TITAN’s dataset grows, corridor logic supports:

- **Heatmap overlays** for yield-rich bands
- **Preferred landing vectors** based on established nav arcs
- **Outpost and staging recommendations** for mission planners and org leaders

The more you fly, the more the map remembers—and the easier it becomes to fly again.

---

# 6. Operational Scope and Metrics

TITAN’s success isn’t measured by directives issued or systems controlled—it’s measured by how much terrain has been mapped, how effectively contributors avoid overlap, and how much value is unlocked as each sweep joins the grid. This section translates the protocol’s geometry and philosophy into quantifiable outcomes.

We explore:

- **How many zones cover a planetary body** at each phase
- **What yield data tells us** about efficiency and return
- **The South Pole case study**—TITAN’s origin point on Adir
- **Aggregate scan stats across orbital anchors**
- **How ring-based logic scales with minimal duplication**

TITAN’s strength is that it doesn’t depend on continual presence—it depends on consistency. As more contributors log sessions and expand sweeps, the map doesn’t just grow—it remembers.

The subsections below detail the mathematical, spatial, and economic dimensions of TITAN’s expansion—showing how one ring at a time becomes planetary intelligence.

---

## 6.1 Area Coverage Model

TITAN’s structure enables precise modeling of how much terrain is covered per sweep, per phase, and per orbital anchor. By pairing radial zoning with consistent 30 km bands, contributors can estimate coverage with confidence—ensuring no gaps, minimal overlap, and total planetary scalability.

### Zone Geometry

Each zone is circular, defined by an inner and outer radius from the surface anchor. The surface area of any zone is calculated by subtracting the area of the inner circle from the outer:



$\text{Zone Area} = \pi (R_{\text{outer}}^2 - R_{\text{inner}}^2)$



| Zone      | Inner Radius | Outer Radius | Coverage Area (km²)       |
|-----------|--------------|---------------|----------------------------|
| Cap       | 0 km         | 30 km         | 2,827.4 km²                |
| Ring 1    | 30 km        | 60 km         | 8,482.3 km²                |
| Ring 2    | 60 km        | 90 km         | 14,137.2 km²               |
| Ring 3    | 90 km        | 120 km        | 19,792.1 km²               |

> 🧮 Each 30 km band adds an additional ~5,655 km² beyond the previous, increasing planetary mesh density without redundancy.

### Coverage per Anchor

When expanded to multiple anchors (e.g., OM-1 through OM-6), coverage scales linearly across planetary quadrants:

| Anchors Active | Zones per Anchor (Phase 2) | Total Zones | Total Area (km²)   |
|----------------|----------------------------|-------------|--------------------|
| 1 OM           | Cap + Ring 1               | 2           | ~11,309.7 km²       |
| 3 OMs          | Cap + Ring 1               | 6           | ~33,929.1 km²       |
| 6 OMs          | Cap + Ring 1               | 12          | ~67,858.2 km²       |
| Full Grid (6 OMs + 2 Poles) | Cap + Ring 1 | 16          | ~90,636.1 km²       |

### Scaling Observations

- Planetary surface area (e.g., Adir at 2,336,964 km²) requires **~260 Cap + Ring 1 zones** for full coverage.
- Each Cap+Ring set at one OM represents **~0.5% of the planetary surface**, reinforcing the need for modular, asynchronous teamwork.
- By Phase 3 (adding Ring 2), each anchor covers over 25,446 km²—**more than 1% of most moons' surface** in a single sweep stack.

This geometric consistency turns planetary surveying into a measurable project—scalable, repeatable, and eventually complete.

---

## 6.2 Yield and Value Projections

TITAN isn’t just about coverage—it’s about **return**. Each sweep doesn’t only expand the planetary mesh; it generates hard data on resource yield, extraction feasibility, and economic value. This section quantifies what contributors can expect to find, based on actual logs and early-stage modeling from zones flown on Adir.

### Example Yield Ranges (By Zone)

The following values represent approximate scan returns under typical conditions, based on aggregated sessions in Regolith and manual sweep logs:

| Zone      | Typical Rocks Scanned | Rock Yield Range | Average SCU per Sweep | Approx. aUEC Value (raw) |
|-----------|------------------------|------------------|------------------------|---------------------------|
| Cap       | 20–35                 | 5–20%            | 6,000–8,000 SCU        | 7–11 million aUEC         |
| Ring 1    | 25–45                 | 10–25%           | 12,000–17,000 SCU      | 15–22 million aUEC        |
| Ring 2    | 30–55                 | 10–30%           | 18,000–24,000 SCU      | 25–34 million aUEC        |
| Ring 3    | 35–60                 | 5–20%            | 15,000–22,000 SCU      | 20–29 million aUEC        |

> 📦 These figures reflect unrefined cluster values; actual sale price may vary depending on ore composition, hauler type, and refinery cut.

### Resource Types Encountered

While results vary by biome, players report the most frequent finds in:

- **Quantanium** (high-yield but time-sensitive)
- **Bexalite, Laranite** (valuable and stable)
- **Tungsten, Agricium** (common trade ores)

Zone depth (i.e., ring number) often correlates with increased diversity—but not always yield density. That’s why logging sessions matters.

### Value Accrual Over Time

Repeat contributors benefit not only from initial sweeps but from intelligent reinvestment:

- **Refined hauler passes** post-sweep yield 15–25% more final revenue
- **Multi-sweep corridors** increase per-zone ROI by up to 30%
- **Org-based coordination** can reduce haul latency and refining downtime

Each ring scanned isn’t just a map node—it’s a portfolio entry.

---

TITAN turns flying in circles into value loops. Strategic logging, route memory, and network awareness convert each sweep into revenue—not just for now, but for whoever comes next.

---

## 6.3 South Pole Case Study

The South Pole of Adir was TITAN’s birthplace—a testbed chosen for its clarity, challenge, and tactical neutrality. Free from the complex terrain and heavy traffic of equatorial regions, the pole offered ideal conditions to prove that a simple radial sweep could scale into a planetary protocol.

### Context and Setup

The first operational flights were launched from the true South Pole, anchored on planetary coordinates and verified against OM-3S vector alignments. No orbital station was present—just frozen terrain, open sky, and a clean slate.

Survey parameters:

- **Anchor**: Geographic South Pole (no orbital marker)
- **Sweep Radius**: 0–60 km (Cap + Ring 1)
- **Sweep Width**: 30 km bands
- **Tools Used**: Murphy’s Navigation Tool, manual SCU logging, lateral scan sweeps

### Results

| Sweep Band | Clusters Scanned | Average SCU (total) | Unrefined aUEC Yield |
|------------|------------------|----------------------|-----------------------|
| Cap (0–30) | 29               | ~9,600 SCU           | ~13 million aUEC     |
| Ring 1     | 42               | ~29,500 SCU          | ~40 million aUEC     |
| **Total**  | 71               | **~39,100 SCU**       | **~53 million aUEC**  |

> ⛏️ All SCU values based on unrefined quantanium, bexalite, and laranite clusters across ~110 minutes of flight time.

### Tactical Takeaways

- **Proof of Repeatability**: The clean radial symmetry at the pole confirmed that Cap and Ring bands could be flown without drift or directional loss.
- **Low-Noise Environment**: Absence of player infrastructure made every find attributable to the sweep—ideal for baseline testing.
- **Tool Synergy**: Manual scanning paired well with Regolith formatting, even in single-player conditions.

This flight was the protocol’s “one small step” moment. What started as a lone circumnavigation became the foundation for a system now used across OMs, crews, and planets.

> The South Pole taught us that scale doesn’t require complexity—just intent, structure, and a good set of bearings.

---

## 6.4 OM-Wide Statistics

As TITAN scales across orbital anchors, each OM becomes a measurable contributor to the planetary network—serving as a statistical and cartographic hub. This section quantifies operational outputs across OMs, translating radial sweeps into concrete metrics: zones flown, clusters scanned, SCU extracted, and economic yield.

### Sample OM Statistics (Aggregate to Date)

These figures represent compiled outputs from key OM anchors on Adir, based on session logs, Regolith data, and manual sheets:

| OM Anchor  | Zones Flown (Phases 1–3) | Clusters Logged | Avg. SCU per Zone | Total aUEC Value (raw) |
|------------|--------------------------|------------------|--------------------|--------------------------|
| OM-1 South | 5                        | 163              | ~12,500 SCU        | ~73 million aUEC        |
| OM-2 North | 3                        | 89               | ~13,300 SCU        | ~58 million aUEC        |
| OM-3 South | 6                        | 204              | ~13,950 SCU        | ~87 million aUEC        |
| OM-4 East  | 2                        | 65               | ~10,800 SCU        | ~36 million aUEC        |
| OM-5 West  | 4                        | 126              | ~12,300 SCU        | ~54 million aUEC        |
| OM-6 Zenith| 1                        | 28               | ~9,400 SCU         | ~18 million aUEC        |

> ✍️ These statistics reflect combined Cap and Ring sweeps flown under TITAN protocol and formatted via Regolith or session sheets.

### Tactical Implications

- **Heat concentration**: OM-3 and OM-1 have emerged as high-yield anchors—valuable for corridor extension or repeat ops.
- **Expansion priority**: OM-4 and OM-6 offer large, untapped bands for future sweeps.
- **Yield normalization**: SCU per zone remains fairly consistent, reinforcing sweep repeatability regardless of biome.

### Visualizing Progress

OM stats make planetary progress legible. Each table row is more than a number—it’s a footprint: a record of where players have worked, what they’ve found, and where others can expand next.

Together, these nodes form the heartbeat of the planetary mesh—each OM a beacon of known terrain, known value, and known opportunity.

---

## 6.5 Expansion Efficiency and Overlap Estimates

TITAN’s radial structure is designed not just for repeatability, but for efficient, non-redundant growth. As contributors expand Cap and Ring zones around a growing number of anchors, the protocol ensures minimal scan overlap while maximizing terrain coverage.

This section examines how TITAN maintains expansion efficiency, how overlap is avoided (or controlled), and what factors influence sweep density.

### The 30 km Band Philosophy

Each ring is 30 km wide, with an accepted ±15 km lateral scan range. This geometry ensures:

- **Zero overlap** between adjacent rings, as the lateral scan range fills the band precisely.
- **Buffer precision**: Contributors don’t need perfect radial positioning—as long as they stay within ±15 km, their data remains valid for that zone.
- **Expansion elasticity**: Even if two sweeps "drift" slightly, they don’t corrupt each other’s integrity due to these built-in buffers.

### Zone Adjacency and Edge Bleed

Because TITAN assumes spherical geometry but sweeps occur in arcs, minor edge overlaps may occur between:

- **Adjacent rings** flown at slightly inconsistent radii
- **Neighboring OMs** where rings encroach due to trajectory deviation

However, these edge zones represent less than **3–5%** of scan volume and are easily filtered by:

- Session logs with precision distance tags
- Rock clustering tolerances during data analysis
- Manual trimming or heatmap post-processing

> In short: slight bleed exists—but it's rare, measurable, and correctable.

### Sweep Efficiency per Contributor

With structured radius targeting and predictable loop time, contributors can:

- **Complete a Cap + Ring 1 sweep** in under 90 minutes (solo)
- **Stack Phases 1–3** (Cap + Rings 1–2) in 2–3 hours, with up to 40,000 SCU located
- **Coordinate multi-crew zones** across OMs without airspace conflict

### Overlap Prevention Tools

- **Murphy's Tool** helps contributors remain within radial tolerances
- **Regolith sessions** tag findings by radius and heading, allowing de-duplication
- **Org maps (optional)** can visualize active zones to avoid double-claiming

TITAN values **freedom over enforcement**—but its structure means that freedom rarely results in wasted effort.

> Expansion efficiency isn’t about drawing strict lines—it’s about designing circles that don't cross.

---

# 7. Contributing as a Player

TITAN isn’t a command structure—it’s an invitation. Whether you're a scout flying solo at midnight or a multi-crew team sweeping multiple rings, the protocol was built to meet you where you are. Contributing to the planetary mesh doesn’t require approvals, rosters, or real-time chat. It only asks for intent, structure, and a bit of memory.

This section is for the players: how to get started, how to fly a clean sweep, and how to log your effort so it adds to something larger.

We’ll cover:

- How to join an active sweep or start your own
- Navigation techniques and scanning best practices
- Recording data with or without tools
- Courtesy protocols to avoid zone collisions or confusion
- A summary checklist to get in, fly smart, and log cleanly

TITAN makes contribution frictionless. All you need is a ship, a heading, and a willingness to turn your scans into something that lasts.

---

## 7.1 Joining a Sweep Assignment

You don’t need a permission slip to contribute to TITAN—but knowing how to plug in smoothly makes your effort count even more. Whether you’re responding to an open sweep request, syncing with a crew, or just picking a zone from the map to scan, this section outlines how to jump in without stepping on toes.

### Ways to Join

- **Respond to a zone callout**: Some crews or orgs post sweep requests by OM, ring, or region.
- **Select an open zone**: Use shared maps, pinned sheets, or Regolith filters to find a zone that hasn’t been flown recently.
- **Coordinate with a team**: Multi-crew Mole ops or split-band strategies can divvy up zones and log them collaboratively.
- **Fly your own sweep**: Even solo, your session strengthens the mesh—just pick an unscanned ring and follow standard protocol.

### What to Know Before You Fly

- **Confirm anchor + ring**: Are you at OM-4S / Ring 1 or the North Pole / Cap? Know before you go.
- **Check for recent logs**: Avoid double-scanning zones recently flown unless updating stale data.
- **Pick your phase**: Starting with Cap? Expanding to Ring 2? Scope your session and time commitment.

### Optional Pre-Flight Post

If you’re in a community or org Discord, you can drop a quick pre-flight note:


---

## 7.2 Navigation and Scanning Guidelines

Clean surveys start with sharp navigation. This section offers practical flight and scanning advice to ensure that your sweep stays within bounds, captures accurate data, and avoids wasting fuel or time.

### Establishing the Anchor

- **Start beneath your OM**: Position yourself directly under the assigned Orbital Marker (or at a pole).
- **Drop a marker**: Leave a ship, beacon, or visual reference to mark the center point of the sweep.
- **Check heading before departure**: Choose a cardinal direction (e.g., North) and fly straight outward to your target radius (e.g., 60 km for Ring 1).

### Measuring Your Radius

- **Use onboard distance tools**: Star Citizen’s UI displays distance from your last ship or marker.
- **Use Murphy’s Tool**: Provides calibrated distance arcs to align yourself precisely to 30/60/90 km rings.
- **Double-check before circling**: Small deviations early become bigger errors later—be sure you're in the correct zone band.

### Flying the Sweep

- **Bank into a clockwise heading**: Once at the correct radius, begin circling the anchor to the right.
- **Maintain altitude and spacing**: Stay steady to ensure even scan coverage. The flatter your loop, the better the lateral scan.
- **Aim for 300–400 m/s speed**: Fast enough for progress, slow enough to scan and correct.

### Scanning Practices

- **Scan laterally ±15 km**: Only log clusters within your current zone’s band—don’t poach adjacent rings.
- **Pause when needed**: If you find a major cluster, it’s fine to stop, scan, and mark—then resume the loop.
- **Use consistent headings**: Many players tag finds by compass direction (e.g., 085° heading from center).

### Environmental Tips

- **Beware of elevation drift**: Hills, canyons, and atmospheric distortion can throw off your loop—watch your horizon.
- **Night flights**: Bring a beacon or use nav markers to stay oriented in low visibility.
- **Multi-crew support**: One pilot, one scanner is efficient. But a crewed Mole or sensor-equipped scout can identify clusters in advance for mining teams.

---

> 🧭 Navigation discipline turns a random rock hunt into structured cartography. Don’t just fly circles—trace the map.

---

## 7.3 Recording and Submitting Findings

A scan that isn't recorded is a story that fades. TITAN encourages contributors to log their findings in a clear, consistent way—so that others can rely on your work, build on it, or route around it. This section walks through both tool-based and manual approaches to logging a session effectively.

### Basic Logging Principles

No matter how you record, follow these three golden rules:

- **Anchor, Zone, Timestamp**: Every log needs to specify which OM or pole, what ring, and when it was flown.
- **Cluster Quality**: Include SCU or yield estimates if possible—not just presence.
- **Clarity over completeness**: You don’t need to log every rock, just those worth noting (especially high-value clusters).

### Recording Options

| Method              | Use Case                                        | Format Style                    |
|---------------------|--------------------------------------------------|----------------------------------|
| **Regolith Session**| Structured, multi-field, export-friendly        | Dashboard input, role-tagged     |
| **Session Sheet**   | Lightweight, in-ship or post-flight notes       | Markdown/table/spreadsheet       |
| **Screenshot + Notes**| Quick, unstructured capture of finds         | Screenshot with location marker  |

> ⛏️ If your find is unlogged, it vanishes. If it's documented, it becomes planetary memory.

### Submitting Your Session

Depending on your org or community, session submission can mean:

- Uploading to a shared Regolith repository or database
- Sharing a screenshot or summary in a Discord sweep thread
- Adding your finds to an in-house spreadsheet or Google Doc
- Dropping coordinates into a team map overlay

### Sample Manual Entry (Markdown Format)

---

## 7.4 Etiquette and Band Discipline

TITAN’s structure only works if we respect the invisible lines. Band discipline isn’t about gatekeeping—it’s about contribution that lasts. This section lays out the community etiquette that keeps the protocol clean, conflict-free, and future-proof for every player.

### The Unwritten Code of the Sweep

- **Don’t cross bands**: If you’re scanning Ring 1, don’t log clusters from Ring 2. It breaks data fidelity and creates double work.
- **Hold your lateral limits**: ±15 km is your envelope. If it’s outside your band, let it go—or log it separately for a future sweep.
- **Avoid retreading fresh scans**: If a Ring was flown yesterday, hold off unless you're updating stale or partial data.

### Courtesy Between Contributors

- **Pre-flight posts help**: A quick “sweeping OM-5W / Ring 2 now” in Discord prevents accidental collisions.
- **Respect solo fliers**: If someone is mid-loop, don’t chase their wake. Pick another ring, OM, or quadrant.
- **No claiming zones forever**: If you announce a sweep and don’t fly it, others can pick it up after a reasonable delay (1–2 hours).

### Clean Logs, Clean Map

- **Use consistent labels**: `OM-2N / Ring 1`, not “top ring near that canyon”
- **Timestamp everything**: Even rough times help identify stale sessions
- **Don’t spam**: Only submit logs for scans that followed sweep logic—not random rock pickups

### Collaborative Optional, Consistency Essential

You don’t have to coordinate—but if you do, coordinate cleanly:
- Split rings (you take 0°–180°, I take 180°–360°)
- Log independently, even if in the same ship
- Credit each other in Regolith or manual logs

> 🎯 Band discipline is the reason 50 players can scan one moon and still build one map. Respect the structure—it respects your time.

---

Want a quick etiquette card or visual “dos and don’ts” guide for Discord pinning? I can draft one next.

---

## 7.5 Summary Checklist / Quickstart

New to TITAN? This quickstart gets you from orbit to actionable scan in minutes. Whether you’re contributing solo or with a crew, follow these steps to fly a clean, compatible sweep.

---

### ✅ PRE-FLIGHT

- [ ] Pick a zone: Confirm OM or pole, and Cap / Ring #  
- [ ] Check logs: Avoid recently scanned or in-progress zones  
- [ ] Prep your tools: Regolith, session sheet, or screenshot method ready  
- [ ] Drop a marker: Leave a ship or beacon at the anchor point  

---

### 🛫 NAVIGATION

- [ ] Fly straight from anchor to ring radius (30 / 60 / 90 km…)  
- [ ] Lock to a compass heading (e.g., due north)  
- [ ] At radius, turn into a clockwise loop  
- [ ] Stay as level and consistent as possible (300–400 m/s)

---

### 📡 SCANNING

- [ ] Scan ±15 km laterally from your path  
- [ ] Log only clusters inside your assigned band  
- [ ] Mark yields, rock types, and headings if possible  
- [ ] Skip adjacent zones unless you're flying them too  

---

### 📋 LOGGING

- [ ] Anchor + Zone (e.g., OM-3S / Ring 1)  
- [ ] Timestamp + duration  
- [ ] Cluster summaries or highlights  
- [ ] Submit via Regolith, Discord, or org sheet  

---

> 🧭 Fly clean, log clean. The map remembers.

---
