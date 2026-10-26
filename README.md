# SSM — Smart Switch Module

**Custom PCB Design | AC Power Switching | Embedded Systems | Altium Designer**

## 1. Project Overview

The **Smart Switch Module (SSM)** is a compact electronic switching system designed around two separate printed circuit boards (PCBs): a high-voltage power board and a low-voltage control board.

The project focuses on PCB design, power and control circuit integration, and multi-board assembly using Altium Designer.

The hardware architecture separates the mains power circuitry from the low-voltage embedded control electronics.

## 2. Hardware Architecture

The design is organized into three Altium project folders:

| Folder | Description |
|---|---|
| `SSM_POWER/` | High-voltage power PCB, schematic, and associated design files |
| `SSM_CONTROL/` | Low-voltage control PCB, microcontroller schematic, and associated design files |
| `PCB_ASSEM_SSM/` | Multi-board assembly project |
| `Pictures/` | PCB layouts, routing views, and assembly renders |

### Power Board — SSM_POWER

The power board contains the mains-side switching circuitry and associated power components.

Main design considerations:
- AC power routing and component placement
- High-voltage insulation distances
- PCB layout and manufacturability
- Separation between hazardous-voltage and low-voltage circuitry

### Control Board — SSM_CONTROL

The control board contains the embedded control electronics and associated low-voltage circuitry.

Main design considerations:
- Microcontroller integration
- Schematic and PCB layout
- Component placement and routing
- Interfaces between the control and power sections

### Multi-Board Assembly — PCB_ASSEM_SSM

The multi-board project is intended to represent the mechanical and electrical integration of the power and control PCBs into a single system.

## 3. Design Tools

- **Altium Designer** — schematic capture, PCB layout, libraries, and multi-board assembly
- **Git / GitHub** — version control and project documentation

## 4. Repository Structure

```text
SSM-Smart-Switch-Module/
├── SSM_POWER/
├── SSM_CONTROL/
├── PCB_ASSEM_SSM/
├── Pictures/
└── README.md
```

The project folders contain the native Altium design files and supporting documents. The `Pictures/` folder contains visual documentation of the PCB layouts and assembly.

## 5. PCB Design Considerations

The design requires particular attention to:

- **Creepage distance:** the shortest distance along an insulating surface between conductive parts.
- **Clearance distance:** the shortest distance through air between conductive parts.
- **Power routing:** conductor width and copper temperature rise under load.
- **Electrical isolation:** separation of mains-voltage circuitry from accessible low-voltage circuitry.
- **Manufacturability:** component footprints, routing, soldering access, and board assembly.

Relevant design references include:

- **IPC-2221** — Generic Standard on Printed Board Design.
- **IPC-2152** — Guidance for determining current-carrying capacity and conductor temperature rise.
- **IEC 60664-1** — Insulation coordination for equipment within low-voltage systems.

Applicable requirements depend on the operating voltage, overvoltage category, pollution degree, material properties, and intended product use.

## 6. Project Status

This repository contains the current PCB design files, supporting documents, and visual representations of the assembly.

Electrical validation, safety verification, and manufacturing qualification must be performed before the module is used in a real mains-powered application.

## 7. Safety Notice

**Warning: This project involves potentially hazardous mains voltage.**

Do not connect the boards to the mains supply without verifying insulation distances, protective measures, component ratings, enclosure safety, and applicable electrical safety requirements.

The presence of a PCB design in this repository does not constitute certification or proof of safe operation.

## 8. Repository

GitHub: [SSM-Smart-Switch-Module](https://github.com/Junior-Kabulo/SSM-Smart-Switch-Module)

---

Designed with Altium Designer.
