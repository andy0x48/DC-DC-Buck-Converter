# DC-DC Buck Converter

## Overview
This project focuses on designing, simulating, and testing a **DC-DC buck converter** that steps down **12V to 5V** with a **2A output**. The project follows an **industry-standard approach**, including:
- **LTSpice Simulation**
- **PCB Design using KiCad/Altium**
- **Prototype Fabrication & Testing**
- **Power Efficiency & Ripple Analysis**

---

## Project Specifications

| Parameter            | Value  |
|----------------------|--------|
| **Input Voltage**    | 12V    |
| **Output Voltage**   | 5V     |
| **Output Current**   | 2A     |
| **Power Output**     | 10W    |
| **Efficiency Goal**  | >85%   |
| **Switching Frequency** | 150kHz - 500kHz |
| **Topology**        | Buck Converter |

---

## Component Selection

### **Main Controller IC**
| Component | Part Number | Comment |
|-----------|------------|---------------------|
| **DC-DC Regulator IC** | LM2675-5.0 | High efficiency, integrated switch, 5V fixed output |

### **Passive Components**
| Component | Value | Comment |
|-----------|-------|---------|
| **Inductor** | 47µH | Filters ripple, stores energy |
| **Input Capacitor** | 100µF | Reduces input noise |
| **Output Capacitor** | 330µF | Minimizes output ripple |
| **Schottky Diode** | 1N5822 | Fast recovery, low losses |

### **Power Components**
| Component | Part Number | Function |
|-----------|------------|----------|
| **MOSFET (if needed)** | IRF540N | Low R_DS(on) switch |
| **Diode** | 1N5822 | High-speed rectifier |

---

## LTSpice Simulation Results
> [!NOTE]
> This section is a work in progress.

### **Voltage Regulation**

- Looking for **Steady 5V output** with minimal deviation.
- Looking for **Voltage ripple < 50mV** under load.

---

## Bill of Materials (BOM)

| Component | Part Number | Quantity | Source |
|-----------|------------|----------|--------|
| **LM2675-5.0** | DC-DC Converter | 1 | Digi-Key |
| **Inductor** | 47µH | 1 | Mouser |
| **Capacitors** | 100µF, 330µF | 2 | LCSC |
| **Diode** | 1N5822 | 1 | Digi-Key |
| **MOSFET** | IRF540N | 1 | Mouser |
| **PCB Fabrication** | JLCPCB | 1 | JLCPCB |

---
