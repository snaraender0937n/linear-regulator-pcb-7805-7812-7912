# Linear Voltage Regulator PCB (7805, 7812, 7912)

This repository presents the design, simulation, and implementation of a linear voltage regulator PCB developed during a PCB workshop. The circuit provides stable DC outputs of +5V, +12V, and -12V using standard linear regulator ICs.

---

## 🔌 Project Overview

The objective of this project is to design a regulated power supply capable of delivering multiple voltage levels from a single input source. The system uses:

- **7805** → +5V output  
- **7812** → +12V output  
- **7912** → -12V output  

The project demonstrates the complete workflow from circuit design to PCB fabrication and output verification.

---

## ⚙️ Working Principle

1. **Input Stage**  
   An AC or unregulated DC input is provided to the circuit.

2. **Rectification (if AC input is used)**  
   A bridge rectifier converts AC to DC.

3. **Filtering**  
   Capacitors are used to smooth the rectified voltage and reduce ripple.

4. **Voltage Regulation**  
   - 7805 regulates output to +5V  
   - 7812 regulates output to +12V  
   - 7912 regulates output to -12V  

5. **Output Stage**  
   Stable DC voltages are obtained for use in electronic circuits.

---

## 🧩 Components Used

- 7805 Voltage Regulator
- 7812 Voltage Regulator
- 7912 Voltage Regulator
- Diodes (for rectification)
- Capacitors (input and output filtering)
- Transformer (if AC input is used)
- PCB board
- Connectors / terminals

---

## 📁 Repository Structure

```
regulator-design/   → Circuit, PCB, simulation, and documentation
pcb-etching/        → Manual PCB fabrication using ferric chloride
```

---

## 📊 Expected Output

| Regulator | Output Voltage |
|----------|--------------|
| 7805     | +5V          |
| 7812     | +12V         |
| 7912     | -12V         |

---

## 🧪 Results

The designed PCB successfully provides regulated voltage outputs with minimal ripple, suitable for low-power electronic applications.

---

## 🎯 Learning Outcomes

- Understanding of linear voltage regulators (78xx & 79xx series)
- PCB design and layout fundamentals
- Power supply design basics
- Practical exposure to hardware fabrication

---

## 🚧 Future Improvements

- Add complete PCB images and Gerber files  
- Include detailed calculations and simulations  
- Improve efficiency using switching regulators  

---

## 📌 Status

Documentation is being updated. Additional files and images will be added soon.
