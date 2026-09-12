# BMS_GAR
Battery Management System & Power Distribution Board for the GAR Autonomous Vehicle Platform

## Overview

The BMS_GAR project aims to develop a custom power distribution and battery monitoring solution for the GAR autonomous vehicle platform. The board will serve as the central power hub of the vehicle, safely distributing power from the battery to all electrical subsystems while providing monitoring, protection, and diagnostic capabilities.

The primary objective of Revision 1 is to establish a reliable electrical backbone that enables safe operation, efficient power distribution, and future expandability as the vehicle platform grows.

---

# Project Objectives

## Power Distribution
- Distribute battery power to all vehicle electronics
- Generate regulated voltage rails for onboard systems
- Provide power connectors for future expansion
- Maintain reliable operation under vehicle load conditions

## Battery Monitoring
- Monitor pack voltage
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

---

# Team Structure

## Student 1 — Battery & Requirements Lead

### Responsibilities
- Battery research and selection
- Vehicle runtime estimation
- Current consumption analysis
- System voltage requirements
- Battery connector selection
- Wiring requirements

### Deliverables
- Battery Selection Report
- Power Budget Spreadsheet
- Runtime Analysis
- Electrical Requirements Document

---

## Student 2 — Protection & Safety Lead

### Responsibilities
- Fuse selection
- Reverse polarity protection research
- TVS protection research
- Fault detection architecture
- Emergency stop integration
- Power safety recommendations

### Deliverables
- Protection Circuit Proposal
- Safety Requirements Document
- Component Selection Report
- Fault Management Plan

---

## Student 3 — PCB Design Lead

### Responsibilities
- KiCad project management
- Schematic capture
- Symbol and footprint verification
- PCB layout
- Connector placement
- Design reviews
- Manufacturing file generation

### Deliverables
- Complete KiCad Project
- Schematics
- PCB Layout
- Fabrication Files
- Assembly Documentation

---

# System Architecture

```text
Battery Pack
      |
      v
+----------------------+
| Power Distribution   |
|       Board          |
+----------------------+
      |
      +---- Voltage Monitoring
      |
      +---- Current Monitoring
      |
      +---- Protection Circuitry
      |
      +---- 5V Rail
      |
      +---- 3.3V Rail
      |
      +---- Vehicle Electronics
```

---

# Revision 1 Scope

## Electrical Features
- Battery input connector
- Main fuse
- Reverse polarity protection
- Current sensing
- Voltage sensing
- 5V regulator
- 3.3V regulator
- Status LEDs
- Expansion connectors

## Design Goals
- Reliable power delivery
- Modular architecture
- Easy debugging and testing
- Manufacturable PCB layout
- Future expansion support

---

# Future Development

## Battery Monitoring Expansion
Potential future additions:
- Battery State of Charge estimation
- Temperature monitoring
- Cell balancing
- Battery health diagnostics

## Safety Expansion
Potential future additions:
- Dedicated safety board
- Independent watchdog systems
- Automatic fault shutdown
- Advanced fault reporting

## Telemetry Expansion
Potential future additions:
- Wireless telemetry
- Data logging
- Remote diagnostics
- CAN bus integration

---

# Repository Structure

```text
BMS_GAR/
│
├── Hardware/
│   ├── Schematics/
│   ├── PCB/
│   ├── Manufacturing/
│   └── Libraries/
│
├── Documentation/
│
├── Testing/
│
├── Resources/
│   ├── Datasheets/
│   └── References/
│
└── Project_Management/
```

---

# Success Criteria

A successful Revision 1 board will:

- Safely distribute power throughout the vehicle
- Regulate required voltage rails
- Monitor battery voltage and current
- Provide basic fault protection
- Support integration with the vehicle control system
- Establish a foundation for future power system development

---

## Project Vision

The BMS_GAR project will provide the electrical backbone of the GAR autonomous vehicle platform while giving team members hands-on experience in power electronics, battery systems, PCB design, system architecture, testing, validation, and engineering collaboration.
