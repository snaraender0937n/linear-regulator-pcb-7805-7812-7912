# Design Calculations

This document includes basic calculations involved in the voltage regulator circuit design.

---

## ⚡ Input Voltage Requirement

For proper regulation:

- 7805 requires input ≥ 7V
- 7812 requires input ≥ 14V
- 7912 requires input ≤ -14V

---

## 🔌 Transformer Selection (if AC used)

For ±12V output:

- Transformer rating ≈ 15V–0–15V (center-tapped) or equivalent
- After rectification:

  V_dc ≈ V_ac × √2

Example:
15V × 1.414 ≈ 21.2V (before losses)

---

## 🔻 Diode Voltage Drop

- Each diode drop ≈ 0.7V
- Bridge rectifier uses 2 diodes per cycle

Total drop:
≈ 1.4V

---

## 🔋 Filter Capacitor Calculation

Formula:

C = I / (f × Vr)

Where:
- C = capacitance
- I = load current
- f = frequency (50Hz → 100Hz after rectification)
- Vr = ripple voltage

Example:
If I = 0.5A and Vr = 1V

C = 0.5 / (100 × 1) = 5000 µF

---

## 🔥 Power Dissipation in Regulator

Formula:

P = (Vin - Vout) × I

Example (7805):
Vin = 12V, Vout = 5V, I = 0.5A

P = (12 - 5) × 0.5 = 3.5W

→ Heat sink required

---

## 📊 Summary

| Parameter            | Value (Example) |
|---------------------|----------------|
| Input Voltage       | 12V–15V        |
| Output Voltages     | +5V, +12V, -12V|
| Capacitor Range     | 1000µF–4700µF  |
| Diode Drop          | ~1.4V          |
| Frequency (India)   | 50Hz           |

---

## 🎯 Conclusion

Proper selection of input voltage, capacitors, and heat management ensures stable and efficient operation of the regulator circuit.
