# 🐭 Micro-mouse Project – Power Subsystem (Group 14)

This repository contains the complete hardware design, testing documentation, and supporting files for the **Power Subsystem** developed by **Group 14** as part of the University of Cape Town’s **EEE3088F Micro-mouse Project**.

The Power Subsystem forms the heart of the Micro-mouse robot, supplying regulated 3.3V and 5V rails, enabling safe LiPo battery charging, driving DC motors, and interfacing cleanly with the Processor and Motherboard modules.

---

## ⚡ System Overview

- **Input Power Sources**: 
  - LiPo Battery (3.7V nominal)
  - USB-C PD input (5V or 9V via CH224K)
- **Outputs**:
  - 3.3V rail (max 300mA)
  - 5V rail (max 1.5A)
  - Bidirectional control of four DC motors via dual H-bridge ICs
  - Battery voltage and current monitoring (INA219 over I2C)
- **Key Features**:
  - Ultra-low standby current mode (<30µA)
  - Manual ON/OFF control (SW2)
  - High-side load switching for external peripherals
  - Compact PCB (82mm x 60mm) with 2x16-pin interface

---

## 📁 Repository Structure
- `/hardware/kicad/` – Full KiCad project files (`.kicad_pro`, `.kicad_sch`, `.kicad_pcb`, etc.)
- `/hardware/production_files/` – Gerbers, BOM, CPL files for JLCPCB submission
