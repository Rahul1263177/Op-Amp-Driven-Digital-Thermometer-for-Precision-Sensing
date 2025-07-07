# DIY Digital Thermometer using Op-Amps and BC108 Sensor

This project demonstrates a simple, low-cost **digital thermometer** capable of measuring temperatures up to **150°C** with an accuracy of approximately **±1°C**. The output is displayed on a **1V full-scale deflection (FSD)** analog voltmeter or a **digital voltmeter**.

---

## 🔧 Components Used

- **IC 7805** – Voltage regulator to supply +5V  
- **IC 7660** – Negative voltage generator (–5V)  
- **IC 741 (×2)** – Operational amplifiers for signal amplification  
- **BC108** – NPN transistor acting as the temperature sensor  
- **Variable Resistors**  
  - **VR1 = 100kΩ** – Used for zero calibration  
  - **VR2 = 500kΩ** – Used to set the measurement range  
- **ZD1 (4.7V Zener Diode)** – For voltage clamping  
- **Capacitors** – 10µF and 1µF for filtering  
- **Resistors** – 10kΩ and 100kΩ  
- **Power Source** – 9V Battery or regulated DC supply  
- **Multimeter or Analog Voltmeter** – For output display

---

## ⚙️ Working Principle

- The **BC108 transistor** is used as a temperature sensor.
- The **base-emitter voltage (V<sub>BE</sub>)** of the transistor varies with temperature, approximately –2 mV/°C.
- The first op-amp (IC3) supplies **constant current** and senses the small V<sub>BE</sub> variation.
- The second op-amp (IC4) **amplifies** the signal for a readable analog voltage.
- The output voltage is **linearly proportional** to temperature.
- **VR1** adjusts the **zero reference**, and **VR2** sets the **range** (gain).

---

## 🔌 Circuit Diagram

![Circuit Diagram](circuit.png)


---

## ✅ Features

- Temperature Range: **0°C to 150°C**
- Accuracy: **±1°C**
- Uses **commonly available** components
- Display output via voltmeter: **1V = 100°C** (scalable)
- Compact and ideal for learning analog electronics

---

## 📌 Notes

- You can use a **silicon diode** (like 1N4148) in place of the BC108 transistor.
- The meter used can be **analog** or **digital**.
- Calibration can be done using **ice water** (0°C) and **boiling water** (100°C).

---


