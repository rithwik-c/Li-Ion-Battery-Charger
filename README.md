# Li-Ion Battery Charger Simulation using CC-CV Mode

A MATLAB/Simulink implementation of a **Lithium-Ion Battery Charger** based on the **Constant Current–Constant Voltage (CC-CV)** charging algorithm. The model demonstrates the charging process of a Li-Ion battery while ensuring safe charging by automatically transitioning from constant current to constant voltage mode.

---

##  Overview

Lithium-Ion batteries require a controlled charging profile to maximize battery life, improve efficiency, and prevent overcharging. This project implements the industry-standard **CC-CV charging method** in Simulink using feedback control.

The charger operates in two stages:

- **Constant Current (CC):** Charges the battery at a fixed current until the battery voltage reaches its maximum charging voltage.
- **Constant Voltage (CV):** Maintains a constant battery voltage while the charging current gradually decreases until the battery is fully charged.

---

##  Features

- Closed-loop Buck Converter
- CC-CV charging algorithm
- Automatic mode transition (CC → CV)
- PI Controller for voltage/current regulation
- PWM-based switching control
- Real-time monitoring of battery voltage and charging current
- Simulink implementation suitable for learning and research

---

##  Working Principle

### Constant Current (CC) Mode

- The controller regulates the converter to supply a constant charging current.
- Battery voltage increases gradually as charging progresses.

### Constant Voltage (CV) Mode

- Once the battery reaches its rated charging voltage, the controller maintains a constant output voltage.
- Charging current naturally tapers off until it reaches the termination level.

---



##  Expected Results

The simulation demonstrates:

- Constant charging current during the initial charging stage
- Gradual increase in battery voltage
- Smooth transition from CC mode to CV mode
- Decreasing charging current during CV mode
- Stable battery terminal voltage at the end of charging

---

##  Applications

- Battery Management Systems (BMS)
- Electric Vehicle (EV) Chargers
- Portable Electronics
- Renewable Energy Storage Systems

---

##  Future Improvements

- Temperature-dependent charging
- State of Charge (SOC) estimation
- State of Health (SOH) estimation
- Cell balancing for battery packs
- Fast charging techniques
- Hardware implementation using embedded controllers


## 👨‍💻 Author

**Rithwik Chander**

---

## 📄 License

This project is intended for educational and research purposes.
