# Closed-Loop DC Traction Motor Control & Fault Simulation

## Project Overview
This repository contains the schematic and simulation files for a robust, closed-loop DC traction motor drive. Designed to mimic real-world electric train operations, the electromechanical system is modeled in **Ngspice** using behavioral dependent sources to represent mechanical parameters like train mass, inertia, and rolling resistance. 

A DC Chopper (Buck Converter) integrated with an active **PID controller** provides precise speed regulation. The system dynamically adjusts the PWM duty cycle to maintain constant speed despite simulated mechanical loads, gradient changes, and electrical faults.

## Key Features
* **Electromechanical Co-Simulation:** Accurate modeling of both electrical (Armature resistance/inductance, Back EMF) and mechanical dynamics (Mass, Inertia) using Ngspice behavioral voltage/current sources.
* **Closed-Loop Speed Regulation:** Active PID feedback loop adjusting PWM logic to counteract load variations.
* **Dynamic Fault Simulation:** Built-in test cases for real-world stress conditions:
  * Variable gradient slopes (variable load torque)
  * Start-stop acceleration/deceleration cycles
  * Short circuit and open armature faults
  * Sudden braking impacts
* **Performance Analysis:** Granular observation of current spikes, voltage sags, and system recovery times.

## Tools & Technologies
* **Circuit Design & Schematic:** KiCad
* **Simulation Engine:** Ngspice
* **Control Logic:** Custom PID & PWM behavioral modeling
