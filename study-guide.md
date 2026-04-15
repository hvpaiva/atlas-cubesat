# Phase-by-Phase Study Guide

This document organizes progressive study materials for each ECSS phase of the Atlas project.
The premise: study what is needed *for the current phase*, not everything at once. Knowledge
accumulates phase by phase, and each section indicates what to study *before* starting work
on the corresponding phase.

The author is a software developer with ~10 years of backend experience, proficient in Rust,
with no background in aerospace engineering, embedded systems, or safety-critical systems.
Basic math.

> **Note on `ref/`:** Reference documents (PDFs, DOCX) are not included in the repository for
> copyright reasons. Download links are available in `ref/docs.txt`. Descriptions and detailed
> tables of contents are in `ref/index.md`. When this guide says "Already in `ref/`", it means
> the document is indexed and its download link is listed — you need to download it yourself.

---

## Conventions

| Symbol | Meaning |
|--------|---------|
| **[ESSENTIAL]** | Mandatory reading/study before starting the phase |
| **[RECOMMENDED]** | Deepens understanding; consult as needed |
| **[REFERENCE]** | Spot-consultation material during the phase |
| **[FREE]** | Available at no cost |
| **[~USD X]** | Approximate cost in US dollars |

---

## General Prerequisites (Study First)

These materials are the starting point. Study them *before* any specific phase.

### CubeSat Overview

| # | Material | Format | Cost | Notes |
|---|----------|--------|------|-------|
| P1 | **NASA CubeSat 101** | PDF, 86p | [FREE] | Start here. Covers the complete lifecycle of a CubeSat, from concept through operations. Accessible language, process-oriented. Already in `ref/`. |
| | | | | https://www.nasa.gov/wp-content/uploads/2017/03/nasa_csli_cubesat_101_508.pdf |
| P2 | **CubeSat Design Specification (CDS) Rev 14.1** | PDF, ~40p | [FREE] | The de facto standard for CubeSats. Defines physical, electrical and operational specifications for 1U through 12U. Mandatory reading to understand form factor constraints. Already in `ref/`. |
| | | | | https://www.cubesat.org/cubesatinfo |
| P3 | **A Guide to CubeSat Mission and Bus Design** (Univ. Hawaii) | Online textbook (OER) | [FREE] | Funded by NASA Artemis program. Covers all subsystems with hands-on labs and video lectures. 12 chapters including orbital mechanics, ADCS, communications, thermal and software. Nothing else free comes close for CubeSat beginners. |
| | | | | https://pressbooks-dev.oer.hawaii.edu/epet302/ |
| P4 | **KiboCUBE Academy** (UNOOSA/JAXA) | PDF lectures + video | [FREE] | Pre-recorded lectures covering each subsystem. No engineering prerequisite. Individual lectures by subsystem. |
| | | | | https://www.unoosa.org/oosa/en/ourwork/access2space4all/KiboCUBE_Academy_Webinars.html |
| P5 | **NASA S3VI Systems Engineering Video Series** | YouTube videos + PDFs | [FREE] | Two seasons (2023-2025) covering SE fundamentals, requirements, design, AIT, lifecycle reviews and MBSE. NASA presenters with real mission experience. |
| | | | | https://www.nasa.gov/smallsat-institute/systems-engineering-series/ |

### Minimum Math

These topics are needed throughout the entire project. Study order matters.

| # | Topic | Material | Format | Cost | Est. time |
|---|-------|----------|--------|------|-----------|
| M1 | **Visual linear algebra** | 3Blue1Brown — Essence of Linear Algebra | 16 videos | [FREE] | ~4h |
| | | Focus: vectors, linear transformations, matrices, determinants, eigenvalues/eigenvectors. Geometric intuition, not mechanical computation. | | | |
| | | https://www.3blue1brown.com/topics/linear-algebra | | | |
| M2 | **Interactive linear algebra** | Immersive Linear Algebra | Online book | [FREE] | Reference |
| | | Interactive 3D figures. Each chapter starts with a concrete example. | | | |
| | | http://immersivemath.com/ila/tableofcontents.html | | | |
| M3 | **Quaternions** | 3Blue1Brown + Ben Eater — Visualizing Quaternions | Interactive web | [FREE] | ~2h |
| | | Clearest visual explanation of quaternions and 3D rotation available. Essential for ADCS. | | | |
| | | https://eater.net/quaternions | | | |
| M4 | **PID control** | mbedded.ninja — PID Control | Web tutorial | [FREE] | ~3h |
| | | Oriented toward embedded systems. Covers P, I, D, anti-windup, filtered derivative. | | | |
| | | https://blog.mbedded.ninja/programming/general/pid-control/ | | | |
| M5 | **Control theory** | Brian Douglas — Control Systems Lectures | YouTube | [FREE] | ~10h selective |
| | | Brian Douglas is a GNC engineer with 20+ years on spacecraft (Boeing, Planetary Resources). 17 thematic series. Focus on: "All of Control Theory", "State Space Control", "Sensor Fusion". | | | |
| | | https://engineeringmedia.com/videos | | | |
| M6 | **Kalman Filter visual** | Bzarg — "How a Kalman Filter Works, in Pictures" | Web tutorial | [FREE] | ~2h |
| | | Visual Kalman filter tutorial that builds intuition before equations. Prerequisites: basic probability and matrices. | | | |
| | | https://www.bzarg.com/p/how-a-kalman-filter-works-in-pictures/ | | | |
| M7 | **Kalman Filter with examples** | kalmanfilter.net | Web tutorial | [FREE] | ~4h |
| | | Based on numerical examples. Goes from basics through Extended Kalman Filter (EKF). | | | |
| | | https://kalmanfilter.net/ | | | |
| M8 | **Linear algebra for programmers — Rotations** | linearalgebraforprogrammers.com — Rotations Series | Web tutorial | [FREE] | ~3h |
| | | Covers 2D rotations, 3D rotation matrices, quaternions, geometric algebra. | | | |
| | | https://www.linearalgebraforprogrammers.com/series/rotations/0_intro | | | |

**When to study each math topic:**
- M1-M2: Before Phase A (needed to understand budgets and coordinate systems)
- M3: Before Phase B (quaternions appear in ADCS specification)
- M4-M5: Before Phase C (needed to implement controllers)
- M6-M7: Before Phase C (needed to implement attitude estimators)
- M8: When implementing coordinate transformations (Phase C)

---

## Phase 0 — Mission Analysis / Needs Identification

**Objective**: Elaborate the mission statement, identify needs, expected performance and
safety goals.

**Deliverables**: MDD, Preliminary TS.

**What you need to know for this phase:**
- What a CubeSat is and what its constraints are
- Basic space mission concepts (orbit, payload, subsystems)
- How to write a mission document
- Systems engineering process at a high level
- What ECSS standards are and how they work

### Materials

| # | Material | Type | Cost | Why study |
|---|----------|------|------|-----------|
| 0.1 | **NASA CubeSat 101** [P1] | PDF | [FREE] | Lifecycle overview. For Phase 0: focus on chapters 1 (definition) and 2 (development process, especially concept development and feasibility reviews). |
| 0.2 | **CDS Rev 14.1** [P2] | PDF | [FREE] | Sections 1-2: understand the mechanical and electrical constraints of the form factor that bound the mission. |
| 0.3 | **NASA SE Handbook (SP-2016-6105 Rev2)** | PDF, ~350p | [FREE] | [ESSENTIAL] NASA's primary SE reference. For Phase 0: chapters 1-4 (lifecycle, SE engine, technical processes). |
| | | | | https://www.nasa.gov/wp-content/uploads/2018/09/nasa_systems_engineering_handbook_0.pdf |
| 0.4 | **ECSS-E-ST-10C Rev.1 — Annex B (MDD DRD)** | DOCX | [FREE] | [ESSENTIAL] Defines the mandatory structure of the MDD. Already in `ref/`. Read BEFORE writing the MDD. |
| 0.5 | **ECSS-E-ST-10-06C — Technical Requirements Specification** | PDF | [FREE] | [ESSENTIAL] Defines how to structure technical specifications. Already in `ref/`. Read BEFORE writing the Preliminary TS. |
| 0.6 | **ECSS Training Course (slides)** | PDF | [FREE] | [RECOMMENDED] Already in `ref/` as `ECSS-E-10-SE-Training-Course-2021.pdf`. Overview of ECSS systems engineering processes. |
| 0.7 | **Hawaii OER — Chapters 1-3** [P3] | Web | [FREE] | [ESSENTIAL] Introduction to the space environment, mission concepts and basic orbital mechanics. |
| 0.8 | **NASA State-of-the-Art Small Spacecraft Technology (2024)** | PDF, ~420p | [FREE] | [REFERENCE] Already in `ref/` as `soa-2024.pdf`. Catalogs current technology for every subsystem with specs and TRL. Use as reference for initial trade studies. |
| | | | | https://www.nasa.gov/smallsat-institute/sst-soa/ |
| 0.9 | **ECSS-M-ST-10C Rev.1 — Project Planning** | DOC | [FREE] | [REFERENCE] Defines project phases and review gates. Already in `ref/`. Section 4.4.3.2 (Phase 0). |
| 0.10 | **NASA CubeSat Lessons Learned (2022)** | PDF | [FREE] | [RECOMMENDED] Compilation of real lessons learned from CSLI missions. Valuable for avoiding common mistakes from the start. |
| | | | | https://www.nasa.gov/wp-content/uploads/2018/01/cubesat_information_and_lessons_learned-2022.pdf |

---

## Phase A — Feasibility

**Objective**: Assess technical and programmatic feasibility of system concepts. Propose
concepts for further elaboration in Phase B.

**Deliverables**: SEP, System Concept Report, Function Tree, Technology Plan, Risk Assessment, TS.

**What you need to know for this phase:**
- Systems engineering in greater depth (SE plan, function trees, product trees)
- Trade studies: how to systematically compare alternatives
- Concepts of each subsystem with enough depth to assess feasibility
- Basic orbital mechanics (enough to justify orbit selection)
- Link budget, power budget, mass budget concepts
- Rust feasibility for each subsystem
- Technical and programmatic risk

### Materials

| # | Material | Type | Cost | Why study |
|---|----------|------|------|-----------|
| A.1 | **Space Mission Engineering: The New SMAD** (Wertz et al.) | Book, 1033p | [~USD 130] | [ESSENTIAL] The standard reference for space mission engineering. For Phase A: Part I (Mission Analysis and Design), especially chapters on mission architecture, budgets (mass, power, link) and orbit selection. |
| | | | | https://astrobooks.com/spacemissionengineeringthenewsmadsme-smadwertzeverettpuschellavailablespring2011softcover.aspx |
| A.2 | **Hawaii OER — All chapters** [P3] | Web | [FREE] | [ESSENTIAL] Read all 12 chapters for an integrated view of all subsystems. For Phase A, the power budget, link budget, orbital mechanics and ADCS chapters are particularly critical. |
| A.3 | **KiboCUBE Academy — All lectures** [P4] | PDF + video | [FREE] | [ESSENTIAL] Complements the Hawaii OER with JAXA/UNOOSA perspective. Each subsystem covered individually. |
| | | | | ADCS: https://www.unoosa.org/documents/pdf/psa/access2space4all/KiboCUBE/AcademySeason2/On-demand_Pre-recorded_Lectures/KiboCUBE_Academy_2021_OPL14.pdf |
| | | | | Communications: https://www.unoosa.org/documents/pdf/psa/access2space4all/KiboCUBE/AcademySeason2/On-demand_Pre-recorded_Lectures/KiboCUBE_Academy_2021_OPL09.pdf |
| | | | | EPS: https://www.unoosa.org/documents/pdf/psa/access2space4all/KiboCUBE/AcademySeason2/On-demand_Pre-recorded_Lectures/KiboCUBE_Academy_2021_OPL08.pdf |
| | | | | Thermal: https://www.unoosa.org/documents/pdf/psa/access2space4all/KiboCUBE/AcademySeason2/On-demand_Pre-recorded_Lectures/KiboCUBE_Academy_2021_OPL13.pdf |
| | | | | Payload: https://www.unoosa.org/documents/pdf/psa/access2space4all/KiboCUBE/AcademySeason2/On-demand_Pre-recorded_Lectures/KiboCUBE_Academy_2022_OPL18.pdf |
| A.4 | **NASA SE Handbook — Chapters 5-6** [0.3] | PDF | [FREE] | [ESSENTIAL] Technical management and requirements management chapters. How to derive system requirements from mission needs. |
| A.5 | **ECSS-E-ST-10C Annexes D, E, H, L** | Standard | [FREE] | [ESSENTIAL] DRDs for: SEP (Annex D), Technology Plan (Annex E), Function Tree (Annex H), System Concept Report (Annex L). Read BEFORE writing each artifact. |
| | | | | https://ecss.nl/standards/downloads/ecss-cd-download/ |
| A.6 | **ESA IOD CubeSat Engineering Guidelines** | PDF | [FREE] | [ESSENTIAL] Shows how ESA tailors ECSS for IOD CubeSats, which matches the rigor level appropriate for Atlas. |
| | | | | https://www.esa.int/Enabling_Support/Space_Engineering_Technology/Technology_CubeSats/Engineering_Guidelines_for_ESA_IOD_CubeSat_Projects_released |
| | | | | ECSS tailoring for CubeSats: https://www.ntnu.no/wiki/download/attachments/112275035/IOD_CubeSat_ECSS_Eng_Tailoring_Iss1_Rev3.pdf |
| A.7 | **Orbital Mechanics for Engineering Students** (Howard Curtis) | Book, ~700p | [~USD 90] | [RECOMMENDED] "Teach-by-example" approach with computational algorithms. For Phase A: chapters on orbital elements, Sun-Synchronous Orbits (SSO) and basic propagation. Every concept comes with an algorithmic implementation — ideal for devs. |
| | | | | https://shop.elsevier.com/books/orbital-mechanics-for-engineering-students/curtis/978-0-12-824025-0 |
| A.8 | **Kerbal Space Program** | Game/simulator | [~USD 10-40] | [RECOMMENDED] Orbital physics simulator disguised as a game. Teaches delta-v, Hohmann transfers, stable orbits intuitively. Probably the most intuitive way to learn orbital mechanics. |
| | | | | Academic companion: https://sites.google.com/view/kspmath |
| A.9 | **NASA SoA 2024 — Relevant chapters** [0.8] | PDF | [FREE] | [REFERENCE] Ch. 3 (Power), Ch. 5 (GNC), Ch. 8 (Avionics), Ch. 9 (Communications), Ch. 13 (Deorbit). Use during trade studies to identify COTS components and TRL. |
| A.10 | **CelesTrak — Tutorials** | Web | [FREE] | [REFERENCE] T.S. Kelso's tutorial series on orbital coordinates, TLEs and SGP4 propagation. |
| | | | | Coordinates: https://celestrak.org/columns/v02n01/ |
| | | | | Propagation: https://www.celestrak.org/columns/v01n01/ |
| A.11 | **EPFL/edX — Space Mission Design and Operations** | MOOC | [FREE] | [RECOMMENDED] Mission design from concept to operations. Complements books well with practical exercises. Free to audit (videos + readings); certificate is paid (~USD 50-100). |
| | | | | https://www.edx.org/learn/space/ecole-polytechnique-federale-de-lausanne-space-mission-design-and-operations |
| A.12 | **Link budget tutorials** | Web | [FREE] | [ESSENTIAL] Needed to justify communication band selection in Phase A. |
| | | | | Hawaii OER: https://pressbooks-dev.oer.hawaii.edu/epet302/chapter/9-6-link-budget/ |
| | | | | Charan Langton: https://complextoreal.com/wp-content/uploads/2013/01/linkbud.pdf |
| A.13 | **Power budget tutorials** | Web | [FREE] | [ESSENTIAL] Needed to confirm power feasibility. |
| | | | | Hawaii OER: https://pressbooks-dev.oer.hawaii.edu/epet302/chapter/5-9-power-budget-and-profiling/ |
| | | | | BIRDS Project (real example): https://birds-project.com/open-source/pdf/Power-Budget-Analysis-for-1U-satellit20220514.pdf |

---

## Phase B — Preliminary Definition

**Objective**: Confirm technical solutions. Establish preliminary design definition.
Prepare next-level specifications.

**Deliverables**: TS, DDF, Product/Spec Trees, Budgets, Verification Plan, IRD, SSS, SRS, SVerP,
Disposal Plan.

**What you need to know for this phase:**
- Flight software architecture (patterns, existing frameworks)
- ECSS-E-ST-40C in depth (space software process)
- CCSDS / PUS (space communication protocols)
- ADCS concepts (enough to specify software requirements)
- Safety-critical software fundamentals
- How to write verifiable software requirements
- Embedded Rust: feasibility, tooling, constraints

### Materials — Process and Standards

| # | Material | Type | Cost | Why study |
|---|----------|------|------|-----------|
| B.1 | **ECSS-E-ST-40C Rev.1 — Software Engineering** | PDF, 253p | [FREE] | [ESSENTIAL] The central space software engineering standard. For Phase B: sections 4 (principles), 5.2 (system requirements), 5.3 (management), 5.4 (requirements and architecture). Already indexed in `ref/index.md`. |
| | | | | https://ecss.nl/standard/ecss-e-st-40c-software-general-requirements/ |
| B.2 | **ECSS-Q-ST-80C Rev.2 — Software Product Assurance** | PDF, 132p | [FREE] | [ESSENTIAL] Complements E-ST-40. For Phase B: Annex D (tailoring by criticality — category D for Atlas), ch. 6 (process assurance). Already indexed in `ref/index.md`. |
| B.3 | **ECSS-E-ST-40C Annexes B, C, D, I** | Standard | [FREE] | [ESSENTIAL] DRDs for: SSS (Annex B), IRD (Annex C), SRS (Annex D), SVerP (Annex I). Read BEFORE writing each artifact. |
| B.4 | **ECSS-M-ST-10-01C — Conduct of Reviews** | PDF | [FREE] | [RECOMMENDED] How to conduct the SRR and PDR reviews. Already in `ref/`. |

### Materials — Flight Software and Architecture

| # | Material | Type | Cost | Why study |
|---|----------|------|------|-----------|
| B.5 | **NASA cFS Training Document** | PDF (NASA TM) | [FREE] | [ESSENTIAL] Understand the architecture of NASA's most-used FSW framework: PSP + OSAL + cFE + apps. Publish-subscribe messaging model. Reference for Atlas architecture. |
| | | | | https://ntrs.nasa.gov/api/citations/20205011588/downloads/TM%2020205000691%20REV%201.pdf |
| | | | | Repository: https://github.com/nasa/cFS |
| B.6 | **F Prime (F') — Docs + Getting Started** | Web | [FREE] | [ESSENTIAL] Component-driven architecture used on Mars Helicopter Ingenuity. Compare patterns with cFS for architecture decisions. |
| | | | | https://fprime.jpl.nasa.gov/latest/docs/ |
| | | | | Getting started: https://fprime.jpl.nasa.gov/latest/docs/getting-started/ |
| B.7 | **sat-rs — Documentation** | Web | [FREE] | [ESSENTIAL] The only Rust FSW framework with real flight heritage (OPS-SAT/ESA). Native ECSS PUS C and CFDP support. Directly relevant to Atlas architecture decisions. |
| | | | | Docs: https://docs.rs/satrs/latest/satrs/ |
| | | | | GitHub: https://github.com/us-irs/sat-rs |
| B.8 | **"Bringing Rust to Safety-Critical Systems in Space"** (Seidel et al., 2024) | Paper | [FREE] | [ESSENTIAL] Overview of efforts to adapt Rust for space systems. C-to-Rust rewrite methodology. Discovery of 3 vulnerabilities in satellite communication protocol. |
| | | | | https://arxiv.org/abs/2405.18135 |
| B.9 | **Spacecraft Systems Engineering** (Fortescue, Swinerd, Stark) | Book, 4th ed. | [~USD 100] | [RECOMMENDED] European/ESA focus. Each chapter by a specialist. For Phase B: AOCS, communications, power, thermal chapters — for deriving software requirements from subsystem requirements. |
| | | | | ISBN: 978-0470750124 |

### Materials — Space Protocols

| # | Material | Type | Cost | Why study |
|---|----------|------|------|-----------|
| B.10 | **CCSDS — Overview of Space Communications Protocols (Green Book)** | PDF | [FREE] | [ESSENTIAL] Visual introduction with protocol stack diagrams. Covers commanding, telemetry, frame/packet formats. |
| | | | | https://ccsds.org/Pubs/130x0g4e1.pdf |
| B.11 | **CCSDS Space Packet Protocol (Blue Book)** | PDF | [FREE] | [ESSENTIAL] Normative specification of the space packets Atlas will use. |
| | | | | https://ccsds.org/Pubs/133x0b2e2.pdf |
| B.12 | **ECSS PUS (Packet Utilization Standard) — Introduction** | Web | [FREE] | [ESSENTIAL] Understand what PUS is and which services Atlas needs to implement. |
| | | | | Accessible intro: https://pusopen.com/ecss-pus |
| | | | | Standard: https://ecss.nl/standard/ecss-e-st-70-41c-space-engineering-telemetry-and-telecommand-packet-utilization-15-april-2016/ |
| B.13 | **CFDP — Part 1: Introduction (Green Book)** | PDF | [FREE] | [ESSENTIAL] Written explicitly for those unfamiliar with the protocol. Needed to specify the downlink subsystem. |
| | | | | Green Book: https://ccsds.org/Pubs/720x1g4.pdf |
| | | | | Implementers Guide: https://ccsds.org/Pubs/720x2g4.pdf |
| | | | | Blue Book: https://ccsds.org/Pubs/727x0b5e1.pdf |
| B.14 | **GSAW CCSDS Tutorial (2018)** | PDF | [FREE] | [RECOMMENDED] Complete visual tutorial of the entire CCSDS stack. |
| | | | | https://gsaw.org/wp-content/uploads/2018/03/2018tutorial_e.pdf |
| B.15 | **spacepackets (Rust crate)** | Code + docs | [FREE] | [REFERENCE] Rust implementation of CCSDS + ECSS PUS + CFDP. Supports `no_std`. |
| | | | | https://docs.rs/spacepackets |

### Materials — Safety-Critical and Embedded Rust

| # | Material | Type | Cost | Why study |
|---|----------|------|------|-----------|
| B.16 | **Engineering a Safer World** (Nancy Leveson) | Book/PDF, ~500p | [FREE] | [ESSENTIAL] STAMP/STPA framework for systems safety analysis. Reframes safety analysis: instead of probabilistic failure trees, analyze systemic constraints. Required reading before writing safety-critical software. |
| | | | | Direct PDF: http://sunnyday.mit.edu/safer-world.pdf |
| | | | | MIT Press Open Access: https://direct.mit.edu/books/oa-monograph/2908/Engineering-a-Safer-WorldSystems-Thinking-Applied |
| B.17 | **Safety-Critical Rust Coding Guidelines v0.1** | Web | [FREE] | [ESSENTIAL] The closest thing to "MISRA for Rust". Covers types, traits, ownership, concurrency, `unsafe` usage. |
| | | | | https://coding-guidelines.arewesafetycriticalyet.org/ |
| | | | | Repository: https://github.com/rustfoundation/safety-critical-rust-coding-guidelines |
| B.18 | **High Assurance Rust** | Online book | [FREE] | [ESSENTIAL] Safe Rust subset based on MISRA-C directives. Differential fuzzing, deductive verification, data structures for resource-constrained environments. Fills the gap between general Rust proficiency and safety-critical Rust. |
| | | | | https://highassurance.rs/ |
| B.19 | **The Embedded Rust Book** | Web | [FREE] | [ESSENTIAL] Covers `no_std`, HALs, embedded concurrency. Mandatory starting point for embedded Rust. Actively maintained by the Rust Embedded Working Group. |
| | | | | https://docs.rust-embedded.org/book/ |
| B.20 | **Discovery Book (micro:bit v2)** | Web | [FREE] | [RECOMMENDED] Hands-on course teaching real hardware interaction with Rust. Ideal for those with zero embedded experience. |
| | | | | https://docs.rust-embedded.org/discovery-mb2/ |
| B.21 | **DO-178C Overview** | Web | [FREE] | [REFERENCE] Understand the 5 Design Assurance Levels (DAL A-E). For context: ECSS-E-ST-40C is the European space equivalent. |
| | | | | https://www.rapitasystems.com/do178 |

---

## Phase C — Detailed Definition

**Objective**: Complete the detailed design definition. Begin implementation and unit testing.

**Deliverables**: SDD, ICD, DJF, Traceability Matrix, source code, unit tests, preliminary SUM.

**What you need to know for this phase:**
- Embedded Rust in depth (Embassy, `no_std`, HAL, drivers)
- RTOS concepts and alternatives (cooperative multitasking, async)
- ADCS algorithm implementation (B-dot, quaternion PD, EKF)
- CCSDS/PUS protocols in detail for implementation
- Basic signal processing (for communications)
- Memory management in embedded
- Property-based testing
- IGRF model, SGP4

### Materials — Advanced Embedded Rust

| # | Material | Type | Cost | Why study |
|---|----------|------|------|-----------|
| C.1 | **Embassy Framework — Book + Examples** | Web + code | [FREE] | [ESSENTIAL] The most-used async framework for embedded Rust. Tasks as compile-time state machines. No dynamic allocation. Understanding Embassy is understanding how async/await replaces RTOS in many scenarios. |
| | | | | https://embassy.dev/book/ |
| | | | | Repository: https://github.com/embassy-rs/embassy |
| C.2 | **"Writing an OS in Rust"** (Philipp Oppermann) | Web | [FREE] | [ESSENTIAL] Async/await from scratch, Futures, state machines, pinning. Builds deep understanding of how cooperative multitasking works internally. |
| | | | | https://os.phil-opp.com/ |
| C.3 | **Google Comprehensive Rust — Bare Metal Day** | Online course | [FREE] | [RECOMMENDED] Full day dedicated to bare-metal Rust. |
| | | | | https://google.github.io/comprehensive-rust/ |
| C.4 | **Ferrous Systems — Embedded Training Slides** | Slides | [FREE] | [RECOMMENDED] Professional embedded Rust training material, openly available. |
| | | | | https://rust-training.ferrous-systems.com/ |
| C.5 | **Hubris OS (Oxide Computer)** | Code + docs | [FREE] | [REFERENCE] Message-passing microkernel with memory protection, 100% Rust. Use as architecture reference for component isolation. |
| | | | | https://hubris.oxide.computer/ |
| | | | | Blog: https://oxide.computer/blog/hubris-and-humility |
| C.6 | **heapless crate** | Code + docs | [FREE] | [ESSENTIAL] Fixed-capacity collections, no dynamic allocation, deterministic execution time. Golden rule in safety-critical: avoid `malloc`/`free`. |
| | | | | https://docs.rs/heapless |
| C.7 | **FreeRTOS Fundamentals** | Web | [FREE] | [RECOMMENDED] RTOS concepts (scheduling, tasks, queues, semaphores) even if Atlas uses Embassy. Needed to understand FSW literature. |
| | | | | https://www.freertos.org/Documentation/01-FreeRTOS-quick-start/01-Beginners-guide/01-RTOS-fundamentals |

### Materials — Algorithms and Implementation

| # | Material | Type | Cost | Why study |
|---|----------|------|------|-----------|
| C.8 | **Fundamentals of Spacecraft Attitude Determination and Control** (Markley & Crassidis) | Book | [~USD 100] | [ESSENTIAL] The canonical ADCS textbook. For Phase C: chapters on quaternion kinematics, B-dot detumbling, PD control, estimators (EKF). Includes MATLAB code. |
| | | | | https://link.springer.com/book/10.1007/978-1-4939-0802-8 |
| C.9 | **B-Dot Detumbling — Tutorials** | Web | [FREE] | [ESSENTIAL] For implementing the detumbling mode. |
| | | | | BLUEsat UNSW: https://bluesat.com.au/detumbling-and-the-b-dot-algorithm/ |
| | | | | IIT Bombay Wiki: https://www.aero.iitb.ac.in/satelliteWiki/index.php/B_Dot_Law |
| | | | | Hawaii OER Lab: https://pressbooks-dev.oer.hawaii.edu/epet302/chapter/software-lab-detumbling-simulation-using-magetorquers-and-bdot-control/ |
| C.10 | **Quaternion Attitude Control** | PDF/Web | [FREE] | [ESSENTIAL] For implementing fine pointing with reaction wheels. |
| | | | | Breeden (U. Michigan): https://public.websites.umich.edu/~jbreeden/Quaternions.pdf |
| | | | | DTU Satellite Dynamics: https://backend.orbit.dtu.dk/ws/files/98594729/Satdyn_mb_2010f.pdf |
| C.11 | **PySDR: A Guide to SDR and DSP using Python** | Online book | [FREE] | [ESSENTIAL] 25 chapters covering frequency domain, digital modulation (BPSK, QPSK), filters, link budgets, channel coding. Impossible to translate to physical book because of the animations. For Phase C: chapters 1-6 + 13 (channel coding). |
| | | | | https://pysdr.org/ |
| C.12 | **CelesTrak + sgp4 crate** | Web + code | [FREE] | [ESSENTIAL] For implementing onboard orbit propagation. |
| | | | | sgp4 Rust (no_std): https://crates.io/crates/sgp4 |
| | | | | satkit: https://lib.rs/crates/satkit |
| | | | | CelesTrak tutorials: https://celestrak.org/columns/ |
| C.13 | **IGRF / Magnetic field** | Web | [FREE] | [ESSENTIAL] For implementing the magnetic field model (input for magnetorquers). |
| | | | | NOAA official: https://www.ncei.noaa.gov/products/international-geomagnetic-reference-field |
| C.14 | **Space radiation — NASA NEPP** | PDF | [FREE] | [ESSENTIAL] For implementing SEU mitigations (EDAC, TMR, watchdog) and understanding hardware limitations. |
| | | | | Rad Effects 101: https://nepp.nasa.gov/docuploads/392333B0-7A48-4A04-A3A72B0B1DD73343/Rad_Effects_101_WebEx.pdf |
| | | | | SmallSat specific: https://nepp.nasa.gov/docs/tasks/053-SmallSat-RHA/NEPP-CP-2023-Campola-SmallSat-LEARN-Forum-Presentation-Radiation-Effects-and-EEE-Parts-Selection-20230015879.pdf |
| C.15 | **PID in C for embedded** | Web | [FREE] | [REFERENCE] Implementation with filtered derivative, saturation, anti-windup. Port to Rust. |
| | | | | https://simonebertonilab.com/pid-controller-in-c/ |

### Materials — Testing

| # | Material | Type | Cost | Why study |
|---|----------|------|------|-----------|
| C.16 | **Proptest (Rust)** | Code + docs | [FREE] | [ESSENTIAL] Property-based testing. Composable strategies, automatic shrinking. Most used in Rust. Isolate `no_std` logic in crates tested on host. |
| | | | | https://github.com/proptest-rs/proptest |
| | | | | Tutorial: https://www.lpalmieri.com/posts/an-introduction-to-property-based-testing-in-rust/ |
| C.17 | **ECSS-E-ST-40C Annex U — Code Verification** | Standard | [FREE] | [ESSENTIAL] 14 recommended code verifications. New in Rev.1. Practical checklist for code review. |
| C.18 | **ECSS-E-ST-40C Annexes F, E** | Standard | [FREE] | [ESSENTIAL] DRDs for SDD (Annex F) and ICD (Annex E). Read BEFORE writing. |
| C.19 | **Ferrous Systems — Concurrency Patterns in Embedded Rust** | Blog | [FREE] | [RECOMMENDED] Practical patterns: interrupts, shared state, async in embedded. |
| | | | | https://ferrous-systems.com/blog/embedded-concurrency-patterns/ |

---

## Phase D — Qualification and Production

**Objective**: Complete qualification testing. Complete integration and interoperability testing.

**Deliverables**: Verification Control, Test Specs/Procedures/Reports, SIL/PIL/HIL results, SRelD, final SUM.

**What you need to know for this phase:**
- SIL, PIL, HIL testing in depth
- Orbital environment simulation
- Formal verification and validation
- Cross-compilation to target MCU
- Ground segment software (for interoperability testing)
- Simulation tools (42, Basilisk)

### Materials

| # | Material | Type | Cost | Why study |
|---|----------|------|------|-----------|
| D.1 | **NOS3 — NASA Operational Simulator for Small Satellites** | Software | [FREE] | [ESSENTIAL] Software-only testbed for SmallSats. Integrates orbital dynamics simulator (42), cFS and command/control system (COSMOS). Enables complete V&V without hardware. |
| | | | | Wiki: https://github.com/nasa/nos3/wiki/ |
| | | | | NASA Catalog: https://software.nasa.gov/software/GSC-17737-1 |
| | | | | Paper: https://arxiv.org/abs/1901.07583 |
| D.2 | **42 — NASA Attitude/Orbit Simulator** | Software | [FREE] | [ESSENTIAL] Attitude and orbit dynamics simulator. Input for ADCS SIL testing. |
| | | | | https://github.com/ericstoneking/42 |
| D.3 | **Basilisk — CU Boulder Simulation Framework** | Software | [FREE] | [REFERENCE] More complete simulation framework, but steeper learning curve. |
| | | | | https://github.com/AVSLab/basilisk |
| D.4 | **SIL vs HIL — Concepts** | Web | [FREE] | [ESSENTIAL] Understand the differences and when to use each test level. |
| | | | | OPAL-RT: https://www.opal-rt.com/blog/hardware-in-the-loop-vs-software-in-the-loop/ |
| | | | | Robotics KB: https://roboticsknowledgebase.com/wiki/system-design-development/In-Loop-Testing/ |
| D.5 | **MOVE-II CubeSat HIL Paper** | Paper | [FREE] | [RECOMMENDED] Real-world example of a CubeSat HIL setup, including architecture and lessons learned. |
| | | | | https://www.mdpi.com/2226-4310/6/12/130 |
| D.6 | **ECSS-E-ST-10-02C Rev.1 — Verification** | Standard | [FREE] | [ESSENTIAL] Verification standard. DRDs for Verification Control Document and Verification Report. |
| | | | | https://ecss.nl/standard/ecss-e-st-10-02c-rev-1-verification-1-february-2018/ |
| D.7 | **ECSS-E-ST-10-03C Rev.1 — Testing** | Standard | [FREE] | [ESSENTIAL] Testing standard. DRDs for Test Specification, Procedure and Report. |
| | | | | https://ecss.nl/standard/ecss-e-st-10-03c-rev-1-testing-31-may-2022/ |
| D.8 | **ECSS-E-ST-40C Annexes G, H** | Standard | [FREE] | [ESSENTIAL] DRDs for SRelD (Annex G) and SUM (Annex H). |
| D.9 | **Ground Segment — Yamcs** | Software | [FREE] | [ESSENTIAL] Open-source mission control framework (Java). Used by NASA and ESA. Needed for interoperability testing. |
| | | | | https://yamcs.org/ |
| | | | | CFDP support: https://docs.yamcs.org/yamcs-server-manual/services/instance/cfdp/ |
| D.10 | **SatNOGS** | Software + network | [FREE] | [RECOMMENDED] Global open-source ground station network. For understanding real ground segment. |
| | | | | https://satnogs.org/ |
| | | | | Getting started: https://wiki.satnogs.org/Get_Started |
| D.11 | **GNU Radio — Tutorials** | Software | [FREE] | [RECOMMENDED] SDR framework for signal processing. Used in real ground stations. |
| | | | | Tutorials: https://www.gnuradio.org/news/2022-02-03-new-tutorials/ |
| | | | | gr-satellites: https://gr-satellites.readthedocs.io/en/latest/overview.html |
| D.12 | **NASA Open MCT** | Software | [FREE] | [REFERENCE] Web-based mission data visualization framework. |
| | | | | https://nasa.github.io/openmct/ |
| D.13 | **embedded-test (probe-rs)** | Code | [FREE] | [REFERENCE] Test framework for Rust on real hardware. For PIL testing. |
| | | | | https://github.com/probe-rs/embedded-test |

---

## Phase E — Utilization (Operations)

**Objective**: Execute the mission. Commissioning and nominal operations.

**Deliverables**: Operations log, anomaly reports, commissioning results.

**What you need to know for this phase:**
- Ground station operation
- Tracking and pass prediction
- Telemetry monitoring
- Anomaly procedures
- Operational FDIR

### Materials

| # | Material | Type | Cost | Why study |
|---|----------|------|------|-----------|
| E.1 | **NASA SoA 2024 — Ch. 11 (Ground Data Systems)** [0.8] | PDF | [FREE] | [ESSENTIAL] Covers ground architecture, frequencies, link budget, GSaaS, mission ops software. Pages 303-375. |
| E.2 | **Pass prediction — sgp4 + CelesTrak** | Code | [FREE] | [ESSENTIAL] Implement pass prediction for ground station. |
| | | | | Python ref: https://pypi.org/project/passpredict/ |
| E.3 | **Yamcs + Open MCT** [D.9, D.12] | Software | [FREE] | [ESSENTIAL] Mission control tools for operations. |
| E.4 | **SatNOGS + gr-satellites** [D.10, D.11] | Software | [FREE] | [RECOMMENDED] For real ground station operation. |

---

## Phase F — Disposal

**Objective**: Implement the disposal plan.

**Deliverables**: Disposal report, Lessons learned.

### Materials

| # | Material | Type | Cost | Why study |
|---|----------|------|------|-----------|
| F.1 | **NASA SoA 2024 — Ch. 13 (Deorbit Systems)** [0.8] | PDF | [FREE] | [ESSENTIAL] State of the art in deorbit systems: drag sails, propulsion, tethers, regulations. |
| F.2 | **25-Year Rule + FCC 5-Year Rule** | Regulation | [FREE] | [ESSENTIAL] Understand debris regulations. The FCC reduced from 25 to 5 years in 2024. |
| F.3 | **NASA DAS (Debris Assessment Software)** | Software | [FREE] | [REFERENCE] NASA tool for orbital debris analysis. |
| | | | | https://orbitaldebris.jsc.nasa.gov/mitigation/das.html |

---

## Cross-Cutting Materials (All Phases)

These materials are relevant throughout the entire project.

### Reference books (buy when budget allows)

| # | Book | Cost | When to buy |
|---|------|------|-------------|
| T.1 | **Space Mission Engineering: The New SMAD** (Wertz et al., 2011) | ~USD 130 | Before Phase A. Primary reference for the entire project. |
| T.2 | **Orbital Mechanics for Engineering Students** (Curtis, 4th ed., 2019) | ~USD 90 | Before Phase A. Computational algorithms for orbital mechanics. |
| T.3 | **Spacecraft Systems Engineering** (Fortescue et al., 4th ed., 2011) | ~USD 100 | Before Phase B. Subsystems in depth, ESA perspective. |
| T.4 | **Fundamentals of Spacecraft Attitude Determination and Control** (Markley & Crassidis, 2014) | ~USD 100 | Before Phase C. Canonical ADCS textbook. |
| T.5 | **CubeSat Handbook** (Cappelletti et al., 2020) | ~USD 120 | When deeper CubeSat-specific detail is needed. First book exclusively about CubeSats. |
| T.6 | **The Safety Critical Systems Handbook** (David Smith, 4th ed., 2016) | ~USD 80 | Before Phase B. IEC 61508, SIL levels, functional safety. |
| | | | ISBN: 978-0-12-805121-4 |
| T.7 | **INCOSE Systems Engineering Handbook** (5th ed., 2023) | ~USD 100 | SE process reference. NASA handbook is more practical; INCOSE is more formal. |
| | **Total if buying all:** | **~USD 720** | |
| | **Recommended minimum (T.1 + T.4):** | **~USD 230** | |

### Online courses

| # | Course | Platform | Cost | When to take |
|---|--------|----------|------|--------------|
| T.8 | **Space Mission Design and Operations** | edX (EPFL) | [FREE] | Phase A. Free to audit; certificate is paid. |
| | | | | https://www.edx.org/learn/space/ecole-polytechnique-federale-de-lausanne-space-mission-design-and-operations |
| T.9 | **Spacecraft Dynamics and Control** | Coursera (CU Boulder) | [FREE] | Phase B-C. Free to audit; certificate is paid. |
| | | | | https://www.coursera.org/specializations/spacecraft-dynamics-control |
| T.10 | **MIT BWSI — Build a CubeSat** | MIT (self-study) | [FREE] | Phase A |
| | | | | https://bwsi.mit.edu/cubesat-challenge/ |

### Relevant Rust tools

| Tool | Description | URL |
|------|-------------|-----|
| **sat-rs** | Rust FSW framework. ECSS PUS + CFDP. Heritage: OPS-SAT. | https://docs.rs/satrs |
| **spacepackets** | CCSDS + PUS + CFDP + time codes. `no_std`. | https://docs.rs/spacepackets |
| **sgp4** | SGP4 propagator. `no_std`. | https://crates.io/crates/sgp4 |
| **satkit** | SGP4 + IGRF + coordinate conversions. | https://lib.rs/crates/satkit |
| **Embassy** | Async executor for embedded. | https://embassy.dev |
| **heapless** | Fixed-capacity collections. | https://docs.rs/heapless |
| **proptest** | Property-based testing. | https://github.com/proptest-rs/proptest |
| **va416xx-rs** | HAL for Vorago rad-hard MCU. | https://github.com/us-irs/va416xx-rs |
| **nyx-space** | High-fidelity astrodynamics. | https://github.com/nyx-space/nyx |
| **AeroRust** | Catalog of Rust crates for space. | https://aerorust.org/catalogue/space-protocols/ |

### Reference repositories

| Repository | Description | URL |
|-----------|-------------|-----|
| **NASA cFS** | Most-used FSW framework (~40+ missions). C. | https://github.com/nasa/cFS |
| **NASA F Prime** | Component-driven FSW. Flew on Ingenuity. C++. | https://github.com/nasa/fprime |
| **NOS3** | Operational simulator for SmallSats. | https://github.com/nasa/nos3 |
| **42** | Attitude and orbit simulator (NASA). | https://github.com/ericstoneking/42 |
| **Vallado** | Reference astrodynamics algorithms. | https://github.com/CelesTrak/fundamentals-of-astrodynamics |
| **ops-sat-rs** | Rust experiment on ESA's OPS-SAT. | https://egit.irs.uni-stuttgart.de/rust/ops-sat-rs |
| **cubesat-adcs** | C implementation of CubeSat ADCS. | https://github.com/IvanVnucec/cubesat-adcs |
| **Yamcs** | Open-source mission control. | https://github.com/yamcs/yamcs |
| **gr-satellites** | Amateur satellite decoder. | https://github.com/daniestevez/gr-satellites |

---

## Summary: Investment per Phase

| Phase | Free materials | Recommended additional investment | Estimated study time |
|-------|---------------|-----------------------------------|---------------------|
| Prerequisites | P1-P5, M1-M8 | — | ~30h |
| Phase 0 | 0.1-0.10 | — | ~20h |
| Phase A | A.2-A.6, A.10-A.13 | New SMAD (~USD 130) + Curtis (~USD 90) | ~60h |
| Phase B | B.1-B.8, B.10-B.21 | Fortescue (~USD 100) | ~80h |
| Phase C | C.1-C.19 | Markley & Crassidis (~USD 100) | ~100h |
| Phase D | D.1-D.13 | — | ~40h |
| Phase E | E.1-E.4 | — | ~15h |
| Phase F | F.1-F.3 | — | ~5h |
| **Total** | | **~USD 420 recommended** | **~350h** |

**Note**: Times are very rough estimates for focused study, not including ECSS artifact
production or implementation. Study is progressive by design: you don't need all 350h before starting, only the ~30h of
prerequisites and ~20h for the current phase.

