# Hi, I'm Durrice Léa Tahoc Wokam 

**Computer Engineering** undergraduate student at the Université du Québec en Outaouais (UQO), Canada.
I'm interested in **FPGA digital design**, **embedded systems** and **hardware/software integration**.

##  Skills

| Area | Tools and technologies |
|---|---|
| Digital design | VHDL, finite state machines, UART, Intel Quartus Prime, Cyclone V (DE1-SoC) |
| ASIC flow | RTL-to-GDS, Cadence Genus (synthesis), Cadence Innovus (place & route), SDC timing constraints, TSMC 65 nm |
| Verification | VHDL / Verilog testbenches, gate-level simulation with SDF back-annotation, NCSim / SimVision, Questa / ModelSim |
| Embedded | Arduino (C/C++), sensor acquisition, PWM motor control, interrupts, servomotors |
| Instrumentation | Experimental calibration, statistical analysis of measurements |
| Documentation | Technical writing, keeping documentation consistent with the implementation |

## Featured projects
### [Data-Attack-Resilient TinyML — DC Motor Monitoring](https://github.com/AnonymousCandela/moteur-tinyml) · 🚧 *In progress*
TinyML anomaly detection for an IoT DC motor that stays reliable when sensor data is forged, injected or replayed, and tells a real fault apart from a data attack.

* Physics-based DC motor simulator (electrical, mechanical, thermal) with 4 fault types and 5 sensor-data attacks: injection, modification, frozen value, replay, noise.
* INT8 neural network (3,845 parameters, 7.5 KB) running in TensorFlow Lite Micro on ESP32-S3 firmware under QEMU, matching the Python reference on 999 of 1,000 test windows.
* Two defence layers: HMAC-SHA256 with an anti-replay counter, and physical-consistency checks (electrical residual, noise fingerprint, active watermark). In simulation: 95.6 % of attacked windows detected, 99.9 % safe decisions when a real fault is masked (5 seeds).
* Validated on real motor measurements (Paderborn University dataset): frozen temperature detected 99.7 % of the time, replay only 34 %, a documented limitation.
* End-to-end MQTT pipeline (Mosquitto) and an interactive Streamlit dashboard to replay attack scenarios.

CYB6053 course project (IoT & embedded systems security) · UQO · Fall 2026 · Project documentation is in French.

### [DC Motor Monitoring — Arduino + FPGA](https://github.com/AnonymousCandela/surveillance-moteur-fpga)

Real-time embedded system that classifies a DC motor's condition as **NORMAL**, **DEGRADED** or **FAULT** from its speed and current.

- Full FPGA pipeline in VHDL: UART reception, frame decoding and checksum validation, threshold classifier, state transmission.
- State changes confirmed over 3 consecutive measurements, while faults are applied immediately for safety.
- 115,200 baud UART link between an Arduino Mega 2560 (5 V) and a DE1-SoC board (3.3 V).

*GEN5001 internship · UQO · Summer 2026*
*Project documentation is in French.*

### [Multifunction Address Register — ASIC flow in 65 nm](https://github.com/AnonymousCandela/registre-ar-asic-65nm)

4-bit multifunction address register taken from VHDL all the way to physical layout with the Cadence RTL-to-GDS flow.

- Synthesis with Genus on TSMC 65 nm standard cells: 22 cells, no timing violation (+9.2 ns setup slack at 100 MHz).
- Place and route with Innovus, with connectivity and geometry checks passing.
- Functional, post-synthesis and post-layout simulations with SDF back-annotation.

*GEN1333 Integrated Circuit Design · UQO · Winter 2026 · Team of four*
*Project documentation is in French.*

### [Automated Railway Level Crossing — FPGA](https://github.com/AnonymousCandela/passage-a-niveau-fpga)

Level crossing controller written entirely in VHDL on a DE1-SoC board.

- Redundant train detection in both directions with four HC-SR04 ultrasonic sensors.
- Servo-driven barrier (50 Hz PWM), traffic lights, "STOP" message on 7-segment displays and audible alarm.
- Obstacle detection on the track and PIN-protected manual mode.

*GEN1243 Digital Systems Design · UQO · Fall 2024 · Team of three*
*Project documentation is in French.*

### [Obstacle-Avoiding Robot — Arduino Uno](https://github.com/AnonymousCandela/Robot-Eviteur-d-obstacles)

Autonomous mobile robot that detects obstacles and reacts to avoid collisions.

- Distance measurement with an HC-SR04 ultrasonic sensor mounted on a scanning servo.
- Dual DC motor control through an L298N H-bridge with PWM speed control.
- Wiring diagram, demo video and full project report included.

*INF1643 Computer Architecture II · UQO · Winter 2024 · Team of two*
*Project documentation is in French.*

## Languages

French · English
