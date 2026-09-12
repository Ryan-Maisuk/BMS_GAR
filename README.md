# BMS_GAR
Battery Management Board
# BMS_GAR
Battery Management System Board for the GAR Autonomous Vehicle Platform

## Overview

The BMS_GAR project aims to develop a custom Battery Management System (BMS) and power distribution board for the GAR autonomous vehicle platform. 
The board will safely monitor, protect, and distribute power from the vehicle battery to all vehicle electronics while providing real-time telemetry and fault 
monitoring.

The primary goal of Revision 1 is to establish a reliable electrical backbone for the vehicle, enabling safe battery operation, system monitoring, and regulated 
power delivery.

---

## Objectives

### Battery Monitoring
- Pack voltage monitoring
- Current measurement
- Remaining battery estimation
- Battery health diagnostics

### Power Distribution
- Deliver regulated power to all vehicle electronics
- Support motor controller power requirements
- Support sensor and embedded systems power requirements
- Provide protected auxiliary power outputs

### Safety
- Reverse polarity protection
- Fuse protection
- Under-voltage protection
- Over-current protection
- Emergency shutdown support

---

## System Architecture

```text
Battery Pack
      |
      v
Protection Circuitry
      |
      v
Current / Voltage Monitoring
      |
      +----> STM32 Control Board
      |
      +----> Sensors
      |
      +----> ESC
      |
      +----> Auxiliary Electronics
