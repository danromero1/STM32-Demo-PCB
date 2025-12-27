# STM32 Demo PCB

![KiCAD](https://img.shields.io/badge/KiCAD-2--Layer-314CB0?style=flat-square&logo=kicad&logoColor=white)
![Status](https://img.shields.io/badge/status-Design%20Complete-green.svg)
![Year](https://img.shields.io/badge/year-2023-blue.svg)

My first end-to-end PCB design project - An STM32F103C8T6 development board for learning microcontroller hardware implementation and PCB design fundamentals.

---

## Overview

This project was my introduction to professional PCB design practices and microcontroller hardware implementation. The board features an STM32F103C8T6 MCU with external crystal oscillator, voltage regulation, and USB interface for programming and power delivery. The entire design was created in KiCAD following industry best practices for decoupling, signal routing, and design-for-manufacturability.

**Purpose:** Learn foundational PCB design skills and microcontroller hardware implementation  
**Outcome:** Complete 2-layer board design with manufacturing-ready Gerber files  
**Year:** 2023

---

## Design Features

**Microcontroller**
- STM32F103C8T6 (ARM Cortex-M3, 72 MHz)
- External 16 MHz crystal oscillator with load capacitance matching
- SWD/debug header for programming and debugging
- Boot mode selection

**Power Management**
- AMS1117-3.3V linear voltage regulator
- USB-powered (5V input)
- Ferrite bead filtering on VDDA (analog supply)
- Comprehensive decoupling capacitor network

**Interfaces**
- USB interface for programming and power
- SWD/JTAG debug header
- GPIO breakout headers
- I2C, SPI, UART accessible via headers

**PCB Design**
- 2-layer board layout
- Proper ground plane implementation
- Signal routing with impedance awareness
- ERC/DRC verification passed

---

## Technical Skills Demonstrated

**Schematic Design**
- Microcontroller peripheral connections
- Crystal oscillator design with load capacitance calculation
- Power supply design and voltage regulation
- USB interface implementation
- Reset and boot configuration circuits

**PCB Layout**
- Component placement optimization
- Signal routing and trace width selection
- Ground plane design and via placement
- Decoupling capacitor placement near power pins
- SWD/debug header routing
- Pick-and-place file generation

**Design Verification**
- Electrical Rule Check (ERC) compliance
- Design Rule Check (DRC) compliance
- Schematic-to-layout verification

---

## Design Process

### 1. Schematic Capture
Referenced STM32F103C8T6 datasheet and application notes to create a complete schematic including power, reset, clock, and USB circuitry.

### 2. Component Selection
- Selected AMS1117-3.3V for stable voltage regulation
- Calculated crystal load capacitors for 16 MHz oscillator
- Chose ferrite beads for analog/digital supply isolation

### 3. PCB Layout
- Created 2-layer stackup (signal/ground)
- Placed components with signal flow in mind
- Routed high-speed signals (USB, crystal) first
- Implemented ground plane with proper stitching vias
- Added silkscreen labels for all connectors

### 4. Manufacturing Preparation
- Generated Gerber files (RS-274X format)
- Created drill files and pick-and-place data
- Verified design against manufacturer capabilities

---

## Technical Specifications

**Microcontroller:** STM32F103C8T6 (ARM Cortex-M3, 72 MHz, 64KB Flash, 20KB RAM)  
**Clock:** 16 MHz external crystal oscillator  
**Power Input:** 5V via USB  
**Regulated Output:** 3.3V (AMS1117)  
**PCB:** 2-layer, standard FR4    
**Connector:** USB Type-B (or mini/micro - specify if known)

---

## Learning Outcomes

This project provided hands-on experience with:

**Hardware Design**
- STM32 microcontroller architecture and peripherals
- Clock circuitry and crystal oscillator design
- Power supply design and voltage regulation
- USB hardware implementation

**PCB Design Fundamentals**
- Schematic capture and component selection
- PCB layout and routing techniques
- Ground plane design and EMI mitigation
- Manufacturing file generation and validation
- Design rule verification (DRC/ERC)

**Professional Practices**
- Reading and interpreting datasheets
- Following application note guidelines
- Design-for-manufacturability principles
- Version control and documentation

---

## Project Files

- **Schematic:** Complete schematic design in KiCAD format
- **PCB Layout:** 2-layer board layout with ground plane
- **Gerber Files:** Manufacturing-ready RS-274X format

---

## Design Tools

- **KiCAD 6** - Schematic capture and PCB layout
- **Datasheets** - STM32F103C8T6, AMS1117, USB specifications
- **Application Notes** - STMicroelectronics hardware design guidelines

---

## Lessons Learned

**What Went Well:**
- Clean schematic organization and hierarchical design
- Proper decoupling capacitor placement
- Successful DRC/ERC verification


**Future Improvements:**
- Consider 4-layer stackup for better power distribution
- Add test points for critical signals
- Include LED indicators for power and status
- Optimize component placement for hand assembly

---

## Connection to Future Work

This project laid the foundation for more advanced designs:
- **Mixed-Signal Guitar Effects Pedal** - Applied layout techniques learned here to 4-layer mixed-signal design
- **Embedded Systems Projects** - Understanding of microcontroller hardware fundamentals
- **Power Supply Design** - Experience with voltage regulation and decoupling

The skills gained from this first PCB design directly enabled more complex projects involving high-speed signals, mixed-signal design, and multi-layer boards.

---

## Status

**Design Status:** Complete  
**Manufacturing:** Not fabricated (design exercise)  
**Testing:** N/A  
**Future Plans:** Foundational project - skills applied to advanced designs

---

## Contact

**Daniel Romero**  
Email: daniel.romero@ieee.org  
Portfolio: [electricalromero.com](https://electricalromero.com)  
LinkedIn: [linkedin.com/in/daniel-romero-ee](https://www.linkedin.com/in/daniel-romero-ee/)

---

*This was my first complete PCB design project, serving as a practical introduction to hardware design and manufacturing practices.*

*Last Updated: December 2024*
