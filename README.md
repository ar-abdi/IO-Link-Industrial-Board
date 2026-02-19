# IO-Link Industrial Communication Board
Multi-revision industrial IO-Link master platform with on-board Ethernet and STM32H5 hardware integration.

## Overview

This repository documents the iterative development of an industrial IO-Link communication board integrated with on-board Ethernet connectivity and STM32H5 hardware control.

The project evolved through three major hardware revisions to address physical layer reliability, wake-up timing determinism, and ecosystem maturity concerns.

Firmware and protocol stack implementation are handled by the software team. This repository focuses exclusively on hardware architecture, PCB design, and system-level integration.

---

## System Architecture

The board integrates:

- IO-Link Master interface
- STM32H5 microcontroller (hardware integration)
- On-board Ethernet interface
- Industrial 24V power domain
- 3.3V regulated subsystem

The design emphasizes deterministic wake behavior, signal integrity, and robust power routing.

---

## Revision History

### Version 1 – LTC2874 Based
- Inherited legacy hardware design from senior member of the same organisation
- Identified wake-up timing instability
- Refined signal routing and protection topology
- Improved grounding strategy

---

### Version 2 – CCE4511CA Based
- Re-architected IO-Link interface
- Schematic completed
- Project discontinued due to limited ecosystem maturity and software integration risk

---

### Version 3 – MAX14819 Based (Current)
- Selected due to mature ecosystem support
- Integrated framing and improved timing handling
- Improved hardware determinism
- Currently under software integration

---

## On-Board Ethernet Interface

The board includes integrated Ethernet connectivity to allow communication within a larger robotic subsystem network.

Hardware responsibilities included:
- Differential pair routing
- Magnetics integration
- Impedance-aware layout
- Structured ground partitioning

---

## Tools Used

- Altium Designer
- Multi-layer PCB Layout
- Datasheet-Driven Hardware Design
