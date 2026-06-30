Li-Ion Battery Charger Simulation using CC-CV Control (Simulink)

A MATLAB/Simulink model of a Lithium-Ion Battery Charger implementing the Constant Current–Constant Voltage (CC-CV) charging algorithm using a closed-loop buck converter.

The simulation demonstrates the complete charging process, where the battery is initially charged at a constant current and automatically transitions to constant voltage mode as the battery reaches its rated voltage.

Overview

Lithium-Ion batteries require a controlled charging strategy to ensure:

Safe operation
Longer battery life
Higher charging efficiency
Prevention of overcharging

This project implements the industry-standard CC-CV charging method using a DC-DC buck converter regulated through closed-loop control.

Features
🔋 Closed-loop Li-Ion battery charger
⚡ Buck converter topology
🔄 Automatic transition between CC and CV modes
🎯 PI controller-based voltage/current regulation
📈 Real-time monitoring of:
Battery Voltage
Charging Current
State of Charge (SOC)
Converter Output
Charging Algorithm
1. Constant Current (CC) Mode
The charger supplies a fixed charging current.
Battery voltage gradually increases.
This mode provides fast charging while keeping current within safe limits.
2. Constant Voltage (CV) Mode
Once the battery reaches its rated voltage, the charger switches to constant voltage mode.
Output voltage is maintained at the battery's maximum charging voltage.
Charging current gradually decreases until it reaches the termination threshold.

This charging profile closely follows the charging methodology used in commercial Li-Ion battery chargers.

Simulation Components
DC Input Source
Buck Converter
PWM Generator
PI Controller
Feedback Control System
Li-Ion Battery Model
Voltage & Current Measurement Blocks
Scope Blocks for waveform visualization
Control Strategy

The controller continuously measures the battery voltage and current and adjusts the PWM duty cycle of the buck converter.

During CC mode:
Current is regulated to the reference charging current.
During CV mode:
Voltage is regulated to the battery's rated charging voltage.

The controller automatically transitions between both modes without user intervention.

Expected Results

The simulation demonstrates:

Constant charging current during the initial charging stage.
Smooth rise in battery voltage.
Automatic switching from CC mode to CV mode.
Gradual reduction in charging current during CV mode.
Stable battery terminal voltage throughout the final charging stage.
Software Requirements
MATLAB
Simulink
Simscape Electrical (recommended)
Simscape Power Systems (if applicable)
Repository Structure
.
├── Simulation.slx
├── README.md
└── Images/            (optional screenshots)
Applications
Battery Management Systems (BMS)
Electric Vehicle (EV) Chargers
Portable Electronics
Renewable Energy Storage Systems
Power Electronics Education
Future Improvements
Temperature-dependent charging
Cell balancing for battery packs
State of Charge (SOC) estimation
State of Health (SOH) estimation
Fast charging algorithms
Hardware implementation using embedded controllers
License

This project is intended for educational and research purposes.

Author

Rithwik Chander

Suggested screenshots to include in your GitHub repository

To make the repository more attractive, add screenshots of:

Simulink model overview
Buck converter subsystem
Battery voltage waveform
Charging current waveform
CC to CV transition waveform
State of Charge (SOC) curve
