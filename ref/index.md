# Reference Material Index

> This index exists so that LLM agents can locate specific information in the Atlas project's
> reference documents without needing to read them in full. Each document has a summary,
> followed by a thematic index with page/section references.

---

## 1. nasa_csli_cubesat_101_508.pdf

**Title:** CubeSat 101 — Basic Concepts and Processes for First-Time CubeSat Developers  
**Author:** NASA CubeSat Launch Initiative (CSLI) / Cal Poly  
**Revision:** October 2017  
**Pages:** 86 (including appendices)  
**URL:** https://www.nasa.gov/wp-content/uploads/2017/03/nasa_csli_cubesat_101_508.pdf

### Summary

Introductory NASA guide aimed at first-time CubeSat developers, especially within the context of the
CSLI program. Covers the entire lifecycle of a CubeSat project: from the mission concept, through
funding, design, manufacturing, testing, licensing, integration with the dispenser and launch vehicle,
to on-orbit operations. The document is process-oriented — it does not go into deep technical details
of subsystems, but explains what needs to be done at each phase, which documents are required, and
which organizations are involved. Includes useful templates in the appendices (ODAR, transmitter
survey, materials list, compliance letter, acceptance checklists).

### Table of Contents

| Topic | Description | Pages |
|-------|-------------|-------|
| **Ch 1 — Introduction** | CubeSat definition, sizes (1U-12U), dispensers (3U and 6U), launch vehicles | p.1-8 |
| What is a CubeSat | Standard dimensions, mass, form factors (1U = 10cm cube, ~1.33 kg) | p.4 |
| Dispensers | P-POD (3U rail-based), 6U dispensers, interface with LV | p.4-6 |
| Launch vehicles | List of LVs used for CubeSats (Falcon 9, Atlas V, Electron, etc.) | p.6-8 |
| **Ch 2 — Development process** | Overview of the 16 lifecycle phases, with estimated duration for each | p.9-30 |
| Concept development | 1-6 months, mission flexibility, Keys to CSLI Selection | p.11 |
| Funding | Typical costs (materials, labor, environmental testing, travel), funding sources | p.11-13 |
| Merit and Feasibility Reviews | Mandatory reviews before submitting a proposal to CSLI | p.14-15 |
| CubeSat design | Practical design advice (KISS, external components, UL batteries, burn wire) | p.15-16 |
| CSLI proposal | AoPO process, deadlines, focus areas (science, tech, education) | p.17-18 |
| Selection and manifesting | CSLI selection process, CRADA, manifest priority | p.18 |
| Mission coordination | 9-18 months, role of the mission integrator, ICD, deliverables | p.19-20 |
| Regulatory licensing | Overview of RF licensing (FCC/NTIA) and remote sensing (NOAA) | p.20-21 |
| Flight documentation | List of 11 deliverables required for flight certification | p.21 |
| Ground station | Design, development and testing (2-12 months), SDR, TNC, troubleshooting | p.22 |
| Hardware manufacturing and testing | ETU, FlatSat, development testing vs verification testing, DITL | p.23-25 |
| Mission Readiness Review | In-person presentation to the mission integrator | p.25 |
| CubeSat-dispenser integration | 2-day process at the integration site | p.26 |
| Dispenser-LV integration | ~1-day process, without developer presence | p.27 |
| Launch | Launch day logistics | p.28 |
| Mission operations | TLE tracking, post-launch identification, operations up to 20 years | p.29-30 |
| **Ch 3 — Mission models** | 5 different organizational models depending on who provides the launch | p.31-38 |
| NASA-Procured LV | NASA LSP → mission integrator → CubeSats org chart | p.32-33 |
| ORS Rideshare | Department of Defense (DOD), ORS org chart | p.34-35 |
| NRO Rideshare | National Reconnaissance Office, APIC team | p.35-36 |
| Commercial Third-Party Broker | Brokers in commercial launches | p.37 |
| ISS Deployment | NanoRacks, deploy via ISS, specific requirements | p.38 |
| **Ch 4 — Requirements sources** | Documents that define CubeSat requirements | p.39-42 |
| ICD (Interface Control Document) | Official mission document, CubeSat-to-dispenser and dispenser-to-LV | p.40 |
| LSP-REQ-317.01 | NASA program-level requirements for CubeSats | p.40 |
| CDS (CubeSat Design Specification) | General design requirements (unofficial, for preliminary design) | p.40 |
| Dispenser specs | Specifications specific to each dispenser manufacturer | p.41 |
| Federal Statutes | FCC (47 CFR Part 97), NOAA (15 CFR Part 960) | p.41 |
| Range Safety | AFSPCMAN 91-710, EWR 127-1, Wallops Range Safety Manual | p.42 |
| **Ch 5 — Licensing** | Detailed procedures for obtaining RF and remote sensing licenses | p.43-52 |
| RF license types | Amateur (FCC Part 97), Experimental (FCC Part 5), Commercial (Part 25), Government (NTIA) | p.44-50 |
| Amateur license | IARU coordination requirements, prelaunch notification, required documents | p.45-46 |
| Experimental license | STA form (<6 months) or Form 422 (>6 months), FCC process 90 days min | p.47-49 |
| Government license | NTIA, no FCC, Spectrum Management Office | p.50 |
| Remote sensing (NOAA) | CRSRA, licensing process, imagers, NEI waiver | p.51-52 |
| **Ch 6 — Flight certification documentation** | 11 deliverables required for flight approval | p.53-64 |
| ODAR (Orbital Debris Assessment Report) | Demonstrates compliance with debris mitigation, NASA DAS software | p.54-55 |
| Transmitter survey | Communication system data for EMI/EMC analysis | p.55 |
| Materials list | List of all materials with outgassing properties (TML, CVCM) | p.55-56 |
| Mass properties report | CG, MOI, POI — first version early, final after flight unit ready | p.56 |
| Battery report | UL number, manufacturer specs, protection circuit, short circuit test | p.57 |
| Dimensional verifications | CAC checklists, verification before/after environmental testing | p.57 |
| Electrical report | Electrical diagram, inhibits, RBF pin, separation switches | p.58 |
| Venting analysis | Ventable/non-ventable volumes, acceptable ventilation rate | p.58-59 |
| DITL testing | Day In The Life — proves that software and timers work per ICD | p.59-60 |
| Dynamic environment testing | Vibration (mandatory) and shock (typically not required) | p.60-61 |
| TVAC bakeout testing | Outgassing in thermal vacuum, optional TVAC cycling | p.62-63 |
| Compliance letter | PI letter attesting compliance with ICD | p.64 |
| Safety package (MSPSP) | CubeSat hazards, submitted 45 days before arriving at the range | p.64 |
| **Appendices** | | p.65-86 |
| Abbreviations | Complete list of acronyms used in the document | p.65 |
| Glossary | Key term definitions (ADCS, breadboard, ETU, FlatSat, etc.) | p.66-68 |
| Templates | ODAR inputs, ODAR components, transmitter survey, materials list, compliance letter | p.69-78 |
| CubeSat Acceptance Checklists | Acceptance checklists for 1U, 1.5U, 2U, 3U, 3U+ | p.79-83 |
| Technical reference documents | List of applicable standards (AFSPCMAN, GSFC-STD-7000A, SMC-S-016, UL 1642, etc.) | p.84 |
| Event timeline | Notional Gantt diagram for the entire project | p.85 |

---

## 2. CDS+REV14_1+2022-02-09.pdf

**Title:** CubeSat Design Specification (CDS) — 1U to 12U  
**Author:** The CubeSat Program, Cal Poly SLO  
**Revision:** Rev 14.1 (February 2022)  
**Document:** CP-CDS-R14.1  
**Pages:** ~40 (including appendices with drawings)  
**URL:** https://www.cubesat.org/s/CDS-REV14_1-2022-02-09.pdf

### Summary

Normative document that defines the design specifications for CubeSats from 1U to 12U. It is the
industry reference standard, maintained by Cal Poly. Contains mechanical requirements (dimensions,
mass, rails, center of gravity), electrical requirements (deployment switch, RBF pin, inhibits, batteries, RF) and
operational requirements (licensing, orbital debris, deployables timing). Also specifies testing
requirements (vibration, TVAC bakeout, shock) and documents the dispensers available on the market.

**Important note:** Launch Provider requirements supersede CDS requirements. The CDS is intended
for preliminary design; official requirements come from the mission-specific ICD.

### Table of Contents

| Topic | Description | Pages |
|-------|-------------|-------|
| **Sec 1 — Introduction** | | p.7-9 |
| Overview | CubeSat history (1999, Cal Poly + Stanford), CDS objective | p.7 |
| Purpose | Ensure safety and compatibility with dispensers and launch opportunities | p.8 |
| Mission requirements | CDS is for preliminary design; LV provider requirements prevail | p.8 |
| Non-compliance with CDS | Each deviation reduces chances of finding a compatible launch | p.9 |
| Definitions | Developer, Dispenser integrator, Dispenser manufacturer, Launch Provider | p.9 |
| Operational terms | Shall (mandatory), Should (strong recommendation), Will (inevitable), Note (advice) | p.9 |
| **Sec 2 — CubeSat Specification** | Detailed technical requirements | p.9-15 |
| General specs (2.1) | Fixed parts during launch, pyrotechnics (AFSPCMAN 91-710), propulsion (3 inhibits), hazardous materials, outgassing (TML ≤1.0%, CVCM ≤0.1%), magnetic field (≤0.5 Gauss), venting | p.9-10 |
| Mechanical specs (2.2) | Coordinate system, dimensions per configuration (Appendix B drawings), "tuna can" extra volume, insertion -Z face first, protrusions ≤6.5mm, deployables constrained by the CubeSat, rails min 8.5mm width, roughness <1.6μm, radius ≥1mm, contact area 6.5x6.5mm, 75% rail in contact, mass per config (1U=2kg, 3U=6kg, 6U=12kg, 12U=24kg), CG ranges per axis, aluminum (7075/6061/6082/5005/5052), hard anodized, separation springs (≤6.7N, stroke >2.5mm) | p.10-13 |
| Electrical specs (2.3) | Power off from delivery to LV until on-orbit deploy, deployment switch (min 1), RTC (isolated, <320kHz, <10mA), RBF pin (≤6.5mm protrusion), battery protection, 3 RF inhibits, 3 deployable inhibits | p.14-15 |
| Operational specs (2.4) | RF licenses (IARU), compliance with country laws, orbital debris (NPR 8715.6, <15 Joules re-entry), deployables wait 30 min, no transmit <45 min, mandatory fit check | p.15 |
| **Sec 3 — Testing requirements** | | p.16-17 |
| Random vibration | Levels defined by the Launch Provider | p.16 |
| Thermal vacuum bakeout | Outgassing, specification defined by the Launch Provider | p.16 |
| Shock testing | Defined by LP; typically not required for CubeSats | p.16 |
| Visual inspection | CIFP or as defined by LP | p.16 |
| Testing philosophy | Qualification (eng unit) vs Protoflight (flight unit) vs Acceptance (post-integration); test flowchart (Fig 6) | p.16-18 |
| **Sec 4 — CubeSat Dispenser** | | p.18-19 |
| Interface | Two standardized systems: rail (P-POD/CPCL) and tab (PSC/CSD flange); spring deployment, pusher plate | p.18-19 |
| Dispenser images | P-POD rail (Fig 7), PSC tab (Fig 8), ISIS ISIPOD (Fig 9), PSC 6U (Fig 10), Tyvak NLAS 6U (Fig 10), AstroFein PSL-P 12U (Fig 11) | p.19-20 |
| **Sec 5 — Dispenser options** | Table of commercial dispenser capabilities (Table 3) and contacts (Table 4) | p.20-22 |
| **Sec 6 — Contacts** | Cal Poly CubeSat Lab contact | p.23 |
| **Appendix A — Change History Log** | Revision history (Rev 1 in 2003 through Rev 14.1 in 2022) | p.24-26 |
| **Appendix B — Specification Drawings** | Dimensional technical drawings for all configs (1U, 1.5U, 2U, 3U, 3U+, 6U, 6U+, 12U, 12U+) | p.27+ |
| **Acronyms** | ADC, CDS, CIFP, P-POD, RBF, RF, etc. | p.5-6 |
| **Applicable Documents** | AFSPCMAN 91-710, GSFC-STD-7000A, LSP-REQ-317.01B, NPR 8715.6B, SMC-S-016, NASA-STD-6016 | p.6 |

---

## 3. soa-2024.pdf

**Title:** State-of-the-Art Small Spacecraft Technology  
**Author:** NASA Ames Research Center / Small Spacecraft Systems Virtual Institute (S3VI)  
**Document:** NASA/TP-20250000142  
**Edition:** 2024 (published February 2025)  
**Pages:** ~420+  
**URL:** https://www.nasa.gov/wp-content/uploads/2025/02/soa-2024.pdf

### Summary

Comprehensive technical report updated annually by NASA that catalogs the state of the art in
small spacecraft technologies (up to ~180 kg, with emphasis on CubeSats and nanosatellites). Each
chapter functions as a standalone report on a subsystem, including: technology introduction,
available commercial products with tabulated specifications, TRL levels, design considerations,
and emerging technologies ("on the horizon"). It is the densest and most technical document in the
collection — it functions as a component and technology catalog for those designing a small spacecraft.

Classifies technologies by NASA's TRL (Technology Readiness Level): TRL ≥5 is considered
state-of-the-art; TRL 1-4 is "on the horizon". Mass categories: minisatellite (100-180 kg),
microsatellite (10-100 kg), nanosatellite (1-10 kg), picosatellite (0.01-1 kg), femtosatellite (0.01-0.09 kg).

### Table of Contents

| Topic | Description | Pages |
|-------|-------------|-------|
| **Ch 1 — Introduction** | Objective, scope, mass classification, TRL methodology | p.1-6 |
| SmallSat categories | Mini (100-180kg), micro (10-100kg), nano (1-10kg), pico (0.01-1kg), femto (0.01-0.09kg) | p.2 |
| CubeSat sizes | 1U to 12U with dimensions and masses (Fig 1.2, 1.3) | p.3 |
| TRL assessment | TRL 1-9 scale, TMA flowchart, terminology, heritage systems | p.3-6 |
| **Ch 2 — Complete platforms** | Hosted orbital services and commercial spacecraft buses | p.7-30 |
| Hosted orbital services | Providers that host payloads on existing vehicles (Table 2-1) | p.7-10 |
| Spacecraft bus — PocketQubes | Commercial PocketQube platforms (Table 2-2) | p.11 |
| Spacecraft bus — CubeSats | 0.25U-3U platforms (Table 2-3), 6U (Table 2-4), 12U (Table 2-5), 16U+ (Table 2-6) | p.12-21 |
| Spacecraft bus — ESPA-Class | ESPA-class 100-400 kg platforms (Table 2-7) | p.22-26 |
| Systems engineering considerations | Mission selection process | p.27 |
| **Ch 3 — Power** | Power generation, storage and distribution | p.31-59 |
| Solar cells | Multi-junction cells, efficiency, vendors (Table 3-1) | p.33-34 |
| Solar panels and arrays | Commercial products with power, mass, area (Table 3-2) | p.34-40 |
| Power vs solar distance | Practical limit by distance in AU (Fig 3.4) | p.41 |
| Horizon: advanced solar | Advanced multi-junction, flexible, organic, fuel cells | p.41-43 |
| Li-ion/LiPo batteries | Commercial packs (Table 3-3), 18650 cells (Table 3-4), 21700, 4680 | p.43-49 |
| Horizon: energy storage | Supercapacitors, solid-state batteries, low-temperature batteries | p.49-51 |
| PMAD (Power Management) | Commercial EPS boards (Table 3-9), MPPT, bus regulation | p.51-55 |
| Horizon: PMAD | Modular architecture, wireless power transfer | p.55 |
| **Ch 4 — In-space propulsion** | All propulsion types for small spacecraft | p.60-139 |
| Definitions and TRL | delta-V, Isp, thrust, PMI classifications (Concept/Development/Engineering/Flight) | p.62-66 |
| Technology overview | Comparative table of all types (thrust range, Isp range) — Table 4-1 | p.67 |
| Chemical: hydrazine monoprop | Traditional systems, vendors (Table 4-2) | p.68-70 |
| Chemical: green propellants | ADN, HAN, HTP, water electrolysis, bipropellants (Table 4-3) | p.70-75 |
| Chemical: hybrids | Hybrid systems (Table 4-4) | p.75-76 |
| Chemical: cold gas | N2, R236fa, butane, xenon (Table 4-5) | p.77-79 |
| Chemical: solid motors | Solid motors (Table 4-6) | p.79-80 |
| Electric: electrothermal | Resistojets, arcjets (Table 4-7) | p.82-84 |
| Electric: electrospray | Ionic liquid, FEEP (Table 4-8) | p.84-87 |
| Electric: gridded-ion | DC/RF discharge, iodine propellant (Table 4-9) | p.87-91 |
| Electric: Hall-effect | Xenon, krypton, iodine thrusters (Table 4-10) | p.91-98 |
| Electric: pulsed plasma | PPT, vacuum arc (Table 4-11) | p.98-101 |
| Electric: ambipolar | Ambipolar thrusters | p.101 |
| Propellant-less | Solar sails, tethers, electric sails, aerodynamic drag | p.102+ |
| Trade space | Thrust vs Isp chart for all types (Fig 4.2) | p.68 |
| **Ch 5 — GNC (Guidance, Navigation & Control)** | Attitude sensors and actuators, navigation | p.140-170 |
| Integrated ADCS units | Complete attitude control units (Table 5-1) | p.141-143 |
| Reaction wheels | Commercial products with torque, momentum, mass (Table 5-2) | p.143-146 |
| Magnetic torquers | Commercial magnetorquers (Table 5-3) | p.146-148 |
| Thrusters for ADCS | Attitude control thrusters (Table 5-4) | p.148 |
| Star trackers | Products with FOV, accuracy, mass, rad tolerance (Table 5-5) | p.148-151 |
| Magnetometers | 3-axis magnetometers (Table 5-6) | p.151-152 |
| Sun sensors | Analog/digital sun sensors (Table 5-7) | p.152-156 |
| Horizon sensors | Earth horizon sensors (Table 5-8) | p.156 |
| Gyros and IMUs | FOGs, MEMS gyros, IMUs with bias stability and ARW (Table 5-9) | p.156-161 |
| GPS receivers | GPS receivers for small spacecraft (Table 5-10) | p.161 |
| Deep space navigation | SDST, IRIS V2 transponders (Table 5-11) | p.162 |
| Atomic clocks | Atomic clocks and oscillators (Table 5-12) | p.162-163 |
| LiDAR | LiDAR systems for small spacecraft (Table 5-13) | p.163 |
| Formation flying & RPO | CPOD, Starling, AutoNGC — proximity operations | p.165 |
| **Ch 6 — Structures, Materials and Mechanisms** | Primary structures, mechanisms, additive manufacturing, radiation | p.171-204 |
| Standard CubeSat structures | Dimensions per config, commercial structures (Tables 6-1, 6-2) | p.171-173 |
| DiskSat | Alternative flat form factor concept | p.173 |
| Dispensers | Dimensional and mass requirements for dispensers (Table 6-3) | p.174-175 |
| Construction methods | Monocoque, modular frames, additive manufacturing | p.175 |
| Mechanisms | Actuators (Table 6-5), deployable booms (Table 6-6), robotic arms (Table 6-7) | p.176-181 |
| Polymeric additive manufacturing | PLA, ABS, Nylon, PC, Windform, PEI/Ultem, PEEK/PEKK, photopolymers (Tables 6-7 to 6-14) | p.182-191 |
| Radiation shielding | Inherent shielding, Z-Shielding (Shields-1 mission), ad hoc shielding, charge dissipation | p.193-199 |
| **Ch 7 — Thermal control** | Passive and active thermal control systems | p.205-225 |
| Passive thermal control | MLI, coatings, radiators, heat pipes | p.205+ |
| Active thermal control | Heaters, louvers, cryo-coolers | p.205+ |
| **Ch 8 — Avionics (Small Spacecraft Avionics)** | CDH, flight software, processors, interfaces | p.226-247 |
| Onboard computing systems | ~50 products from ~30 vendors with detailed specs (Table 8-1) | p.231-238 |
| Rad-hard processors | Vorago, Cobham GR740 (LEON4), BAE 5545 | p.239 |
| Memory types | SRAM vs DRAM vs Flash vs MRAM vs FeRAM vs CRAM (Table 8-2) | p.239 |
| Bus interfaces | RS-232, SPI, I2C, CAN Bus, SpaceWire, SerDes | p.240 |
| Radiation mitigation | TID, DDD, SEEs, SEUs, SEL — mitigation techniques | p.240 |
| Flight software frameworks | cFS, F Prime (F'), NanoSat MO Framework, ROS | p.242 |
| Operating systems | VxWorks, RTEMS, FreeRTOS, Linux | p.242 |
| Languages | C, C++, Python, Arduino | p.242 |
| Horizon: CDH | AI/ML on-orbit, SDRs on FPGAs, edge computing, GPU (NVIDIA Jetson) | p.243 |
| Horizon: FSW | Multicore processing, autonomous systems, cybersecurity | p.243 |
| **Ch 9 — Communications** | RF and optical communications for small spacecraft | p.248-282 |
| Frequency bands | VHF to V-band, allocation table (Table 9-1) | p.249 |
| Communication architecture | Transceiver, amplifiers, antennas, link budget | p.250-252 |
| Policies and licensing | FCC Parts 5/25/97, NOAA, IARU, FIPS 140-3 encryption | p.252-253 |
| Antennas | ~60 commercial antennas, VHF to Ka-band, with specs (Table 9-2) | p.257-262 |
| Radios | ~80+ commercial radios/SDRs/transceivers (Table 9-3) | p.263-271 |
| Beyond-LEO comms | MarCO, CAPSTONE, BioSentinel — deep space CubeSat comms | p.255 |
| Free Space Optical Comms | Laser comm terminals, PAT systems, optical ground stations | p.272-278 |
| Laser comm terminals | 14 LCTs with data rates up to 200 Gbps — TBIRD (Table 9-4) | p.278 |
| Horizon: optical/quantum | Quantum key distribution, DORA | p.279 |
| **Ch 10 — Integration, Launch, Deployment and Orbital Transport** | Launch, dispensers, OTV/OMV | p.283-302 |
| Launch market | 2,938 spacecraft launched in 2023; 68% < 600 kg | p.283 |
| Launch paradigms | Dedicated vs rideshare (SpaceX Transporter) | p.285-286 |
| CubeSat dispensers | Rail-type vs tab-type, mechanical details | p.286-288 |
| Separation systems | MLB, Marman band, multi-point systems | p.288 |
| Integration hardware | ESPA ring, ESPA Grande, SpaceX Cake Topper/Plate, SSMS | p.289-290 |
| Orbital Transfer Vehicles | ~25 commercial OTV/OMVs with specs (Table 10-1): Firefly Elytra, D-Orbit ION, Rocket Lab Photon, Momentus Vigoride, etc. | p.291-296 |
| ISS deployment | NRCSD, Kaber, J-SSOD, NICL, SEOPS SlingShot | p.297-298 |
| **Ch 11 — Ground Data Systems and Mission Operations** | Ground stations, networks, operations software | p.303-375 |
| Ground architecture | Ground station terminal, MOC, SOC, DTE vs space relay | p.304-305 |
| Frequencies and link budget | Band selection, licensing (FCC, NTIA, ITU, IARU) | p.306-307 |
| NASA Near Space Network (NSN) | Government and commercial stations, capabilities by frequency (Tables 11-3 to 11-5) | p.310-313 |
| NASA Deep Space Network (DSN) | Goldstone, Madrid, Canberra; 34m and 70m antennas | p.314-316 |
| KSAT / KSAT-LITE | 100+ 3.7m antennas, global Ka-band network | p.317 |
| Ground Segment as a Service (GSaaS) | AWS Ground Station, Viasat RTE, Leaf Space, ATLAS Global Network | p.317-328 |
| Space relay networks | TDRSS, Iridium short burst data | p.328-330 |
| Ground station components | Antennas, radios (NI USRP X310/X410), modems (Cortex), software (Gpredict, GNU Radio) | p.330-340 |
| Mission operations software | COSMOS, Galaxy, Orbit Logic, Yamcs, Major Tom (Table 11-16) | p.356-360 |
| Cybersecurity | SPD-5, NASA STD-1006, NIST, CCSDS security guidance | p.350-351 |
| Ground aggregators | RBC Signals, InfoStellar, Spaceit (Table 11-14) | p.354-356 |
| Horizon: optical ground | JPL OCTL, DSN optical hybrid, European Optical Nucleus Network | p.361-370 |
| **Ch 12 — Identification and Tracking** | On-orbit spacecraft tracking, conjunction assessment | p.376-388 |
| Ground tracking systems | US Space Force, Space Fence, HUSIR, LeoLabs, ExoAnalytic | p.378-379 |
| Tracking aids | SpaceNav, COMSPOC, Kayhan Space (Table 12-1) | p.380 |
| Radio-based ID | NearSpace Launch Black Box, JAXA NovaHD | p.381-382 |
| Optical/RF ID | Van Atta arrays, laser corner cube reflectors, passive albedo increase | p.382-385 |
| Autonomous ops | Starling 1.5 autonomous collision avoidance | p.385 |
| **Ch 13 — Deorbit Systems** | Devices and techniques for orbit removal | p.389-414 |
| Passive drag | Drag sails, inflatables | p.389+ |
| Active propulsion for deorbit | Dedicated deorbit thrusters | p.389+ |
| Electrodynamic tethers | Tethers for deorbit | p.389+ |
| Regulations | 25-year rule (historical), FCC 5-year rule (new) | p.389+ |
| **Ch 14 — Summary** | General summary of all technologies | p.415-416 |
| **Appendix E — TRL Levels** | Detailed definition of TRL levels 1-9 (NPR 7123.1C) | p.417+ |

---

## 4. CACs+for+CIFP+March+2020.pdf

**Title:** CubeSat Acceptance Checklists (CACs) for CIFP  
**Author:** Cal Poly CubeSat Program  
**Revision:** March 2020  
**Pages:** 13  
**URL:** https://www.cubesat.org/s/CACs-for-CIFP-March-2020.pdf

### Summary

Set of dimensional acceptance checklists used during the CubeSat Inspection and
Fit-check Procedure (CIFP). These are practical forms to verify that a CubeSat meets the
dimensional requirements of CDS Rev 14 before integration with the dispenser. Each checklist contains
diagrams with face/rail/side identification, fields for dimensional measurements, and the
required limits.

### Table of Contents

| Topic | Description | Pages |
|-------|-------------|-------|
| 1U Acceptance Checklist | Mass <2.00 kg, width 100.0±0.1mm, length 113.5±0.1mm, standoffs ≥6.5mm, protrusions ≤6.5mm, RBF pin ≤6.5mm | p.1-2 |
| 1.5U Acceptance Checklist | Mass <3.00 kg, length 170.2±0.1mm | p.3-4 |
| 2U Acceptance Checklist | Mass <4.00 kg, length 227.0±0.2mm | p.5-6 |
| 3U Acceptance Checklist | Mass <6.00 kg, length 340.5±0.3mm | p.7-8 |
| 6U Acceptance Checklist | Mass <12.00 kg, width 226.3±0.1mm (long sides), length 366.0±0.1mm | p.9-10 |
| 12U Acceptance Checklist | Mass <24.00 kg, width 226.3±0.1mm, length 366.0±0.1mm | p.11-12 |
| U+ (Tuna Can) Checklist | Extra volume: Z length ≤36mm, diameter ≤64mm, location 50.0±0.1mm from corner | p.13 |

Each checklist verifies: mass, RBF pin, rails anodized, deployables constrained, separation
mechanisms, deployment switches, width (±Z, middle, -Z), rail length, standoffs
(+Z and -Z), protrusion edge distances (≥8.5mm), lateral protrusions (≤6.5mm), Z face protrusions.

---

## 5. repos.txt

**Title:** Repository Reference Links  
**Type:** Text file with URLs organized by category  
**Content:** ~35 repositories

### Summary

Collection of open-source repositories relevant to the Atlas project, organized in 6 categories:
Flight Software Frameworks, CubeSat Hardware/Platforms, Rust Embedded / Execution Models,
Rust Space/Astrodynamics, Simulation, and Safety-Critical Rust. Collected from the COMPASS
research dossiers (dossiers 001-013).

### Table of Contents

| Category | Repositories | Highlights |
|----------|-------------|------------|
| Flight Software Frameworks | NASA cFS, NASA F Prime, sat-rs, FSFW, KubOS, CubedOS, Adamant, NanoSat MO Framework | cFS (C, 40+ missions), F Prime (C++, Ingenuity), sat-rs (Rust, OPS-SAT) |
| CubeSat Hardware/Platforms | PyCubed, COTS Star Tracker | PyCubed (CircuitPython avionics), NASA COTS Star Tracker |
| Rust Embedded / Execution Models | Embassy, Hubris, FreeRTOS-rust, embedded-alloc, embedded-test, assert-no-alloc | Embassy (async), Hubris (microkernel with MPU isolation) |
| Rust Space/Astrodynamics | spacepackets, va416xx-rs, ops-sat-rs, satkit, nyx-space, sgp4, lox-space, awesome-space | satkit (SGP4+IGRF+propagation), spacepackets (CCSDS/PUS no_std) |
| Simulation | 42 (NASA), Basilisk, TrickCFS, Vallado | 42 (attitude/orbit), Basilisk (CU Boulder), Vallado (reference) |
| Safety-Critical Rust | Safety-Critical Rust Coding Guidelines | Rust Foundation, v0.1, MISRA alignment |

---

## 6. ECSS-E-ST-40C-Rev.1(30April2025).pdf

**Title:** ECSS-E-ST-40C Rev.1 — Space Engineering: Software  
**Author:** ECSS (European Cooperation for Space Standardization) / ESA-ESTEC  
**Revision:** Rev.1 (30 April 2025)  
**Pages:** 253 (including annexes and bibliography)  
**URL:** https://ecss.nl/standard/ecss-e-st-40c-rev-1-software-30-april-2025/

### Summary

European standard that defines the principles and requirements applicable to software engineering for
space systems. It is the central ECSS document for software engineering, complemented by
ECSS-Q-ST-80 (software product assurance). Covers the complete space software lifecycle:
from the specification of system-derived requirements, through architectural and detailed design,
coding, unit and integration testing, validation (against technical specification and requirements
baseline), verification (including code coverage by criticality), delivery and acceptance, operation,
maintenance (including migration and retirement), to the software security process (security analysis,
risk treatment, security activities throughout the entire lifecycle). The document is process-oriented
-- it defines "what" must be done and the "expected outputs" of each requirement, without
prescribing "how" to implement. Follows the ECSS recursive customer-supplier model and synchronizes
software reviews (SRR, SWRR, PDR, DDR, CDR, QR, AR, ORR) with system reviews. Includes 20
normative and informative annexes, notably the DRDs (Document Requirements Definitions) for each
software document (SSS, IRD, SRS, ICD, SDD, SRelD, SUM, SVerP, SValP, SUITP, SVS, SVR, SRF,
SDP, SRevP, SMP), the document organization tables by review (Annex Q), the tailoring by software
criticality A/B/C/D (Annex R, Table R-1), the general tailoring (Annex S), and the recommended code
verifications (Annex U). Rev.1 adds synchronization with ECSS-E-ST-20-40C (ASIC/FPGA),
ECSS-Q-ST-80C Rev2, and ECSS-E-ST-80C (Security), as well as a new complete software security
process (section 5.11) and Annex U on code verification.

### Table of Contents

| Topic | Description | Pages |
|-------|-------------|-------|
| **Change log** | Revision history: ECSS-E-40A (1996), ECSS-E-40 Part1B/Part2B (2003/2005), ECSS-E-ST-40C (2009), ECSS-E-ST-40C Rev.1 (2025). Detailed list of added requirements, modifications and editorial corrections | p.3-4 |
| **Introduction** | Definition of principles and requirements for space software engineering; complements ECSS-Q-ST-80; based on ISO 9000 and ISO/IEC 12207 | p.10 |
| **1 — Scope** | Applicable to "product software" of space systems (space segment, launch service, ground segment). Covers the entire lifecycle: requirements, design, production, V&V, transfer, operations and maintenance. Includes non-deliverable software that affects product quality. Allows tailoring per ECSS-S-ST-00 | p.11 |
| **2 — Normative references** | ECSS-S-ST-00-01, ECSS-E-ST-10-06, ECSS-E-ST-10-11, ECSS-M-ST-10, ECSS-M-ST-10-01, ECSS-M-ST-40, ECSS-Q-ST-80 | p.12 |
| **3 — Terms, definitions and abbreviated terms** | 51 specific definitions (acceptance test, automatic code generation, code coverage, condition, critical software, deactivated code, decision coverage, MC/DC, metric, migration, processing unit, software product, validation, verification, vulnerability, walk-through, etc.). Common abbreviations (AR, CDR, COTS, DDF, DDR, DJF, DRD, FPGA, HMI, ICD, IRD, MOTS, PDR, QR, SDD, SRR, SVSR, TRR, etc.) | p.13-22 |
| **3.4 — Nomenclature** | "Shall" = mandatory requirement, "should" = recommendation, "may" = permission, "can" = capability/possibility | p.22 |
| **4 — Space system software engineering principles** | Introduction to the process framework and the standard's context | p.23-34 |
| 4.1 — Introduction | Context: software engineering within space system engineering. Complemented by ECSS-Q-ST-80, ECSS-M-ST-40, ECSS-Q-ST-20. Recursive customer-supplier relationship | p.23 |
| 4.2 — Process overview | Description of all 10 software engineering processes, their interfaces and review flow (SRR, SWRR, PDR, DDR, CDR, QR, AR, ORR). Fig 4-1: processes in ECSS; Fig 4-2: lifecycle overview with reviews | p.24-32 |
| 4.2.1 — General | Customer-supplier model, functional allocation, HW/SW interface | p.24-25 |
| 4.2.2 — SW related system requirements | Production of the requirements baseline (RB) for SRR. System engineering functions from ECSS-E-ST-10 | p.27 |
| 4.2.3 — SW management process | Software development plan, reviews, interface management, technical budgets | p.27-28 |
| 4.2.4 — SW requirements and architecture | Elaboration of the technical specification (TS), ICD, preliminary SDD. Trade-offs in the DJF. PDRs for review | p.28 |
| 4.2.5 — SW design and implementation | Detailed design, DDF, DJF, code, unit testing, integration testing. CDRs for review | p.28 |
| 4.2.6 — SW validation process | Validation against TS (before CDR) and against RB (before QR). SVSR and TRR. Degrees of independence (ISV, ISVV) | p.29 |
| 4.2.7 — SW delivery and acceptance | Preparation for delivery, acceptance testing, AR | p.29 |
| 4.2.8 — SW verification process | Concurrent verification with all processes. Variable independence (ISVV). Before PDR for plan, in DJF at each review | p.30 |
| 4.2.9 — SW operation process | Post-AR operation. SOS entity, helpdesk, user support, operational testing, vulnerability analysis | p.30-31 |
| 4.2.10 — SW maintenance process | Modification, migration, retirement. Activated before operations. Maintainer = supplier | p.31 |
| 4.2.11 — SW security process | New in Rev.1. Security analysis maintained throughout the lifecycle, risk at each architectural level, different methods per phase | p.32 |
| 4.3 — Organization of this Standard | Single normative clause (5), processes and activities decomposed into tasks with expected outputs. Annexes B-P and T: DRDs. Annex Q: docs by review. Annex R: tailoring by criticality. Annex S: general tailoring. Annex U: code verification | p.32-33 |
| 4.4 — Tailoring | Drivers: safety, dependability, security, development, quality, business. Annex R for criticality, Annex S for general | p.34 |
| 4.5 — Security aspects | Security assurance influences development requirements; increased controls per assurance level | p.34 |
| **5 — Requirements** | Main normative clause with all software engineering requirements | p.35-99 |
| 5.1 — Introduction | Hierarchical requirement identification (e.g. 5.5.3.2a), expected outputs with DRD and associated review | p.35 |
| **5.2 — SW related system requirement process** | | p.36-42 |
| 5.2.2 — System requirements analysis | Specification of requirements allocated to software (functions, performance, V&V, operations, maintenance, in-flight modification, real-time, security, quality). Observability, HMI, HW/SW co-engineering analysis. Security requirements allocation with catalogs (ISO 27002, NIST SP 800-53) and traceability matrix | p.36-38 |
| 5.2.3 — System verification | V&V process requirements, security V&V, validation scenarios, installation/acceptance requirements | p.38 |
| 5.2.4 — System integration and control | Versioning, delivery content, supplier support, interface spec (incl. ASIC/FPGA), system database, development constraints, OBCP, reuse, safety/dependability, format/data medium, security marking, integrity/authenticity, security constraints, secure delivery | p.39-42 |
| 5.2.5 — System requirements review | SRR per 5.3.4.1a | p.42 |
| **5.3 — SW management process** | | p.42-52 |
| 5.3.2 — SW life cycle management | Lifecycle definition (phases, inputs, outputs, reviews), dev/maintenance interfaces, procurement, automatic code generation (autocode model review, interface, tools, V&V strategy, CM), changes to baselines | p.42-45 |
| 5.3.3 — Joint review process | Joint reviews (7 criteria + security), software project reviews (SRR, PDR, CDR, QR, AR min.), review plan, software technical reviews (supplier-led) | p.45-46 |
| 5.3.4 — SW project reviews description | SRR (approved RB), PDR (approved TS, architecture, plans), SWRR (anticipation of PDR), CDR (approved DDF, DJF), DDR (anticipation of CDR), QR (qualified product), AR (accepted product) | p.46-48 |
| 5.3.5 — SW technical reviews | TRR (test readiness), TRB (test results), SW DRB (delivery review board), SVSR (validation spec review) | p.48 |
| 5.3.6 — Review phasing | Flight SW: SRR ≤ system PDR, SW PDR between system PDR and CDR, SW CDR before system QR, SW QR within system QR. Ground SW: SWRR before GS PDR, SW PDR before GS CDR, others before GS QR | p.49-50 |
| 5.3.7 — Interface management | Procedures per ECSS-M-ST-40 | p.50 |
| 5.3.8 — Technical budget and margin management | Budget targets (PU load, memory, deadline, communication), margin philosophy, margin computation (PU: margin_WCET, margin_slack, margin_utilisation; memory: margin = free/total) | p.50-51 |
| 5.3.9 — Compliance to this Standard | Compliance matrix and documentation compliance | p.52 |
| **5.4 — SW requirements and architecture engineering process** | | p.52-57 |
| 5.4.2 — SW requirements analysis | Establishment and documentation of requirements (functional, performance, operational, safety, security, HMI, data, validation, interfaces, reuse, security risk treatment). In-flight modification specs. Logical model (with behavioural view). SWRR | p.52-54 |
| 5.4.3 — SW architectural design | Transformation of requirements into architecture (top-level structure, components, hierarchy, dependencies, interfaces, dynamic architecture, behavior). Design method. Architecture vulnerability analysis. Computational model for real-time. Behavior description. Preliminary interfaces. Reuse (methods, evaluation, config data separation). Reuse of existing software. Integration | p.54-57 |
| 5.4.4 — PDR | Preliminary design review per 5.3.4.2 | p.57 |
| **5.5 — SW design and implementation engineering process** | | p.57-61 |
| 5.5.2 — Design of software items | Detailed design of each component, refinement into units, detailed interfaces, design model (static, dynamic, behavioral), design method, real-time (timing, synchronization, mutual exclusion, dynamic allocation, protection), method consistency, user manual, unit test plan, DDR | p.57-60 |
| 5.5.3 — Coding and testing | Development and documentation of units and build procedures. Unit testing: boundary exercise (n-1, n, n+1), messages/errors, globals, out-of-range, stress testing | p.60-61 |
| 5.5.4 — Integration | Integration test plan (design, cases, procedures, data). Incremental integration and testing | p.61 |
| **5.6 — SW validation process** | | p.62-66 |
| 5.6.2 — Validation process implementation | Establishment, methods/tools, independence, regulations/policies, independent organization (ISV) | p.62-63 |
| 5.6.3 — Validation w.r.t. technical specification | Tests (stress, boundary, singular, error isolation, operational environment, external interfaces, HMI, security). Validation by test preferred; analysis/inspection if justified. CDR | p.63-64 |
| 5.6.4 — Validation w.r.t. requirements baseline | Tests against RB (mission data/scenarios, stress/boundary, error isolation, operational environment, external interfaces, HMI, security). Black box on the final product. QR | p.65-66 |
| 5.6.5 — SW validation control | Validation control with status per requirement (executed/partial/not executed, success/failure/pending), traceability, configuration, dates, logs, SPRs | p.66 |
| **5.7 — SW delivery and acceptance process** | | p.67-69 |
| 5.7.2 — Delivery and installation | Product preparation, secure delivery, training, installation procedures (incl. secure), installation reporting | p.67-68 |
| 5.7.3 — SW acceptance | Acceptance test planning, execution, executable code generation, supplier support, evaluation (traceability to RB), AR | p.68-69 |
| **5.8 — SW verification process** | | p.70-79 |
| 5.8.2 — Verification process implementation | Establishment, software products identification, methods/tools, independence/risk, security regulations, independent organization (ISVV) | p.70-71 |
| 5.8.3 — Verification activities | Verification of: requirements baseline (11 criteria incl. security), technical specification (11 criteria incl. security/criticality), architectural design (11 criteria incl. dynamic features), detailed design (12 criteria incl. timing sync), code (8 criteria — examples in Annex U) | p.71-75 |
| 5.8.3.5b — Code coverage by criticality | **Critical table**: Cat A = 100% statement + 100% decision + 100% MC/DC; Cat B = 100% statement + 100% decision + TBA MC/DC; Cat C/D = TBA (agreed with customer). Object code coverage: Cat A = 100% | p.75 |
| 5.8.3.5f — Robustness verification | Static analysis for errors difficult to detect at runtime | p.76 |
| 5.8.3.6 — Verification of unit testing | 10 verification criteria for unit test results | p.76 |
| 5.8.3.7 — Verification of integration | Traceability, internal consistency, interface testing, conformance | p.76-77 |
| 5.8.3.8 — Verification of validation | Traceability of RB and TS to validation spec, result conformance | p.77 |
| 5.8.3.9 — Complementary system level validation | Identification of requirements that cannot be validated in the supplier's environment | p.77 |
| 5.8.3.10 — Documentation verification | Adequacy, completeness, consistency, timeliness, CM compliance | p.78 |
| 5.8.3.11 — Schedulability analysis (real-time) | Analytical model to prove design feasibility; refined at each phase (PDR, CDR, QR) with values measured in representative environment | p.78 |
| 5.8.3.12 — Technical budgets management | Memory size and PU utilization estimation; updated at each phase; comparison with margins | p.79 |
| 5.8.3.13 — Behaviour modelling verification | Behavior verification using logical model, architecture view and design model | p.79 |
| **5.9 — SW operation process** | | p.80-82 |
| 5.9.2 — Process implementation | Operational testing (incl. vulnerability analysis and penetration testing), support plans/procedures, problem handling, security impact protection | p.80-81 |
| 5.9.3 — Operational testing | Execution per release, demonstration of operational requirements (HW environment, fault tolerance, config, sequences, SOS interventions), software release | p.81 |
| 5.9.4 — SW operation support | Execution of support plan, problem handling, vulnerabilities in operations (continuous monitoring, security analysis, audit) | p.82 |
| 5.9.5 — User support | Assistance, request handling, action reporting, work-around solutions, permanent corrections via maintenance | p.82-83 |
| **5.10 — SW maintenance process** | | p.83-89 |
| 5.10.2 — Process implementation | Maintenance plan, compatibility with development processes, CM, problem reporting, security constraints, long term maintenance for flight SW | p.84-85 |
| 5.10.3 — Problem and modification analysis | Impact analysis (type, scope, criticality), reproduction, implementation options, approval | p.85 |
| 5.10.4 — Modification implementation | Analysis of documentation/models/units, change documentation, invocation of engineering processes (5.3-5.8, 5.11), test criteria, non-regression assurance | p.86 |
| 5.10.5 — Maintenance reviews | Joint reviews for authorization and integrity, baseline for change | p.87 |
| 5.10.6 — SW migration | Applicability, planning (7 items), plan contribution, preparation, notification, post-operation review, data accessibility | p.87-89 |
| 5.10.7 — SW retirement | Planning (cessation, archiving, responsibility, transition, data security), notification, requirements, retired product data accessibility | p.89 |
| **5.11 — SW security process** | New in Rev.1. Concurrent process with all others | p.90-99 |
| 5.11.1 — Overview | Composed of: process implementation, security analysis, security risk treatment, security activities in the lifecycle | p.90 |
| 5.11.2 — Process implementation | Software security management plan (SSMP) with 8 items: objectives, organization, relationship with internal processes, stakeholders, planning, deliverables, tools (threat identification, vulnerabilities), review frequency. Security manager. Security constraints in the lifecycle | p.90-91 |
| 5.11.3 — SW security analysis | Production and maintenance of the security analysis report and risk treatment plan. Methods identified in planning. Analysis based on higher-level requirements and regulations. Hierarchy: bidirectional propagation. Need-to-know distribution. Risk-vulnerability mapping. Review at milestones, change requests, new threats. Component classification by sensitivity | p.91-93 |
| 5.11.4 — Security risk treatment | Treatment measures for risks above risk appetite. Transfer to general risk management. Protection of sensitive information. Requirement-measure traceability. Analysis/risks/treatments consistency. Periodic monitoring | p.93-94 |
| 5.11.5 — Security activities in the SW lifecycle | Activities at each phase: requirements baseline (security analysis for elicitation, assurance requirements, V&V type/extent); requirements spec and architectural design (iterative analysis, PDR review, architecture review); detailed design and implementation (analysis revision, vulnerabilities evaluation, CDR/DDR review); validation (regulations, TRR security approval, security measures for testing, QR review); delivery/acceptance (pre-delivery analysis validity, AR review); operations/maintenance (periodic review, response to incidents/SPRs/CRs, trends analysis, maintenance updates, migration updates, retirement security incl. data sanitation) | p.94-99 |
| 5.11.5.6g-i — Data sanitation | Data sanitation on storage media and hardware, policy compliance, sanitation records | p.99 |
| **Annex A (informative) — SW documentation** | Overview of all software documents and Document Requirements List table (Table A-1) mapping ECSS-E-ST-40 and ECSS-Q-ST-80 | p.100-105 |
| **Annex B (normative) — SSS DRD** | Software System Specification: traceability to ECSS-E-ST-40/ECSS-Q-ST-80 (Table B-1) | p.106-115 |
| **Annex C (normative) — IRD DRD** | Software Interface Requirements Document (Table C-1) | p.116-119 |
| **Annex D (normative) — SRS DRD** | Software Requirements Specification (Table D-1) | p.120-128 |
| **Annex E (normative) — ICD DRD** | Interface Control Document (Table E-1) | p.129-132 |
| **Annex F (normative) — SDD DRD** | Software Design Document (Table F-1) | p.133-143 |
| **Annex G (normative) — SRelD DRD** | Software Release Document (Table G-1) | p.144-146 |
| **Annex H (normative) — SUM DRD** | Software User Manual (Table H-1) | p.147-153 |
| **Annex I (normative) — SVerP DRD** | Software Verification Plan (Table I-1) | p.154-158 |
| **Annex J (normative) — SValP DRD** | Software Validation Plan (Table J-1) | p.159-164 |
| **Annex K (normative) — SUITP DRD** | Software Unit/Integration Test Plan (Table K-1) | p.165-173 |
| **Annex L (normative) — SVS DRD** | Software Validation Specification (Table L-1) | p.174-181 |
| **Annex M (normative) — SVR DRD** | Software Verification Report (Table M-1) | p.182-188 |
| **Annex N (normative) — SRF DRD** | Software Reuse File (Table N-1) | p.189-192 |
| **Annex O (normative) — SDP DRD** | Software Development Plan (Table O-1) | p.193-200 |
| **Annex P (normative) — SRevP DRD** | Software Review Plan (Table P-1) | p.201-210 |
| **Annex Q (informative) — Document organization by review** | Document content tables at each review: Table Q-1 (SRR), Q-2 (PDR/SWRR), Q-3 (PDR additional), Q-4 (TRR/SVSR), Q-5 (TRB), Q-6 (CDR/DDR), Q-7 (CDR additional), Q-8 (QR), Q-9 (AR), Q-10 (ORR), Q-11 (docs without explicit review), Q-12 (SW DRB), Q-13 (SVSR) | p.211-226 |
| **Annex R (normative) — Tailoring by SW criticality** | Applicability matrix (Table R-1) of each requirement by criticality category A/B/C/D per ECSS-Q-ST-80 Annex D.1. Y = applicable, N = not applicable, Ytba = DRD info may be omitted if justified. Highlights: logical model and behaviour (N for C/D), independent V&V (N for C/D), unit test (N for C/D), integration test plan (N for D), software behaviour description (N for C/D), schedulability analysis (N for D) | p.227-239 |
| **Annex S (informative) — General Tailoring** | Technical, operational and managerial factors for tailoring. List of conditional requirements (S.2) and requirements with customer-supplier agreement (S.3) | p.240-242 |
| **Annex T (normative) — SMP DRD** | Software Maintenance Plan: traceability (Table T-1), purpose, scope, general requirements, maintenance concept, activities, resources, maintenance process phases (analysis, design, implementation, acceptance, delivery), training, SPA, CM, records/reports, sample request form | p.243-251 |
| **Annex U (informative) — SW code verification** | New in Rev.1. 14 recommended code verifications: numeric protection (overflow/underflow/div-by-zero), bounds checking (buffers/arrays/strings), no undue infinite loops, correct logical/arithmetic operators, implicit conversions, variable lifetime, visibility (static/global), volatile for asynchronous access, no invalid memory accesses (NULL), no uninitialized variables, no useless assignments, no memory leaks, justified pointer arithmetic, no race conditions | p.252 |
| **Bibliography** | References: ECSS-S-ST-00, ECSS-E-ST-10, ECSS-E-ST-10-06, ECSS-E-ST-70, ECSS-E-ST-70-01, ECSS-M-ST-80, ECSS-M-ST-10, ECSS-Q-ST-20, ISO 9000:2000, ISO 9126-1:2001, ISO/IEC 2382-20:1990, ISO/IEC 12207:1995, ISO/IEC 27000:2018, IEEE 610.12-1990, RTCA/DO-178B/ED-12B, RTCA/DO-278/ED-109 | p.253 |

---

## 7. ECSS-Q-ST-80C-Rev.2(30April2025).pdf

**Title:** ECSS-Q-ST-80C Rev.2 — Space Product Assurance: Software Product Assurance  
**Author:** ECSS (European Cooperation for Space Standardization) / ESA-ESTEC  
**Revision:** Rev.2 (30 April 2025)  
**Pages:** 132  
**URL:** https://ecss.nl/standard/ecss-q-st-80c-rev-2-software-product-assurance-30-april-2025/

### Summary

European standard that defines the software product assurance requirements for the development and
maintenance of software in space systems. Applies to crewed and uncrewed spacecraft, launchers,
payloads, experiments, ground equipment and associated facilities. The standard complements
ECSS-E-ST-40 (general software engineering requirements), adding the quality and assurance
dimension to space software engineering processes. Together, the two standards specify all processes
for space software development.

The document is organized in three main parts: software product assurance programme implementation
(ch. 5), software process assurance (ch. 6), and software product quality assurance (ch. 7). Defines
requirements for organization, planning, reporting, audits, software problems, non-conformances,
quality models, risk management, supplier selection and control, procurement, tools, and assessment
and improvement processes.

A fundamental principle is the customer-supplier relationship, applied recursively in the space system
hierarchy. The standard's tailoring is based on software criticality (Annex D, categories A-D),
dependability and safety, development constraints, and product quality objectives. Rev.2 introduces
new clauses on software security (6.2.9) and handling of security-sensitive software (6.2.10), as well
as separating delivery/installation (6.3.6) from acceptance (6.3.7).

Each requirement is identified by a hierarchical number and has an associated "Expected Output",
indicating the target document (PAF, DJF, MGT, etc.), the corresponding DRD and the applicable
milestone review (SRR, PDR, CDR, QR, AR, ORR).

### Table of Contents

| Topic | Description | Pages |
|-------|-------------|-------|
| **Change log** | Revision history: ECSS-Q-80A (1996), Q-80B (2003), Q-ST-80C (2009), Rev.1 (2017), Rev.2 (2025). Main Rev.2 changes: addition of clauses 6.2.9 (software security) and 6.2.10 (handling of security software), separation of delivery/installation and acceptance | p.3-4 |
| **Ch 1 — Scope** | Scope: SPA requirements for development and maintenance of software in space systems. Applies to non-deliverable software that affects quality. Interface with ECSS-E-ST-40 (engineering) and ECSS-M (management). Allows tailoring via ECSS-S-ST-00 | p.10 |
| **Ch 2 — Normative references** | Normative documents: ECSS-S-ST-00-01, ECSS-E-ST-40, ECSS-E-ST-80 (security), ECSS-Q-ST-10/10-04/10-09/20/30/40, ECSS-M-ST-10/10-01/40/80, CSW-ESAISVV-2022-GBK-02897 (ISVV handbook), ISO/IEC 33002:2015 | p.11 |
| **Ch 3 — Terms, definitions and abbreviated terms** | 39 specific definitions: acceptance test, automatic code generation, code coverage, critical software (cat A/B/C), deactivated code, existing software (COTS/MOTS/freeware/open source), metric, processing unit (GPU/VPU/TPU/NPU/DSP), quality model, software product, vulnerability, walk-through, etc. | p.12-19 |
| **Sec 3.4 — Nomenclature** | Shall (mandatory), should (recommendation), may/need not (permission), can (descriptive) | p.19 |
| **Ch 4 — Space system SPA principles** | SPA objectives: confidence that the software satisfies requirements throughout the system's useful life. Recursive customer-supplier principle. Organization in 3 parts (Fig 4-2). Tailoring by criticality, safety, development constraints, product quality | p.20-23 |
| **Sec 4.3 — Tailoring** | Tailoring drivers: safety, dependability, development constraints, product quality. Annex D contains tailoring by criticality | p.23 |
| **Ch 5 — SPA programme implementation** | Requirements for SPA programme implementation | p.24-39 |
| 5.1 — Organization and responsibility | Organizational structure, responsibility and authority, resources, SW PA manager/engineer role, training | p.24-26 |
| 5.2 — SPA programme management | SPAP planning and control, compliance matrix, SPA reports, milestone reports (SPAMR), audits, alerts, software problems, non-conformances, quality models (10 characteristics) | p.26-31 |
| 5.3 — Risk management and critical item control | Risk management via ECSS-M-ST-80. Critical item control via ECSS-Q-ST-10-04 | p.31 |
| 5.4 — Supplier selection and control | Supplier selection, SPA requirements for sub-suppliers, monitoring | p.32-33 |
| 5.5 — Procurement | Procurement documents, SW component review, identification, inspection | p.34 |
| 5.6 — Tools and supporting environment | Methods and tools for the entire lifecycle. Development environment | p.35-36 |
| 5.7 — Assessment and improvement process | Process assessment (ISO/IEC 33002:2015), CMMI with SCAMPI A accepted, process improvement | p.36-39 |
| **Ch 6 — Software process assurance** | Assurance requirements for software engineering processes | p.40-76 |
| 6.1 — Software development life cycle | Lifecycle definition (phases, I/O, milestones, dependencies), quality objectives | p.40-41 |
| 6.2.1 — Documentation of processes | Software plans (development, specification, design, CM, V&V, maintenance, security) | p.41-42 |
| 6.2.2 — Software dependability and safety | Criticality classification based on failure consequences. HSIA. Fault propagation | p.42-44 |
| **6.2.3 — Handling of critical software** | Measures for critical SW: safe subset, formal proof, 100% branch coverage, full source inspection, independent testing, defensive programming. N for cat D | p.45-46 |
| 6.2.4 — Software configuration management | Backups, software configuration file, integrity (checksum), branching/merging procedures | p.47-49 |
| 6.2.5 — Process metrics | Metrics: duration, effort, problems in verification, problems in integration/validation | p.50 |
| **6.2.6 — Verification** | Verification plan, techniques (review, inspection, walk-through, formal proof, fault tree). Third-party ISVV — N for cat C and D | p.51-53 |
| 6.2.7 — Reuse of existing software | Reuse analysis, 13 quality aspects, reverse engineering when necessary | p.54-57 |
| 6.2.8 — Automatic code generation | Tool evaluation, modelling standards | p.57-58 |
| **6.2.9 — Software security (NEW Rev.2)** | Software security analysis (requirements, risk, design, code analysis). Status reports | p.58-59 |
| **6.2.10 — Handling of security sensitive SW (NEW Rev.2)** | Additional measures: secure coding, fuzzing, static/dynamic security testing, vulnerability assessment, penetration testing | p.60-61 |
| **6.3.4 — Coding** | Coding standards (including security, naming, commentary). Verification tools. Code quality and security metrics | p.64-65 |
| **6.3.5 — Testing and validation** | Strategy per level (unit, integration, validation). Test coverage goals agreed by criticality. Regression testing | p.66-71 |
| 6.3.6 — Software delivery and installation | Delivery Review Board. Verification of executable regenerated from components under CM | p.72 |
| **6.3.7 — Software acceptance** | Acceptance test plan, residual risk confirmation, certification (accepted/conditionally/rejected) | p.72-73 |
| 6.3.8 — Operations | Mission product quality, operational requirements validation | p.74 |
| 6.3.9 — Maintenance | Organization, plans, maintenance records | p.74-76 |
| **Ch 7 — Software product quality assurance** | Software product quality requirements | p.77-84 |
| 7.1 — Product quality objectives and metrication | Quality model, basic metrics: size, complexity, fault density, test coverage, number of failures | p.77-79 |
| 7.2 — Product quality requirements | Correct, unambiguous, complete, consistent, verifiable, traceable requirements. Design for testability | p.79-80 |
| 7.3 — Software intended for reuse | Separate and self-contained documentation. Testing on all platforms | p.81-82 |
| 7.5 — Programmable devices | Programming procedures, indelible marking, security marking | p.84 |
| **Annex A (informative) — Software documentation** | Software document structure (Fig A-1). Table A-1: Document Requirements List (~60 DRL items mapped to SRR/PDR/CDR/QR/AR/ORR) | p.85-90 |
| **Annex B (normative) — SPAP DRD** | Software Product Assurance Plan DRD. Traceability (Table B-1) | p.91-97 |
| **Annex C (normative) — SPAMR DRD** | Software Product Assurance Milestone Report DRD. Traceability (Table C-1) | p.98-100 |
| **Annex D (normative) — Tailoring by SW criticality** | Requirements tailoring based on software criticality categories | p.101-113 |
| **Table D-1 — Software criticality categories** | 4 categories (A, B, C, D). Cat A: cat I functions without compensation. Cat B: cat I functions with compensation or cat II without. Cat C: cat II functions with compensation or cat III without. Cat D: cat III functions with compensation or cat IV without compensation | p.101-102 |
| **Table D-2 — Applicability matrix** | Complete applicability matrix of all requirements by category A/B/C/D. Y=applicable, N=not applicable. Cat D: handling of critical SW (N), ISVV (N), relaxations in formal testing and design standards | p.102-113 |
| **Annex E (informative) — Requirements with built-in tailoring** | List of requirements with tailoring built into the text | p.114 |
| **Annex F (informative) — Document organization by milestone** | Expected Outputs tables per milestone: F.2 SRR, F.3 PDR, F.4 CDR, F.5 QR, F.6 AR, F.7 without milestone | p.115-131 |
| **Bibliography** | ECSS-S-ST-00, ECSS-Q-HB-80-02/03/04, ECSS-Q-ST-30-02 (FMEA), IEEE 610.12, ISO 9000, ISO/IEC 25000/25010, ISO/IEC 24765, RTCA/DO-178B, CMU/SEI CMMI | p.132 |

---

## 8. ECSS-E-ST-10C-Rev1-AnnexB-MDD-DRD.docx

**Title:** (Normative) Mission Description Document (MDD) — DRD  
**Author:** ECSS (European Cooperation for Space Standardization)  
**Revision:** ECSS-E-ST-10C Rev. 1, Annex B  
**Pages:** N/A (template/DRD)  
**URL:** https://ecss.nl/standard/ecss-e-st-10c-rev-1-system-engineering-general-requirements-15-february-2017/ (standalone DOCX download from parent standard page)

### Summary

Document Requirements Definition (DRD) for the Mission Description Document (MDD), called from ECSS-E-ST-10 requirement 5.3.1a. Defines the mandatory structure and content of the MDD, produced in Phases 0 and A for each mission concept under study. The MDD describes how the objectives, operation profile, major system events, capabilities, contingencies, and performance standards are expected to be achieved by a given system concept.

### Table of Contents

| Topic | Description | Pages |
|-------|-------------|-------|
| DRD Identification | Requirement source: ECSS-E-ST-10, req. 5.3.1a | — |
| Purpose and Objective | MDD context in Phase 0/A lifecycle; relationship with MS, TS, SEP, PMP, and System Concept Report | — |
| Introduction (B.2.1 §1) | Purpose, objective, content, and reason for preparation | — |
| Applicable and Reference Documents (B.2.1 §2) | Applicable and reference documents, including the preliminary TS | — |
| Preliminary TS Summary (B.2.1 §3) | Summary of preliminary TS objectives and design-driving requirements | — |
| Concept Description (B.2.1 §4) | Overview, mission analysis, system description element by element (space/ground/user segments), mission phase descriptions, performance drivers, constraints, operations scenarios | — |
| Assessment of Performance (B.2.1 §5) | Assessment against preliminary TS requirements; identification of non-compliances | — |
| Identification of Risk Areas (B.2.1 §6) | Risks: technology, contingencies, programmatic aspects | — |
| Conclusion (B.2.1 §7) | Strengths and weaknesses of the concept | — |

---

## 9. ECSS-E-ST-10-06C-Technical-Requirements-Spec-2009.pdf

**Title:** Space Engineering — Technical Requirements Specification  
**Author:** ECSS / ESA-ESTEC Requirements & Standards Division  
**Revision:** ECSS-E-ST-10-06C, Third Issue — 6 March 2009  
**Pages:** 31  
**URL:** https://ecss.nl/standard/ecss-e-st-10-06c-technical-requirements-specification/

### Summary

ECSS standard governing the purpose, content, and formulation of the Technical Requirements Specification (TS). Defines how the TS is established across Phase 0 (preliminary) and Phase A (release), the twelve recognized types of technical requirements, and the mandatory quality attributes each requirement must satisfy. Annex A provides the normative DRD for the TS, specifying the seven mandatory sections. Adapted from ISO 21351.

### Table of Contents

| Topic | Description | Pages |
|-------|-------------|-------|
| Introduction | Scope and relationship to ISO 21351 | p.7 |
| 1. Scope | Applicability to all space systems, product elements, and projects | p.8 |
| 2. Normative References | ECSS-S-ST-00-01 (Glossary), ECSS-E-ST-10-02 (Verification) | p.9 |
| 3. Terms, Definitions | Constraint, environment (product/project/development), function, functional analysis, life cycle, mission, need, specification, TS | p.10-12 |
| 4. TS Purpose and Description | Purpose as customer's expression of needs (4.1); three content sets: administrative, project/product context, technical requirements (4.2) | p.13-14 |
| 5. Process for Establishing a TS | Preliminary TS in Phase 0 (tasks F1.1-F1.4, Figure 5-1); TS in Phase A (tasks F1.5-F1.10, Figure 5-2) | p.15-17 |
| 6. Technical Requirements Types | Twelve types: functional (6.2.2), mission (6.2.3), interface (6.2.4), environmental (6.2.5), operational (6.2.6), human factor (6.2.7), logistics (6.2.8), physical (6.2.9), product assurance (6.2.10), configuration (6.2.11), design (6.2.12), verification (6.2.13) | p.18-21 |
| 7. Overall Requirements for TS | Formulation per clause 8 (7.2.1), responsibility (7.2.2), grouping/consistency (7.2.3), completeness (7.2.4), config management (7.2.5), format (7.2.6), non-requirement clauses (7.2.7), exclusion of cost/delivery (7.2.8) | p.22-23 |
| 8. Requirements for Formulating Requirements | Performance/quantifiability (8.2.1), justification (8.2.2), traceability (8.2.3), unambiguity (8.2.4), uniqueness (8.2.5), identifiability (8.2.6), singularity (8.2.7), completeness (8.2.8), verifiability (8.2.9), tolerance (8.2.10); wording rules: positive sentences (8.3.1), shall/should/may/can (8.3.2), 27 prohibited terms (8.3.3) | p.24-27 |
| Annex A (normative) — TS DRD | Seven mandatory sections: §1 Introduction, §2 Applicable/reference docs, §3 User's need presentation, §4 Selected concept/product, §5 Life profile description, §6 Environment and constraints, §7 Requirements (per clauses 7 and 8) | p.28-30 |
| Bibliography | ECSS-S-ST-00, ECSS-E-ST-10, ECSS-M-ST-10, EN 1325-1, EN 12973, ISO 9000 | p.31 |

---

## 10. ECSS-M-ST-10C-Rev1-Project-Planning-2009.doc

**Title:** Space Project Management — Project Planning and Implementation  
**Author:** ECSS / ESA Requirements and Standards Division, ESTEC  
**Revision:** ECSS-M-ST-10C, Third issue, 31 July 2008  
**Pages:** ~50  
**URL:** https://ecss.nl/standard/ecss-m-st-10c-rev-1-project-planning-and-implementation/

### Summary

ECSS normative standard governing project planning and implementation for European space projects. Defines the seven-phase life cycle (0 through F), the mandatory review milestones (MDR, PRR, SRR, PDR, CDR, QR, AR, ORR, FRR, LRR, CRR, ELR, MCR), and the V-model review sequencing across the customer-supplier chain. Prescribes requirements for project organization, breakdown structures (function tree, product tree, WBS, OBS), and includes normative DRDs for PMP, product tree, WBS, WP descriptions, and progress reports.

### Table of Contents

| Topic | Description | Pages |
|-------|-------------|-------|
| 4.1 Project planning — Principles | Purpose, objectives, technology needs, product reuse, risk assessment, development approach, deliverables | p.12-14 |
| 4.2 Project organization — Principles | Organizational structure, communication, reporting, audits | p.15 |
| 4.3 Project breakdown structures | Function tree, specification tree, product tree, WBS, work packages, OBS | p.16-18 |
| 4.4.1 Project phasing — Introduction | Seven-phase life cycle, Figure 4-3, configuration baselines, review sequencing | p.19-20 |
| 4.4.3.2 Phase 0 — Mission analysis | Tasks: mission statement, preliminary TS, mission concepts, programmatic assessment, risk. Review: MDR | p.21-22 |
| 4.4.3.3 Phase A — Feasibility | Tasks: plans, system concepts, function tree, feasibility, critical technologies, risk. Review: PRR | p.22-23 |
| 4.4.3.4 Phase B — Preliminary definition | Tasks: finalize plans, trade-offs, preliminary design, verification program, interfaces, debris/disposal plan. Reviews: SRR, PDR | p.23-25 |
| 4.4.3.5 Phase C — Detailed definition | Tasks: detailed design, engineering models, AIT planning, interfaces, user manual. Review: CDR | p.25-26 |
| 4.4.3.6 Phase D — Qualification and production | Tasks: qualification testing, manufacturing, interoperability testing. Reviews: QR, AR, ORR | p.26-27 |
| 4.4.3.7 Phase E — Operations / utilization | Tasks: launch, commissioning, operations, ground support. Reviews: FRR, LRR, CRR, ELR | p.27-28 |
| 4.4.3.8 Phase F — Disposal | Tasks: implement disposal plan. Review: MCR | p.28 |
| 5.1-5.4 Requirements | Project planning (customers, suppliers), organization, breakdown structures, phasing requirements | p.29-34 |
| Annex A — PMP DRD | Project Management Plan structure | p.35-37 |
| Annex B — Product tree DRD | Product tree structure and identification | p.38-39 |
| Annex C — WBS DRD | Work Breakdown Structure | p.40-41 |
| Annex D — WP description DRD | Work Package description elements | p.42-43 |
| Annex E — Progress report DRD | Progress report content | p.44 |
| Annex F — Management docs per review | Table F-1: management documents mapped to review milestones MDR through MCR | p.45-46 |

---

## 11. ECSS-M-ST-10-01C-Reviews-2008.pdf

**Title:** Space Management — Organization and Conduct of Reviews  
**Author:** ECSS Secretariat, ESA-ESTEC Requirements & Standards Division  
**Revision:** ECSS-M-ST-10-01C, 15 November 2008  
**Pages:** 27  
**URL:** https://ecss.nl/standard/ecss-m-st-10-01c-organization-and-conduct-of-reviews/

### Summary

Standard defining the framework for organizing and conducting project reviews throughout the lifecycle of space projects. Establishes roles and responsibilities of review bodies (review authority, customer, supplier, review team), specifies the sequence and purpose of review meetings, and mandates Review Item Discrepancies (RIDs) as the formal mechanism for recording and resolving problems. Includes four normative annexes with DRDs for the review procedure, RID form, review team report, and review authority report.

### Table of Contents

| Topic | Description | Pages |
|-------|-------------|-------|
| 1. Scope | Identifying activities and information required for project reviews; checklists for each review type | p.6 |
| 2. Normative references | ECSS-S-ST-00-01, ECSS-M-ST-10, ECSS-E-ST-10, ECSS-Q-ST-10 | p.7 |
| 3. Terms and definitions | Consumer, review authority, RID, review prerequisite, review team, review team leader | p.8-9 |
| 4. Fundamentals of reviews | Basic principles; four core tasks: initiation, data-package prep, documentation review, findings/conclusions | p.10-11 |
| 5. Requirements | General (5.1), review bodies (5.2), roles: review authority (5.3.1), customer (5.3.2), supplier (5.3.3), review team leader (5.3.4), review team (5.3.5); prerequisite conditions (5.4); five meeting types (5.5.1-5.5.6); RID processing (5.6) | p.12-16 |
| Annex A (normative) — Review Procedure DRD | Introduction, applicable documents, scope/content, prerequisites/objectives/success criteria, organization/responsibilities, review data-package | p.17-18 |
| Annex B (normative) — RID DRD | RID content: issue, recommendation, classification, endorsement, response, concurrence, actions, close-out; example form | p.19-21 |
| Annex C (normative) — Review Team Report DRD | Scope, documentation assessment, RID statistics, findings/recommendations, conclusions | p.22-23 |
| Annex D (normative) — Review Authority Report DRD | Major findings, recommendations/decisions, assessment of objective achievement, conclusions | p.24 |
| Annex E (informative) — RID processing logic diagram | Flow diagram for RID disposition | p.25 |
| Annex F (informative) — Examples for defined terms | Actors at mission/system/subsystem/unit levels | p.26 |

---

## 12. ECSS-E-10-SE-Training-Course-2021.pdf

**Title:** ECSS E-10 System Engineering Standards — ECSS Standardisation Training Course  
**Author:** Ilaria Roma (ESA), with inputs from Andrea Santovincenzo & Hans-Peter de Koning (ESA)  
**Revision:** 2021 (training course edition)  
**Pages:** 121 slides  
**URL:** https://ecss.nl/training-material/ecss-training-material-downloads

### Summary

Training presentation covering the ECSS E-10 Systems Engineering standards series. Documents the complete SE process from requirements definition to verification and testing, including model philosophy (STM/EM/PFM), the V-Model, and MBSE introduction. Contains normative document delivery tables per review (MDR through MCR), requirement type definitions, verification methods, and qualification/acceptance test levels and factors. Directly applicable to projects that need to align with ECSS processes.

### Table of Contents

| Topic | Description | Pages |
|-------|-------------|-------|
| Background & Terminology | ECSS definitions of system, requirement, system engineering; functional vs. physical decomposition; customer-supplier chain | Slides 1-18 |
| System Life Cycle & Reviews | Phases 0/A/B/C/D/E/F; review table (MDR, PRR, SRR, PDR, CDR, QR, AR, FRR/ORR) with objectives per phase | Slides 19-21 |
| E-ST-10C: SE General Requirements | SE functions (Requirements, Analysis, Design, Verification, Integration & Control); specification tree; DDF, DJF, SEP | Slides 26-41 |
| Annex A Document Delivery Tables | Three tables mapping all DRDs to review milestones (MDR through MCR): SEP, Verification Plan, AIT Plan, ICD, VCD, Test Spec/Report, etc. | Slides 38-40 |
| E-ST-10-06C: Requirements Specification | Requirement types (functional, operational, interface, environmental, physical, design, verification); TS DRD structure | Slides 42-45 |
| E-ST-10-24C: Interface Management | IRD, ICD, IDD, IID; interface lifecycle; interface end definition | Slides 46-50 |
| E-ST-10-02C: Verification | Verification vs. validation; stages; V-Model; methods (Test, Analysis, RoD, Inspection); product categories; model philosophy (STM, EM, EQM, PFM) | Slides 51-74 |
| Model Philosophy | Prototype (QM+FM) vs. Proto-Flight (PFM) approaches; cost/risk/schedule trade-offs; hybrid approach | Slides 60-70 |
| E-ST-10-03C: Testing | Test categories (development, qualification, acceptance, proto-flight); "test as you fly"; qualification factors (KQ=1.25, +/-10C) and acceptance (KA=1.0, +/-5C) | Slides 75-90 |
| Other E-10 Standards | E-ST-10-04C (Space Environment), E-ST-10-09C (Reference Frames), E-ST-10-11C (Human Factors), E-ST-10-12C (Radiation) | Slides 91-101 |
| TRL Scale | TRL 1-9 definitions for HW and SW per ISO 16290 / ECSS-E-AS-11C | Slides 105-109 |
| MBSE | "Single Source of Truth" concept; ESA tools (OCDT/COMET, Capella, SysML); continuous digital thread Phase 0 to F | Slides 110-119 |

---

## 13. ESA-HW-Project-Phases-Cripps-2018.pdf

**Title:** Phases of an ESA Hardware Project Explained  
**Author:** Vicki Cripps (ESA / JUICE instrument team)  
**Revision:** 2018-05-23  
**Pages:** ~25 slides (presentation)  
**URL:** https://www.space.irfu.se/seminars/20180523-Cripps-HW_Project.pdf

### Summary

Presentation explaining the complete lifecycle of an ESA hardware project for a non-technical audience. Covers ECSS standardization, formal project phases (0 through F), hardware model types, test regimes (qualification and acceptance), and practical problems from real missions (JUICE, Solar Orbiter, Rosetta). Useful as a quick conceptual reference for how ESA projects are structured, reviewed, and verified.

### Table of Contents

| Topic | Description | Pages |
|-------|-------------|-------|
| ECSS Overview | European space standardization system, members, scope of 127 standards | Slides 1-3 |
| Phase 0 — Mission Definition | Mission needs, performance goals, MDR review | Phase 0 |
| Phase A — Feasibility | Initial technical designs, management plans, feasibility assessment, PRR review | Phase A |
| Requirements & Verification | EID-A/B writing, verification methods (Test, Inspection, Analysis, Review of Design) | — |
| Phase B — Preliminary Definition | Trade-off studies, long-lead procurement, SRR and PDR reviews | Phase B |
| Hardware Models | BBM, EM, STM, QM, FM, FS, PFM, EQM — representativeness and usage | — |
| Test Programme | Physical, structural, thermal, electrical testing categories (vibration, shock, TVAC, EMC, ESD) | — |
| Test Levels & Durations | Acceptance vs. qualification, TVAC cycle examples | — |
| Phase C — Detailed Definition | Design finalization, engineering model construction, CDR review | Phase C |
| Phase D — Qualification & Production | Flight hardware build and test, QR/FAR/ORR/MRR/TRR/DRB reviews | Phase D |
| Phases E & F — Operations & Disposal | FRR, LRR, CRR, ELR, MCR reviews | Phases E-F |
| Real-world Problems | Deviations in JUICE, Solar Orbiter, Rosetta: model changes, component delays, accepted risks | — |

---

## 14. ECSS-E-ST-10-02C-Rev1-Verification-2018.pdf

**Title:** Space engineering — Verification  
**Author:** ECSS Secretariat, ESA-ESTEC, Requirements & Standards Division  
**Revision:** ECSS-E-ST-10-02C Rev.1 (1 February 2018)  
**Pages:** 51  
**URL:** https://ecss.nl/standard/ecss-e-st-10-02c-rev-1-verification-1-february-2018/

### Summary

This standard establishes the requirements for the verification of space system products. It defines the fundamental concepts of the verification process, the criteria for defining the verification strategy, and specifies the requirements for implementation of the verification programme. It covers the full verification lifecycle: planning, execution and reporting, control and close-out. The standard applies to all product decomposition levels (equipment, subsystem, segment, system) and defines four verification methods (test, analysis, review-of-design, inspection), verification stages (qualification, acceptance, pre-launch, in-orbit, post-landing), and the role of the Verification Control Board (VCB). It includes Document Requirements Definitions (DRDs) for six key verification documents: Verification Plan (VP), Verification Control Document (VCD), Test Report, Review-of-Design Report, Inspection Report, and Verification Report. Rev.1 adds the pre-tailoring matrix per space product types (clause 6) and implements multiple change requests. For software verification, ECSS-E-ST-40 and ECSS-Q-ST-80 are considered fully sufficient; detailed testing requirements are in ECSS-E-ST-10-03.

### Table of Contents

| Topic | Description | Pages |
|-------|-------------|-------|
| **1 Scope** | Purpose and applicability; relationship to ECSS-E-ST-40 (SW), ECSS-E-ST-10-03 (Testing), ECSS-E-ST-10-06 (TS); tailoring per ECSS-S-ST-00 | p.6 |
| **2 Normative references** | ECSS-S-ST-00-01, ECSS-E-ST-10, ECSS-E-ST-10-03, ECSS-M-ST-10, ECSS-Q-ST-10-09, ECSS-Q-ST-20 | p.7 |
| **3 Terms and definitions** | Model philosophy, review-of-design, Verification Control Board (VCB), verification level, verification stage | p.8-9 |
| **4 Verification principles** | Informative overview: objectives, activities, documentation, planning (approach, methods, levels, stages, model philosophy, tools), execution/reporting, control/close-out. Figure 4-1: verification process flow | p.10-13 |
| **5.1 Verification process** | Top-level requirement: demonstrate product meets requirements through planning, execution/reporting, control/close-out | p.14 |
| **5.2 Verification planning** | Verification approach (5.2.1), methods — test/analysis/ROD/inspection (5.2.2), levels per decomposition (5.2.3), stages — qualification/acceptance/pre-launch/in-orbit/post-landing (5.2.4), models (5.2.5), tools incl. GSE and simulators (5.2.6), phasing with project lifecycle (5.2.7), planning documents — VP and VCD (5.2.8) | p.14-22 |
| **Table 5-1** | Product categories by heritage: A (off-the-shelf/fully qualified), B (off-the-shelf/delta qualification), C (off-the-shelf with modifications), D (newly designed) | p.18 |
| **5.3 Verification execution and reporting** | General requirements, documentation per method: test report (Annex C), analysis report, ROD report (Annex D), inspection report (Annex E), verification report (Annex F) | p.22-24 |
| **5.4 Verification control and close-out** | VCB establishment and composition, completion criteria, re-verification triggers, VCD updates | p.24-26 |
| **6 Pre-tailoring matrix** | Table 6-1 (column definitions), Table 6-2 (full applicability matrix for 9 space product types) | p.27-35 |
| **Annex A (normative) — VP DRD** | Verification Plan: 12 required sections (approach, model philosophy, strategy, programme, tools, control, documentation, organization) | p.36-38 |
| **Annex B (normative) — VCD DRD** | Verification Control Document: living document through phases C/D/E; matrix with 10 data fields per requirement | p.39-41 |
| **Annex C (normative) — Test report DRD** | Test execution description, results, anomalies, conclusions | p.42-43 |
| **Annex D (normative) — ROD report DRD** | Review-of-design verification evidence | p.44-45 |
| **Annex E (normative) — Inspection report DRD** | Physical/SW characteristics inspection | p.46-47 |
| **Annex F (normative) — Verification report DRD** | Combined multi-method verification report | p.48-49 |

---

## 15. ECSS-E-ST-10C-Rev1(15February2017).pdf

**Title:** Space engineering — System engineering general requirements  
**Author:** ECSS Secretariat, ESA-ESTEC, Requirements & Standards Division  
**Revision:** Rev.1 (15 February 2017)  
**Pages:** 116  
**URL:** https://ecss.nl/standard/ecss-e-st-10c-rev-1-system-engineering-general-requirements-15-february-2017/

### Summary

Top-level ECSS standard for system engineering. Specifies the implementation requirements for the SE process across all space systems and products. Defines five SE sub-functions (requirement engineering, analysis, design and configuration, verification, SE integration and control), their objectives, outputs, and inter-relationships. Establishes the customer-supplier model, maps SE tasks to each project phase (0 through F), and provides a pre-tailoring matrix for applicability per space product type. Contains 14 normative and informative annexes serving as DRDs for the key SE deliverables: MDD (Annex B), System Concept Report (Annex C), SEP (Annex D), Technology Plan (Annex E), Technology Matrix (Annex F), DDF (Annex G), Function Tree (Annex H), Technical Budget (Annex I), Specification Tree (Annex J), DJF (Annex K), Trade-off Report (Annex L), RTM (Annex N), RJF (Annex O), and PUM (Annex P).

### Table of Contents

| Topic | Description | Pages |
|-------|-------------|-------|
| **1 Scope** | SE implementation requirements for space systems; SW/Ground delegated to ECSS-E-ST-40/70 | p.8-9 |
| **2 Normative references** | ECSS-S-ST-00-01, ECSS-E-AS-11, ECSS-E-ST-10-02, ECSS-E-ST-10-06, ECSS-E-ST-10-24, ECSS-M-ST-10, ECSS-Q-ST-10 | p.10 |
| **3 Terms and definitions** | Requirement traceability, recurring product, system engineering, verification matrix | p.11-14 |
| **4.1 The SE discipline** | Five sub-functions: requirements engineering, analysis, design and configuration, verification, SE integration and control. Figure 4-1 (sub-functions and boundaries), Figure 4-2 (inter-relationships) | p.15-18 |
| **4.2 The SE process** | Iterative process across phases; top-down decomposition; customer-supplier model | p.19 |
| **4.3 SE tasks per phase** | Overview of tasks in Phases 0 through F | p.20-23 |
| **5.1 System engineering plan** | SEP per Annex D; consistency with lower-level plans | p.24 |
| **5.2 Requirement engineering** | General analysis (5.2.1), traceability — RTM per Annex N (5.2.2), process — TS, consolidation, risk analysis, verification methods, allocation, consistency, agreement, maintenance, baseline (5.2.3) | p.25-28 |
| **5.3 Analysis** | System analysis — MDD per Annex B, function tree per Annex H, DDF per Annex G, DJF per Annex K (5.3.1); environments and design/test factors (5.3.2); trade-off analyses — report per Annex L (5.3.3); analysis methods and tools (5.3.4) | p.28-30 |
| **5.4 Design and configuration** | Design — technical budgets per Annex I, DDF per Annex G, DJF per Annex K, PUM per Annex P (5.4.1); configuration baselines and assembly constraints (5.4.2) | p.31-33 |
| **5.5 Verification** | VP per ECSS-E-ST-10-02; product verification categories | p.33-34 |
| **5.6 SE integration and control** | Management, planning, engineering data, interface control per ECSS-E-ST-10-24, coordinate systems, technical budgets/margins, technology — Technology Matrix per Annex F, TRL per ECSS-E-AS-11, Technology Plan per Annex E, TRSL, CIL (5.6.7); risk management, changes and nonconformances | p.34-36 |
| **7 Pre-tailoring matrix** | Table 7-1 (column definitions), Table 7-2 (full applicability matrix: all requirements and annexes vs. 9 product types) | p.38-51 |
| **Table A-1** | SE deliverable documents mapped to review milestones (MDR through MCR) | p.53-55 |
| **Figure B-1** | Relationship between MS, preliminary TS, MDD, SEP, PMP, system concept report | p.57 |
| **Annex B (normative) — MDD DRD** | Mission Description Document: concept description, performance assessment, risk areas, conclusion | p.56-59 |
| **Annex C (normative) — System concept report DRD** | System-level trade-off report | p.60 |
| **Annex D (normative) — SEP DRD** | System Engineering Plan: project overview, system design approach, implementation, SE for following phases | p.61-69 |
| **Annex E (normative) — Technology Plan DRD** | TRSL template (Figure E-1), technology evaluation approach | p.70-73 |
| **Annex F (normative) — Technology Matrix DRD** | Candidate technologies per requirement/function, TRL ranking | p.74-75 |
| **Annex G (normative) — DDF DRD** | Design Definition File: functional/physical architecture, function tree, product tree, spec tree, budgets | p.76-80 |
| **Annex H (normative) — Function Tree DRD** | Hierarchical function decomposition | p.81-82 |
| **Annex I (normative) — Technical Budget DRD** | Key engineering parameters (mass, power, comms, memory) with margins | p.83-84 |
| **Annex J (normative) — Specification Tree DRD** | Hierarchical TS relationships | p.85-86 |
| **Annex K (normative) — DJF DRD** | Design Justification File: rationale, qualification status, verification synthesis | p.87-93 |
| **Annex L (normative) — Trade-off Report DRD** | Evaluation criteria, alternatives, robustness analysis, recommendation | p.94-96 |
| **Annex N (normative) — RTM DRD** | Forward/backward requirement traceability | p.98-99 |
| **Annex O (normative) — RJF DRD** | Requirements Justification File | p.100-102 |
| **Annex P (normative) — PUM DRD** | Product User Manual: function definition, product/constituent descriptions | p.103-110 |
| **Annex R (informative)** | Mapping of typical DDP to ECSS documents | p.112-113 |
| **Annex S (informative)** | Guideline content of Analysis Report | p.114-115 |

---

## 16. ECSS-E-ST-10C-Rev1-AnnexD-SEP-DRD.docx

**Title:** System Engineering Plan (SEP) — Document Requirements Definition (DRD)  
**Author:** ECSS Secretariat  
**Revision:** Rev.1 (part of ECSS-E-ST-10C Rev.1)  
**Pages:** ~8 (Annex D)  
**URL:** https://ecss.nl/standard/ecss-e-st-10c-rev-1-system-engineering-general-requirements-15-february-2017/ (standalone DOCX download from parent standard page)

### Summary

DRD defining the mandatory structure and content requirements for the System Engineering Plan (SEP), the central document governing all technical activities across a space project's lifecycle. Called from ECSS-E-ST-10 requirements 5.1a and 5.3.4a. The SEP defines the approach, methods, procedures, resources, and organization needed to specify, design, verify, operate, and maintain a system or product. The DRD emphasizes that content must be adapted to the project phase — early phases (0/A/B) focus on risk analysis and new technologies, while later phases (C/D) focus on verification and validation.

### Table of Contents

| Section | Description | Notes |
|---------|-------------|-------|
| **D.1 DRD Identification** | Source: ECSS-E-ST-10, req. 5.1a and 5.3.4a | Adapt content to project phase |
| **1. Introduction** | Purpose, objective, content, reason for preparation | |
| **2. Applicable and reference documents** | 7 mandatory refs: business agreement, PMP, PA plan, CM plan, production plan, mission ops plan, ILS plan | |
| **3.1 Project objectives and constraints** | 9 mandatory items: user's need, system objective, system architecture, lifecycle characteristics, support elements, organizational constraints, critical issues list, regulations, V&V capacity assessment | |
| **3.2 Product evolution logic** | Incremental strategy: successive versions, objectives per version | |
| **3.3 Project phases, reviews and planning** | SE schedule, milestones, critical path | |
| **3.4 Procurement approach** | Make/buy strategy per product tree item | |
| **3.5 Initial critical issues** | Critical issues at beginning of covered phase(s) | |
| **4.1 System engineering inputs** | Driving inputs (a), external means (b), internal means (c), coordinate system (d), units (e) | 5 sub-requirements |
| **4.2 System engineering outputs** | SE outputs per phase; model philosophy; margin policy per phase/category/maturity; methods/processes; discipline interrelation; interaction with actors; consistency; control activities; COTS assessment | |
| **4.3 SE team responsibilities** | Entities, key roles, cooperative work description | |
| **4.4 SE coordination** | External and internal coordination | |
| **5.1.1 SE process description** | Tailored SE process: all tasks, relationships, interfaces, iteration loops; for each task: inputs, outputs, SE functions, other actors | |
| **5.1.2 Engineering disciplines integration** | 11 disciplines: (a) mechanical, (b) electrical/electronic, (c) software (ECSS-E-ST-40), (d) communications (ECSS-E-ST-50), (e) control engineering, (f) space environment, (g) production, (h) operations (ECSS-E-ST-70), (i) logistics/maintenance, (j) human factors, (k) human interface design | 11 disciplines mandatory |
| **5.1.3 Work packages** | WBS work package descriptions | |
| **5.2 Related plans** | Sub-plans annexed to SEP; other plans by category | |
| **5.3 SE methods, tools and models** | Requirements traceability and VCD tools; supplier interfaces | |
| **5.4 Critical issues** | Issues, risks, and mitigations for current phase | |
| **6. SE for following phases** | Forward-looking SE activities; critical issues for subsequent phases | |

---

## 17. ESA-SRE-PA-2011-097-Margin-Philosophy-Rev3.pdf

**Title:** Margin philosophy for science assessment studies  
**Author:** SRE-PA & D-TEC staff (ESTEC)  
**Revision:** Issue 1, Revision 3 (15/06/2012)  
**Pages:** 11  
**URL:** https://sci.esa.int/documents/34375/36249/1567260131067-Margin_philosophy_for_science_assessment_studies_1.3.pdf

### Summary

Establishes a common margin philosophy for ESA Cosmic Vision 2015-2025 and Mars Robotic Exploration Program (MREP) assessment studies. Consistent with ECSS-E-ST-10-02C, ECSS-E-ST-31C, and ECSS-E-ST-50-05C rev.1. Covers mass, volume, delta-V, power, data processing, communications, and thermal control margins. Provides numbered requirements (R-M1-x, R-M2-x, R-V-x, R-DV-x, R-P-x, R-SW-x, R-C-x, R-T-x) with specific margin percentages for each domain and design maturity category. Heritage from BepiColombo and Solar Orbiter. Rev 3 adds volume margins and corrects thermal margin section.

### Key Margin Values

| Domain | Margin | Applicability |
|--------|--------|---------------|
| Mass — System level | 20% of nominal dry mass | All approaches |
| Mass — Equipment (OTS, Cat A/B) | >= 5% | Off-the-shelf items |
| Mass — Equipment (OTS minor mod, Cat C) | >= 10% | OTS with minor modifications |
| Mass — Equipment (new/redesign, Cat D) | >= 20% | New designed items |
| Mass — Propellant residuals | 2% | Added to propellant |
| Mass — Harness | >= 5% of nominal dry mass | Both approaches |
| Delta-V — Accurate manoeuvres | 5% | Trajectory and orbit maintenance |
| Delta-V — General orbit maintenance | 100% | Non-analytically derived |
| Delta-V — AOCS manoeuvres | 100% | Attitude control |
| Power — System level | >= 20% of nominal power | Total power budget |
| Power — Equipment (Cat A/B/C/D) | >= 5% / >= 10% / >= 20% | Same as mass categories |
| Data processing — Memory (RAM) | >= 50% | On-board memory |
| Data processing — Processor | <= 50% peak usage | On-board processor |
| Thermal — Cryogenic radiators | 50% on heat rejection | Passive cooling |
| Thermal — Active coolers | 50% on max cooling power | Active cooling |

### Table of Contents

| Topic | Description | Pages |
|-------|-------------|-------|
| **1 Introduction** | Scope: common margin philosophy for Cosmic Vision / MREP; references ECSS-E-ST-10-02C, ECSS-E-ST-31C, ECSS-E-ST-50-05C rev.1; heritage from BepiColombo and Solar Orbiter | p.4 |
| **2.1 Mass margins** | Two approaches: Nominal Dry Mass (pre-assessment) vs Maximum Separated Mass (advanced assessment/definition) | p.5 |
| **2.1.1 Margin on total dry mass** | R-M1-1 through R-M1-10: 20% system margin, equipment maturity margins (5%/10%/20% by ECSS category), propellant residuals 2%, harness >= 5%, tank volume +10% | p.5-6 |
| **2.1.2 Margin on maximum separated mass** | R-M2-1 through R-M2-9: same structure, propellant based on Maximum Separated Mass | p.6-7 |
| **2.2 Volume margins** | R-V-1 through R-V-4: Figure of Merit, volume growth drivers, maturity growth allocations | p.7 |
| **2.3 Delta-V margins** | R-DV-1 through R-DV-7: 5% accurate manoeuvres, 100% orbit/AOCS maintenance, GAM allocations (15/10/35 m/s), 5% electric propulsion navigation | p.7-8 |
| **2.4 Power margins** | R-P-1 through R-P-6: equipment maturity margins, 20% system level, sizing at EOL | p.8-9 |
| **2.5 Data processing margins** | R-SW-1, R-SW-2: >= 50% memory margin, processor peak usage <= 50% | p.9 |
| **2.6 Communications margins** | R-C-1, R-C-2: link budgets per ECSS-E-ST-50-05C rev.1 | p.9 |
| **2.7 Thermal control margins** | R-T-1 through R-T-3: temperature ranges per ECSS-E-ST-31C, cryogenic systems (50% simple / sensitivity analysis detailed), cooler qualification (>= 20% TRL 3-5, >= 10% TRL > 5) | p.9-11 |

---

## 18. ECSS-E-HB-10-02A-Verification-Guidelines-2010.pdf

**Title:** Space engineering — Verification guidelines  
**Author:** ECSS Secretariat, ESA-ESTEC, Requirements & Standards Division  
**Revision:** A (first issue)  
**Pages:** 84  
**URL:** https://ecss.nl/hbstms/ecss-e-10-02a-verification-guidelines/

> NOTE: This is a **handbook** (HB), not a normative standard. It provides supporting material and recommendations for applying ECSS-E-ST-10-02C (Verification). It does not contain requirements and cannot be made applicable on its own.

### Summary

Companion handbook to the ECSS-E-ST-10-02C Verification standard. Provides practical guidance on how to organize and perform verification of a space system product across all project phases. Covers the full verification process from planning through execution, reporting, control, and close-out. Includes extensive guidance on model philosophy selection (prototype, protoflight, hybrid, and virtual/hybrid approaches), detailed descriptions of all model types (MU, DM, SM, ThM, STM, EFM, EM, EQM, QM, LTM, PFM, FM, FS, SVF), verification methods (test, analysis, review-of-design, inspection), verification stages (qualification, acceptance, pre-launch, in-orbit, post-landing), and product categorization by heritage (Categories A-D). Referenced in the Atlas project's model philosophy decision (SVF, FVT, PFM hybrid approach).

### Table of Contents

| Topic | Description | Pages |
|-------|-------------|-------|
| **4 Verification principles** | Verification vs. validation distinction; applicability to all engineering domains; development definition | p.12-13 |
| **5.1 Verification process** | Three sub-processes: planning, execution & reporting, control & close-out | p.14 |
| **5.2.1 Verification approach** | The What/How/When framework; Figure 5-1 (basic verification approach) | p.14-18 |
| **5.2.2 Verification methods** | Four methods: test, analysis, review-of-design, inspection; method selection guidelines; methods-vs-stages applicability | p.19-23 |
| **5.2.3 Verification levels** | Equipment, subsystem, element, overall system; parts & materials level | p.23-24 |
| **5.2.4 Verification stages** | Qualification (Table 5-1: product categories A-D), acceptance, pre-launch, in-orbit, post-landing | p.24-27 |
| **5.2.5.2 Models description** | All model types: MU, DM/BB, SM, ThM, STM, Suitcase, EFM, EM, EQM, QM, LTM, PFM, FM, FS, virtual/hybrid models. **Table 5-2: Summary model definitions** | p.28-33 |
| **5.2.5.3 Model philosophies** | Prototype (Figure 5-3/5-4), Protoflight (Figure 5-5), Hybrid HW-oriented (Figure 5-6), **Hybrid with virtual models** (§5.2.5.3.5 — FVT concept, EM replaced by SW models) | p.34-40 |
| **5.2.5.4 Product matrix** | Table 5-3: example product matrix (13 subsystems, Cat A-D, model quantities) | p.39-41 |
| **5.2.6 Verification tools** | GSE, SVF, simulators, analytical tools | p.42-44 |
| **5.2.7 Verification process phasing** | Figures 5-7 through 5-10: verification activities flow per project phase | p.44-50 |
| **5.3 Verification execution and reporting** | Team responsibilities, engineering discipline interfaces, QA/PM relationships | p.51-53 |
| **5.4 Verification control and close-out** | VCB composition, close-out criteria, re-verification triggers | p.53-55 |
| **6 Verification documentation** | Detailed DRD walkthroughs with worked examples | p.56-80 |
| **6.2.1 VP** | Verification Plan: section-by-section DRD walkthrough; Figures 6-2 through 6-6 (strategies, Gantt, activity sheets) | p.58-65 |
| **6.2.2 VCD** | Verification Control Document: Figures 6-7/6-8 (close-out status, VCD sheet) | p.65-68 |
| **6.3 Reports** | TRPT, ARPT, RRPT, IRPT, VRPT with example report sheets (Figures 6-9 through 6-13) | p.69-78 |
| **Annex A** | Verification documents delivery per review milestone | p.81 |
| **Annex B** | Table B-1: tailoring guidelines per product type (10 dimensions) for every ECSS-E-ST-10-02C requirement | p.82-84 |

---

## 19. ECSS-E-TM-10-21A-System-Modelling-Simulation-2010.pdf

**Title:** Space engineering — System modelling and simulation  
**Author:** ECSS Secretariat, ESA-ESTEC, Requirements & Standards Division  
**Revision:** A (first issue), 16 April 2010  
**Pages:** 79  
**URL:** https://ecss.nl/hbstms/ecss-e-tm-10-21a-system-modelling-and-simulation/

> NOTE: This is a **Technical Memorandum** (TM), not a normative standard. It provides guidance on using system simulation to support SE tasks across the spacecraft lifecycle.

### Summary

Defines the spacecraft simulator taxonomy used in the Atlas project. Covers seven simulation facilities — SCS, MPS, FES, FVT, SVF, Spacecraft AIV Simulator, Ground System Test Simulator, and Operations Simulator — each with a specific role in the SE process. Introduces the "virtual system model" concept (a software-simulated representation of the spacecraft that evolves incrementally across project phases), model fidelity levels, harmonisation and reuse strategies. Includes numbered engineering guidelines (SIM.GE, SIM.FU, SIM.OP, SIM.IF, SIM.PE, SIM.MA, SIM.DE, SIM.VV, SIM.MO, and facility-specific requirements). Scope is limited to functional and electrical domains at system level.

### Simulator Taxonomy

| Abbreviation | Full Name | Phase | Purpose |
|---|---|---|---|
| **SCS** | System Concept Simulator | 0/A | Trade-off support, non-real-time mathematical models |
| **MPS** | Mission Performance Simulator | A/B | End-to-end mission product quality, payload performance budgets |
| **FES** | Functional Engineering Simulator | A/B/C | Requirements consolidation, algorithm validation (GNC/AOCS) |
| **FVT** | Functional Validation Testbench | A/B | Critical subsystem design validation with breadboard HW-in-the-loop |
| **SVF** | Software Validation Facility | B/C/D | OBSW validation, OBC emulation, spacecraft DB validation |
| AIV Sim | Spacecraft AIV Simulator | C/D/E | Spacecraft V&V, EGSE integration, real-time HITL |
| GS Test Sim | Ground System Test Simulator | C/D/E | Ground segment testing, dataflow tests |
| Ops Sim | Operations & Maintenance Simulator | D/E/F | Flight control training, procedure validation, anomaly investigation |

### Table of Contents

| Topic | Description | Pages |
|-------|-------------|-------|
| **4 System M&S Domain** | M&S definition, uses across lifecycle (Table 1), benefits, virtual system model concept, harmonisation, reuse | p.15-28 |
| **5.2 SCS** | System Concept Simulator: Phase 0/A trade-off support; Figure 4 | p.31-33 |
| **5.3 MPS** | Mission Performance Simulator: payload performance budgets; Figure 5 | p.33-36 |
| **5.4 FES** | Functional Engineering Simulator: algorithm validation, Monte Carlo; Figure 6 | p.36-38 |
| **5.5 FVT** | Functional Validation Testbench: breadboard HITL; Figure 7 | p.39-41 |
| **5.6 SVF** | Software Validation Facility: OBSW validation, 3 configurations (full SW, OBC model, HITL breadboard); Figures 8-9 | p.41-46 |
| **5.7 AIV Simulator** | Spacecraft AIV: EGSE, missing equipment replacement; Figures 10-11 | p.46-50 |
| **5.8 GS Test Simulator** | Ground segment V&V; Figure 12 | p.50-53 |
| **5.9 Operations Simulator** | Training, procedure validation, mission lifetime support; Figure 13 | p.53-57 |
| **5.10 Summary** | Table 2: all 7 facilities compared (scope, milestones, validation basis, verified products) | p.58 |
| **6 Engineering Guidelines** | SIM.GE (project-level), SIM.FU (functional), SIM.OP (operational), SIM.IF (interface), SIM.PE (performance), SIM.MA (maintainability), SIM.DE (design), SIM.VV (V&V), SIM.MO (model), and facility-specific requirements (SIM.SCS/MPS/FES/FVT/SVF/AIT/GST/TOM) | p.59-78 |

---

## 20. ECSS-S-ST-00-01C-Rev1-Glossary-2023.pdf

**Title:** ECSS system — Glossary of terms  
**Author:** ECSS Secretariat, ESA-ESTEC, Requirements & Standards Section  
**Revision:** Rev.1 (11 October 2023)  
**Pages:** 61  
**URL:** https://ecss.nl/standard/ecss-s-st-00-01c-rev-1-glossary-of-terms-11-october-2023/

### Summary

Master glossary for the entire ECSS standards system. Controls the definition of all common terms used across ECSS management, engineering, product assurance, and sustainability standards. Contains **250 defined terms** (clause 2.3) and approximately **130 abbreviated terms** (clause 2.4). Provides a structured space system breakdown (clause 2.2) with hierarchical definitions from "space system" down through segment/system/element/subsystem/equipment/component/material levels, accompanied by segment tree diagrams in Annex B.

CubeSat/software-relevant definitions include: validation (2.3.245), verification (2.3.246), configurable code (2.3.44), configuration management (2.3.51), FDIR, COTS, tailoring (2.3.236), TRL, OBDH, AOCS, FMEA/FMECA, redundancy types (active 2.3.7, cold 2.3.37), waiver (2.3.248), deviation, acceptance (2.3.2).

### Table of Contents

| Topic | Description | Pages |
|-------|-------------|-------|
| **1 Scope** | Controls definitions of all common ECSS terms | p.5 |
| **2.2 Space system breakdown** | Hierarchical breakdown with Figure 2-1: system/segment/element/subsystem/equipment/component/material | p.7-12 |
| **2.3 Terms and definitions** | 250 alphabetically ordered definitions (absorbed dose through work package) | p.13-47 |
| **2.4 Abbreviated terms** | ~130 abbreviations (A/D through WBS) | p.48-51 |
| **Annex A** | Traceability matrix to previous edition, listing deleted/deprecated terms | p.52-53 |
| **Annex B** | Segment trees with product examples for space, ground, launch, and support segments | p.54-58 |
| **Annex C** | Launch segment-specific terms | p.59-60 |
