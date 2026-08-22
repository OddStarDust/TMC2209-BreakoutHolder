# TMC2209-BreakoutHolder
TMC2209 plug and play breakout board. The porpuse of this pcb is to make an easy way to test stepper drivers

[![License: CERN-OHL-W-v2](https://img.shields.io/badge/License-CERN--OHL--W--v2-blue.svg)](https://ohwr.org/cern_ohl_w_v2.txt)
[![Hardware: KiCad 8+](https://img.shields.io/badge/KiCad-8.0%2B-blue)](https://www.kicad.org/)
[![Status: Production Ready](https://img.shields.io/badge/Status-Production%20Ready-brightgreen)](#)

An ultra-compact, high-reliability breakout board designed for **TMC2209**, **A4988**, and **DRV8825** stepper driver modules (standard StepStick footprint). Engineered for 3D printers, CNC machinery, and custom robotics projects requiring secure connections and transient voltage protection.

---

## 📸 Overview & Rendering

| Board Top View | 3D Render |
| :---: | :---: |
| ![Top View](docs/topview.png) | ![3D Render](docs/schematics.png) |

---

## ✨ Key Features

* **Voltage Spike Protection (VMOT):** Integrated footprint for a $100\\mu\\text{F} / 35\\text{V}$ decoupling electrolytic capacitor to absorb back-EMF spikes and preserve driver life.
* **Secure Interconnects:** Utilizes standard **JST connectors** (2-pin power/signals, 4-pin motor coil) to prevent accidental disconnects during high-vibration operation.
* **Universal StepStick Socket:** Compatible with standard 2.54mm header StepStick drivers (TMC2209, A4988, DRV8825, etc.).
* **Turnkey Manufacturing Ready:** Includes pre-configured Gerber, Drill, BOM, and CPL files tested for 1-click fabrication on **JLCPCB** and **PCBWay**.
* **Clean Signal Routing:** Designed with optimized ground planes and thermal relief pads for easy manual or automated soldering.

---

## 📐 Pinout & Connection Diagram

```text
               +-----------------------+
               |     TMC2209 DRIVER    |
               |       SOCKETS         |
               +-----------------------+
              /                         \\
   [VMOT / GND]                          [STEP / DIR / EN]
  (2-Pin JST Input)                     (2.54mm Header Pins)
              \\                         /
               +-----------------------+
               |   MOTOR COILS (4-Pin) |
               +-----------------------+
