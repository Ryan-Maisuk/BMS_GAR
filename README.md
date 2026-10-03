# BMS_GAR

Battery Management System & Power Distribution Board for the GAR Autonomous Vehicle Platform

## Overview

The BMS_GAR project aims to develop a custom power distribution and battery monitoring solution for the GAR autonomous vehicle platform.

The board will serve as the central power hub of the vehicle, safely distributing power from the battery to the vehicle's electrical subsystems while providing monitoring, protection, and diagnostic capabilities.

The primary objective of Revision 1 is to establish a reliable electrical backbone while also creating a collaborative design environment for students.

Rather than dividing the board into separate sections assigned to individual students, each student will independently develop their own board concept based on the same system requirements.

The team will regularly review these designs together, compare different engineering approaches, and select the best ideas to incorporate into the final Revision 1 design.

---

# Project Objectives

## Power Distribution

- Distribute battery power to vehicle electronics
- Generate required regulated voltage rails
- Provide connections for vehicle subsystems
- Support future expansion
- Maintain reliable operation under expected vehicle loads

## Battery Monitoring

- Monitor battery pack voltage
- Measure system current draw
- Estimate system power consumption
- Provide telemetry data to the vehicle controller

## Protection Features

- Fuse protection
- Reverse polarity protection
- Power rail monitoring
- Fault indication
- Emergency shutdown support

## Expandability

- Support future telemetry systems
- Support future safety systems
- Support additional sensors and peripherals
- Enable future battery management upgrades
- Allow future communication systems such as CAN

---

# Development Workflow

Revision 1 will use an individual design and collaborative review process.

Each student will work from the same system requirements but will independently investigate components, circuits, and system architectures.

The purpose of this process is to allow each student to gain experience designing the entire system while giving the team multiple engineering solutions to evaluate.

```text
                System Requirements
                        |
           +------------+------------+
           |            |            |
           v            v            v
       Student A    Student B    Student C
        Design       Design       Design
           |            |            |
           +------------+------------+
                        |
                        v
                   Design Review
                        |
                        v
                Compare Designs
                        |
                        v
               Select Best Ideas
                        |
                        v
                Team Architecture
                        |
                        v
                  Final Design
                        |
                        v
                PCB Manufacturing
                        |
                        v
                     Testing
```

# Design Process

The BMS_GAR project will follow an **individual design, collaborative review, and team integration** workflow.

Each student will begin with the same system requirements and independently develop their own solution. At defined checkpoints, the team will meet to review each design, compare approaches, and determine which ideas should move forward.

The purpose of this process is to give every student experience with the complete hardware design process while still producing one final team-designed board.

---

## Phase 1 - Requirements and Research

Before beginning circuit design, the team will establish a common set of system requirements.

All students will work from the same requirements so that the resulting designs can be compared fairly.

### Team Tasks

Determine:

- Battery voltage range
- Battery capacity
- Maximum expected system current
- Required voltage rails
- MCU voltage and current requirements
- LiDAR voltage and current requirements
- Servo voltage and current requirements
- ESC voltage and current requirements
- Additional sensor requirements
- Required connectors
- Emergency stop requirements
- PCB size or mechanical constraints
- Communication requirements
- Expansion requirements

### Individual Tasks

Each student should research possible solutions for:

- Voltage regulation
- Current sensing
- Voltage sensing
- Reverse polarity protection
- Fuse protection
- Transient protection
- Connectors
- Power distribution

### Deliverables

Each student should provide:

- Initial component research
- Estimated power requirements
- Possible circuit approaches
- Questions or unknown requirements

---

## Phase 2 - Individual System Architecture

Each student will independently develop their own proposed architecture for the board.

Students are encouraged to explore different solutions rather than attempting to make their designs identical.

Each architecture should include:

- Battery input
- Main protection
- Power distribution
- 5 V regulation
- 3.3 V regulation
- Voltage monitoring
- Current monitoring
- MCU interface
- LiDAR power
- Servo power
- ESC power
- Expansion connections
- Emergency shutdown considerations

### Deliverables

Each student should create:

- System block diagram
- Power budget
- Proposed major components
- Connector selections
- Protection strategy
- Design notes
- Open questions

---

## Design Review 1 - Architecture Review

The team will review each student's architecture together.

The purpose of this review is to compare different engineering approaches before detailed schematic design begins.

The team should discuss:

- What does each design do well?
- What could be improved?
- Which architecture is easiest to understand?
- Which design provides the best protection?
- Which design is easiest to manufacture?
- Which design is easiest to debug?
- Which design provides the most useful expansion options?
- Are any requirements missing?
- Are there components or approaches that should be investigated further?

The goal is **not to select a winning design**.

Students should use what they learn during the review to improve their own designs.

---

## Phase 3 - Individual Schematic Design

After Design Review 1, each student will create their own complete schematic.

Students may incorporate ideas discovered during the architecture review while still developing their own solution.

Each schematic should contain the major Revision 1 subsystems.

### Battery Input

Include:

- Battery connector
- Fuse
- Reverse polarity protection
- Input protection
- Ground connection

### Power Distribution

Include connections for:

- MCU
- LiDAR
- Servo
- Sensors
- Expansion devices

### Voltage Regulation

Include:

- 5 V regulator
- 3.3 V regulator
- Required capacitors
- Protection components
- Supporting circuitry

### Voltage Monitoring

Include:

- Voltage divider
- Filtering
- MCU ADC connection
- ADC protection if required

### Current Monitoring

Include:

- Current sensing device
- Shunt resistor if required
- Supporting circuitry
- MCU communication or ADC connection

### Protection

Investigate or implement:

- Main fuse
- Branch fuses
- Reverse polarity protection
- TVS protection
- Overcurrent protection
- Input transient protection

### Debugging Features

Consider adding:

- Test points
- Status LEDs
- Clearly labeled connectors
- Accessible measurement points

### Deliverables

Each student should provide:

- Complete schematic
- Updated block diagram
- Updated power budget
- Component list
- Datasheets
- Design notes
- Engineering calculations
- Open questions

---

## Design Review 2 - Schematic Review

The team will review the individual schematics subsystem by subsystem.

Instead of comparing entire boards, the team should compare how each student solved each individual problem.

For example:

```text
5 V Regulation
|
├── Student A Solution
├── Student B Solution
└── Student C Solution
        |
        v
Compare
        |
        v
Select Team Approach
``
