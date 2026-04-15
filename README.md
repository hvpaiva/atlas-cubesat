# 🛰️ Atlas

CubeSat flight software in Rust, developed following ECSS standards.

## What is Atlas

Atlas is a personal, open-source project to design and build the software of a 3U CubeSat from scratch, following a process as close as possible to how a real CubeSat would be developed.

It is not a commercial product, academic thesis, or professional aerospace effort. The author is a software engineer with ~10 years of back-end product development experience, entering an unfamiliar domain and learning it through the project.

## Mission

A 3U CubeSat in Sun-Synchronous Orbit for Earth Observation. The satellite captures RGB images with onboard autonomy for target scheduling, cloud coverage assessment before downlink, and multi-pass file delivery via CFDP.

## Core premises

- Rust is the implementation language. This is a project premise, not a preference.
- The process follows ECSS-E-ST-40C Rev.1 (Software Engineering) with Category D tailoring, complemented by ECSS-E-ST-10C Rev.1 (Systems Engineering) for the overall lifecycle and documentation structure.
- The focus is software. Hardware is used only as bench-level support for practical reference.
- There is no intent to launch.
- The project is developed in public.

## Process

Every engineering decision is treated as if the launch were real. The project starts from mission definition and requirements, not from a specific subsystem or piece of hardware.

Engineering artifacts conform to ECSS Document Requirement Definitions (DRDs) and live in `docs/ecss/`, organized by phase. Decisions are recorded with full rationale next to their artifacts.

## Contributing

Feedback and suggestions are welcome, especially from people with experience in aerospace, embedded systems, or safety-critical software.

The project is not structured around dividing work. Doing the work is the point.
