# SSM — Smart Switch Module

**Custom PCB Design | Embedded Systems | Power Electronics | Multi-Board Integration**

Designed by **Junior Kabulo Sungu**, Mechatronics Engineering Student.

## 1. Project Overview

The **Smart Switch Module (SSM)** is an electronics design project focused on the development of a compact power switching system based on custom-designed printed circuit boards (PCBs).

The hardware architecture is divided into two main boards: a power board responsible for the switching circuitry and a control board dedicated to the low-voltage electronics. A multi-board project is used to represent their integration into a single system.

The project covers the electronic design workflow, from schematic capture and component selection to PCB layout, routing, and multi-board assembly, using Altium Designer.

## 2. Hardware Architecture

The repository is organized into three Altium project directories.

### 2.1 SSM_POWER — Power Board

The power board contains the power switching circuitry and associated components.

Key design considerations include:
- High-voltage circuit layout and component placement.
- Power trace sizing and current-carrying capacity.
- Electrical insulation between hazardous-voltage and low-voltage sections.
- PCB manufacturability and assembly constraints.

### 2.2 SSM_CONTROL — Control Board

The control board contains the low-voltage electronics and embedded control circuitry.

Key design considerations include:
- Schematic capture and component integration.
- PCB component placement and routing.
- Control signal routing and interface connections.
- Separation between control electronics and the power section.

### 2.3 PCB_ASSEM_SSM — Multi-Board Assembly

The multi-board project represents the integration of the power and control PCBs.

It supports the visualization and organization of the board-level assembly within the Altium Designer environment.

## 3. PCB Design Considerations

### 3.1 Clearance Distance

**Clearance** is the shortest distance through air between two conductive parts at different electrical potentials.

It helps prevent electrical breakdown through air and must be selected according to working voltage, transient overvoltages, pollution conditions, and other applicable design requirements.

### 3.2 Creepage Distance

**Creepage** is the shortest distance along the surface of an insulating material between two conductive parts.

It helps limit surface leakage and tracking. Its required value depends on factors such as working voltage, pollution degree, and the insulation material's properties.

### 3.3 Power Trace Sizing

PCB copper traces must carry the expected current without exceeding the permitted temperature rise.

Trace width selection depends on copper thickness, current, allowable temperature rise, and whether the trace is on an external or internal layer.

### 3.4 High-Voltage and Low-Voltage Separation

The layout must maintain appropriate separation between hazardous-voltage circuitry and accessible low-voltage electronics.

The design review should consider:
- Clearance and creepage distances.
- Isolation barriers and component placement.
- Routing near board edges, mounting holes, and connectors.
- Enclosure and assembly constraints.

## 4. Design Tools

- **Altium Designer:** Schematic capture, PCB layout, component libraries, and multi-board assembly.
- **Git:** Local version control.
- **GitHub:** Remote repository hosting and project portfolio.

## 5. Repository Structure

```text
SSM-Smart-Switch-Module/
├── SSM_POWER/
│   ├── SSM_POWER.PrjPcb
│   ├── POWER.SchDoc
│   └── PCB_HV.PcbDoc
├── SSM_CONTROL/
│   ├── CONTROL_SSM.PrjPcb
│   ├── MCU.SchDoc
│   └── PCB_LV.PcbDoc
├── PCB_ASSEM_SSM/
│   └── PCB_ASSEM_SSM.PrjMbd
├── Pictures/
└── README.md
```

*Note: The directory tree highlights the main design files. Additional libraries, manufacturing outputs, and supporting documents may also be present in the repository.*

## 6. Design Standards and References

The following standards provide relevant design guidance:

- **IPC-2221 — Generic Standard on Printed Board Design:** General PCB design requirements and layout considerations.
- **IPC-2152 — Standard for Determining Current-Carrying Capacity in Printed Board Design:** Guidance for evaluating conductor current capacity and temperature rise.
- **IEC 60664-1 — Insulation Coordination for Equipment Within Low-Voltage Supply Systems:** Guidance for insulation coordination, including clearance and creepage requirements.

The applicable requirements must be determined from the actual operating conditions, electrical environment, materials, and intended application. Referencing these standards does not, by itself, demonstrate compliance or certification.

## 7. Project Status

This repository contains the current Altium design files, supporting documentation, and visual representations of the PCB assembly.

Electrical validation, design-rule verification, insulation assessment, and manufacturing checks must be completed as applicable before the hardware is used in its intended operating environment.

## 8. Safety Notice

**Warning: The power board may operate at hazardous mains voltage.**

Before applying power, verify the electrical ratings of all components, insulation distances, protective measures, PCB layout, and enclosure requirements. Testing must be performed using appropriate safety procedures and equipment.

This repository is a design project and does not constitute a safety certification.

## 9. Author

**Junior Kabulo Sungu**  
Mechatronics Engineering Student  
Areas of interest: Embedded Systems, Electronic Hardware Design, and PCB Engineering.

GitHub: [Junior-Kabulo](https://github.com/Junior-Kabulo)

## 10. Project Repository

[SSM — Smart Switch Module](https://github.com/Junior-Kabulo/SSM-Smart-Switch-Module)

---

*Designed with Altium Designer.*
