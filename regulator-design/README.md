# Voltage Regulator Design (7805, 7812, 7912)

This module focuses on the design and implementation of a multi-output linear voltage regulator circuit. The system generates +5V, +12V, and -12V regulated outputs using standard 78xx and 79xx series ICs.

---

## 🔧 Objective

To design a stable DC power supply capable of providing multiple voltage levels required for analog and digital electronic circuits.

---

## ⚙️ Circuit Overview

The regulator circuit consists of the following stages:

1. **Input Supply**
   - AC input (via transformer) or unregulated DC input

2. **Rectification**
   - Bridge rectifier converts AC to pulsating DC

3. **Filtering**
   - Capacitors smooth the DC signal and reduce ripple

4. **Voltage Regulation**
   - 7805 → +5V output
   - 7812 → +12V output
   - 7912 → -12V output

---

## 🔌 Regulator IC Details

### 1. 7805 (+5V Regulator)
- Fixed output: +5V
- Used for microcontrollers and digital circuits
- Requires input voltage > 7V

### 2. 7812 (+12V Regulator)
- Fixed output: +12V
- Used in analog circuits and relays
- Requires input voltage > 14V

### 3. 7912 (-12V Regulator)
- Fixed output: -12V
- Used for dual power supply applications (op-amps)
- Requires negative input voltage

---

## 🔄 Working Explanation

- The input voltage is first converted into DC using rectification.
- Capacitors filter out ripples to produce a smoother DC signal.
- Each regulator IC maintains a constant output voltage despite variations in input voltage or load.
- The 79xx series regulator (7912) provides negative voltage, enabling dual supply systems.

---

## 📁 Contents of This Module

- `schematics/` → Circuit diagrams of regulators
- `pcb/` → PCB layout and 3D visualization
- `simulation/` → Output waveform/graphs
- `docs/` → Detailed explanation and calculations
- `results/` → Measured outputs

---

## 📊 Output Summary

| IC    | Output Voltage | Application                |
|------|--------------|----------------------------|
| 7805 | +5V          | Digital circuits           |
| 7812 | +12V         | Analog / general purpose   |
| 7912 | -12V         | Dual supply systems        |

---

## ⚠️ Design Considerations

- Heat dissipation in regulators (use heat sinks if needed)
- Proper capacitor placement for stability
- Input voltage must be sufficiently higher than output voltage
- Ensure correct polarity, especially for 7912

---

## 🎯 Learning Outcomes

- Practical understanding of linear regulators
- Multi-output power supply design
- Handling positive and negative voltage regulation
- PCB design implementation

---

## 🚧 Status

Design files and simulation outputs are included. Further improvements and documentation will be added.
