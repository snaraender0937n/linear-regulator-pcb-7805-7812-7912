# Working Explanation of Voltage Regulator Circuit

This document explains the working of the linear voltage regulator circuit using 7805, 7812, and 7912 ICs.

---

## 🔄 Overall Flow

Input → Rectification → Filtering → Regulation → Output

---

## ⚙️ Step-by-Step Working

### 1. Input Stage
The circuit is supplied with either:
- AC voltage (via transformer), or
- Unregulated DC supply

---

### 2. Rectification
- A bridge rectifier converts AC input into pulsating DC.
- It allows current to flow in one direction only.

---

### 3. Filtering
- Capacitors are used to smooth the pulsating DC.
- They reduce ripple and provide a more stable input to the regulators.

---

### 4. Voltage Regulation

#### ➤ 7805 (+5V Regulator)
- Produces a constant +5V output.
- Maintains output despite input or load variations.

#### ➤ 7812 (+12V Regulator)
- Produces a constant +12V output.
- Suitable for higher voltage applications.

#### ➤ 7912 (-12V Regulator)
- Produces a constant -12V output.
- Used in dual power supply systems like op-amps.

---

### 5. Output Stage
- Final outputs are:
  - +5V
  - +12V
  - -12V
- These outputs are stable and ripple-free.

---

## ⚠️ Important Points

- Input voltage must be higher than output voltage.
- Proper polarity must be maintained.
- Heat sinks may be required for high current loads.
- Capacitors should be placed close to regulator pins for stability.

---

## 🎯 Conclusion

The circuit successfully converts an unregulated input into stable multiple DC outputs using linear regulators. It is simple, reliable, and suitable for basic electronic applications.
