# Hi, I'm Durrice Léa Tahoc Wokam 👋

**Computer Engineering** undergraduate student at the Université du Québec en Outaouais (UQO), Canada.
I'm interested in **FPGA digital design**, **embedded systems** and **hardware/software integration**.

## 🔧 Skills

| Area | Tools and technologies |
|---|---|
| Digital design | VHDL, finite state machines, UART, Intel Quartus Prime, Cyclone V (DE1-SoC) |
| Verification | VHDL testbenches, Questa / ModelSim |
| Embedded | Arduino (C/C++), sensor acquisition, PWM motor control, interrupts, servomotors |
| Instrumentation | Experimental calibration, statistical analysis of measurements |
| Documentation | Technical writing, keeping documentation consistent with the implementation |

## 📌 Featured projects

### [DC Motor Monitoring — Arduino + FPGA](https://github.com/AnonymousCandela/surveillance-moteur-fpga)

Real-time embedded system that classifies a DC motor's condition as **NORMAL**, **DEGRADED** or **FAULT** from its speed and current.

- Full FPGA pipeline in VHDL: UART reception, frame decoding and checksum validation, threshold classifier, state transmission.
- State changes confirmed over 3 consecutive measurements, while faults are applied immediately for safety.
- 115,200 baud UART link between an Arduino Mega 2560 (5 V) and a DE1-SoC board (3.3 V).

*GEN5001 internship · UQO · Summer 2026*
*Project documentation is in French.*

### [Obstacle-Avoiding Robot — Arduino Uno](https://github.com/AnonymousCandela/Robot.Eviteur.d-obstacles)

Autonomous mobile robot that detects obstacles and reacts to avoid collisions.

- Distance measurement with an HC-SR04 ultrasonic sensor mounted on a scanning servo.
- Dual DC motor control through an L298N H-bridge with PWM speed control.
- Wiring diagram, demo video and full project report included.

*INF1643 Computer Architecture II · UQO · Winter 2024 · Team of two*
*Project documentation is in French.*

## 🌐 Languages

French · English
