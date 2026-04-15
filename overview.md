# Atlas — Project Overview

## What Atlas is

Atlas is a personal, open source learning project to design and build the software of a CubeSat, following a process as close as possible to how a real CubeSat would be developed.

The project is driven by personal interest, not by professional, academic, or commercial goals. It exists to:

- Reconnect with hands-on software development, after a career trajectory that has gradually moved toward management.
- Explore a domain of long-standing personal interest (space, physics, aerospace systems) without prior formal background in it.
- Learn areas the author has not worked with professionally: embedded systems, real-time systems, and safety-critical software.
- Build a long-term portfolio around software written in a domain where it is uncommon.

The author is a software engineer with around 10 years of experience, primarily in back-end product development. Atlas is approached from that perspective: a software engineer entering an unfamiliar domain and learning it through the project.

## Core premises

These are decisions already made about the project:

- **It is a 3U CubeSat project.** The mission is Earth Observation in Sun-Synchronous Orbit, capturing RGB images with onboard autonomy for target scheduling, image assessment, and multi-pass file delivery.
- **The implementation language is Rust.** This is a project premise, not just a preference.
- **It is open source.** The project will be developed in public.
- **The focus is software.** Although the project follows the process of building a real CubeSat, the author's interest and contribution are on the software side.
- **Hardware is used only as bench-level support.** Some simple, non-certified hardware has been acquired for bench testing, so that the work is not purely simulated. It serves as a practical reference, not as flight hardware.
- **The software is intended to be written to a professional standard**, within the author's current limitations, and portable enough that it could, in principle, be adapted to real hardware in the future, by the author or by someone else.
- **The process follows ECSS standards.** Specifically ECSS-E-ST-40C Rev.1 (Software Engineering) with Category D tailoring, complemented by ECSS-E-ST-10C Rev.1 (Systems Engineering) for the overall lifecycle and documentation structure.

## What Atlas is not

It is not a commercial product, academic project, or professional aerospace effort. The author is not an aerospace engineer and has no formal training in the field.

It is not aimed at launch. There is currently no intent to launch, and the physical/flight side of a CubeSat is not the focus. This may change in the future, but it is not a goal today.

It is not an attempt to advocate for Rust in this domain. Rust was chosen because the author wants to use it. The project is not framed as a comparison against C, C++, or Python.

It is not a tutorial or instructional material. Any documentation produced is a learning log, not a guide for others to follow.

It is not a delivery-driven project. It is a hobby, conducted alongside work and personal life. There are no deadlines, productivity expectations, or external commitments.

## Approach

Although the project will not produce flight hardware and is not aimed at launch, it is intended to be structured *as if* it were a real CubeSat development effort. This means starting from mission and requirements rather than from a specific subsystem or piece of hardware.

This approach is a reaction to an earlier attempt that started directly from a subsystem (an ADCS) without a defined mission, and which was reset for that reason.

## Collaboration

Atlas is a personal learning project. Collaboration is welcome, but in a specific sense: feedback, corrections, and suggestions from people with more experience in the relevant areas. It is not structured around dividing work, because doing so would reduce the learning value that is the project's primary purpose.

## Documentation

The author intends to document the process as a log of what was learned, the mistakes made, and the paths that had to be redone. The primary purpose is to consolidate the author's own learning and to practice writing. It may be useful to others as a side effect, but that is not its goal.

The location and format of this log are not yet defined.

