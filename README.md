# Analog Programmable Electronic Load
Constant Current (CC) and Constant Resistance (CR) Modes

## About the Project
The Analog Programmable Electronic Load is designed to test and evaluate DC power sources such as batteries, DC power supplies, and DC-DC converters.

Unlike conventional resistive loads, which provide a fixed resistance, an electronic load allows the user to electronically control the amount of current drawn from a power source.

This project implements two operating modes: Constant Current (CC) and Constant Resistance (CR). The system uses an analog feedback-control approach to regulate the load current without requiring a microcontroller or software-based control.

The main objective is to develop a programmable and adjustable electronic load that provides flexible loading conditions for testing and characterizing DC power sources.

## Key Features
- Constant Current (CC) operating mode.
- Constant Resistance (CR) operating mode.
- Adjustable current and resistance settings.
- Analog closed-loop feedback control.
- MOSFET-based electronic load regulation.
- Input-voltage and load-current monitoring.
- Manual selection between operating modes.
- MATLAB Simulink-based modeling and simulation.
- No microcontroller or digital programming required.
  
## Working Principle
The electronic load operates by controlling the conduction of a power MOSFET to regulate the current drawn from an external DC source.

A current-sensing circuit continuously monitors the load current and generates a corresponding feedback voltage. The analog control circuit compares this feedback signal with a reference voltage and adjusts the MOSFET gate drive accordingly.

This process creates a closed-loop feedback system that automatically regulates the load current based on the selected operating mode.
Constant Current (CC) Mode
In Constant Current mode, the electronic load maintains a predefined current regardless of variations in input voltage, within its operating limits.

This mode is useful for evaluating the current-delivering capability and voltage regulation of DC power supplies and batteries.
Constant Resistance (CR) Mode
In Constant Resistance mode, the electronic load behaves approximately like a programmable resistor.

For example, when the selected resistance is 10 Ω, an input voltage of 5 V produces an ideal load current of 0.5 A.

This mode is useful for evaluating the behavior of power sources under different resistive loading conditions.

## MATLAB Simulink Modeling and Simulation
MATLAB Simulink is used to model and simulate the proposed analog electronic load before its hardware implementation.

The Simulink model represents the electrical behavior and feedback-control operation of the system. It provides a simulation environment to study the relationship between input voltage, load current, MOSFET control, and the selected operating mode.

The model incorporates functional blocks representing the DC input source, MOSFET load stage, current-sensing section, analog control system, reference signals, and switching arrangement.

## Simulation Objectives
- Analyze the overall operation of the electronic load.
- Study the Constant Current mode under different input-voltage conditions.
- Examine the Constant Resistance mode and its voltage-current relationship.
- Observe the response of the feedback-control system.
- Analyze the effect of changing reference settings.
- Monitor input voltage, load current, and power behavior.
- Evaluate the system's response under different loading conditions.
  
## CC Mode Simulation
In CC mode, the simulation examines whether the load current remains approximately constant as the input voltage changes.

The reference signal determines the target current, while the feedback loop adjusts the MOSFET control signal to minimize the difference between the desired and measured current.

## CR Mode Simulation
In CR mode, the simulation examines how the load current changes with input voltage for a selected equivalent resistance.

The control reference is designed to vary proportionally with the input voltage, allowing the system to reproduce resistive loading behavior.

## Simulation Analysis
The simulation provides a way to examine:
- Input voltage characteristics.
- Load-current response.
- Equivalent resistance.
- MOSFET control behavior.
- Feedback response in CC and CR modes.
- Power dissipation in the load stage.
The simulation model also serves as a reference for understanding the intended hardware architecture and evaluating the relationship between theoretical calculations and practical circuit behavior.

## Applications
- Testing and characterization of DC power supplies.
- Battery discharge and performance testing.
- DC-DC converter evaluation.
- Solar power system testing.
- Current-delivering capability analysis.
- Voltage regulation testing.
- Power electronics laboratory experiments.
- Analog feedback-control demonstrations.
  
## Advantages
- Fully analog control without a microcontroller.
- Supports two different loading modes.
- Adjustable loading conditions.
- Closed-loop current regulation.
- Useful for practical power-source characterization.
- Combines simulation and hardware-based circuit design.
- Demonstrates the application of analog feedback in power electronics.
  
## Future Scope
- Integration of digital voltage and current displays.
- Improved measurement accuracy.
- Automatic overcurrent and overtemperature protection.
- PCB-based implementation.
- Higher voltage and power capability through an appropriately redesigned power stage.
- Data acquisition and performance monitoring.
- Enhanced simulation and experimental comparison.
  
## Conclusion
The Analog Programmable Electronic Load demonstrates the application of analog electronics, power MOSFET operation, current sensing, and closed-loop feedback control in developing a flexible DC loading system.

By supporting Constant Current and Constant Resistance modes, the proposed system provides two different methods of evaluating DC power sources. MATLAB Simulink modeling complements the hardware design by providing a platform to study circuit behavior and analyze the intended control characteristics.

The project combines analog circuit design, power electronics, feedback control, and simulation into a practical electronic testing instrument.
