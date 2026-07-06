# A Low-Cost Embedded Control System for Tremor Detection and Active Vibration Cancellation

> 🚧 Academic Research Project (Unpublished)

![Status](https://img.shields.io/badge/Status-Unpublished%20Research-orange)
![Platform](https://img.shields.io/badge/Platform-ESP32-blue)
![Language](https://img.shields.io/badge/Language-C++-brightgreen)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 📌 Project Status

> **Note**
>
> This repository contains an **academic embedded systems research project** developed as part of coursework and technical research.
>
> **The associated manuscript has NOT been published or accepted by any conference or journal.**
>
> This repository is intended solely to showcase the project's design, implementation, documentation, and experimental work.

---

# 📖 Overview

Physiological tremors reduce precision during tasks requiring fine motor control, such as biomedical instrumentation, microsurgery, and precision robotics.

This project presents a **low-cost embedded control system** capable of detecting tremors in real time and actively suppressing unwanted vibrations using motion sensing, embedded signal processing, and closed-loop control.

The system integrates:

- ESP32 Microcontroller
- MPU6050 Motion Sensor
- PD Controller
- Servo Motor
- Real-time Motion Processing

The objective is to provide an affordable, portable, and energy-efficient tremor compensation system suitable for biomedical and assistive applications.

---

# ✨ Features

- Real-time tremor detection
- Active vibration cancellation
- Closed-loop embedded control
- Lightweight PD control algorithm
- Low-cost hardware implementation
- Portable architecture
- Low latency response
- Energy-efficient operation
- Easy to expand for wearable systems

---

# 🏗 System Architecture

```
          Hand Motion
                │
                ▼
         MPU6050 Sensor
                │
                ▼
          ESP32 Controller
                │
                ▼
       Digital Signal Filtering
                │
                ▼
         PD Control Algorithm
                │
                ▼
            PWM Output
                │
                ▼
           Servo Motor
                │
                ▼
 Active Tremor Compensation
```

---

# 🔧 Hardware Components

| Component | Purpose |
|------------|----------|
| ESP32 | Main Processing Unit |
| MPU6050 | Motion Sensing |
| Servo Motor | Active Compensation |
| Breadboard | Prototyping |
| Jumper Wires | Connections |
| Power Supply | System Power |

---

# 💻 Software Stack

- Arduino IDE
- Embedded C++
- ESP32 SDK
- I²C Communication
- PWM Control
- Signal Filtering
- PD Control Algorithm

---

# ⚙ Working Principle

The system continuously measures hand motion using the MPU6050.

The ESP32 receives accelerometer and gyroscope data through the I²C interface.

The controller filters the incoming signals to isolate tremor frequencies while preserving intentional movements.

Once tremors are detected, a Proportional-Derivative (PD) controller computes the required correction.

The ESP32 generates PWM signals to drive the servo motor, which produces an opposite-phase motion to suppress the tremor.

This feedback process repeats continuously, enabling real-time active vibration cancellation.

---

# 📈 Control Algorithm

The project employs a **Proportional-Derivative (PD) Controller**.

Control Equation:

```
Output = Kp × Error + Kd × (dError/dt)
```

Where:

- **Kp** = Proportional Gain
- **Kd** = Derivative Gain

The proportional term responds to tremor magnitude, while the derivative term improves stability by responding to the rate of change.

---

# 📊 Experimental Results

Testing demonstrated:

- Tremor reduction of approximately **65–75%**
- Average response latency below **15 ms**
- Stable servo response
- Minimal overshoot
- Low power consumption
- Effective distinction between voluntary movement and tremor

---

# 🎯 Applications

- Biomedical Devices
- Assistive Technology
- Rehabilitation Systems
- Wearable Electronics
- Surgical Instrument Stabilization
- Precision Robotics
- Active Vibration Control
- Smart Healthcare Systems

---

# 🚀 Future Scope

Potential improvements include:

- Machine Learning–based adaptive control
- Automatic PD tuning
- IoT connectivity
- Mobile application integration
- Battery optimization
- Wearable implementation
- Multi-axis stabilization
- Cloud-based monitoring

---

# 📂 Repository Structure

```
embedded-tremor-detection-control-system/

├── README.md
├── LICENSE
├── docs/
│   ├── Research_Manuscript.pdf
│   ├── Project_Report.pdf
│   ├── Architecture.png
│   └── BlockDiagram.png
│
├── hardware/
│   ├── CircuitDiagram.png
│   ├── Components_List.md
│   ├── WiringConnections.md
│   └── PCB/
│
├── firmware/
│   ├── ESP32_Code.ino
│   ├── SensorReading.cpp
│   ├── PD_Controller.cpp
│   ├── ServoControl.cpp
│   └── libraries.txt
│
├── simulation/
│
├── images/
│   ├── Prototype.jpg
│   ├── Hardware.jpg
│   ├── Results.png
│   └── Architecture.png
│
├── results/
│   ├── ExperimentalData.xlsx
│   ├── Graphs.png
│   └── Performance.md
│
└── citations/
```

---

# 📚 Research Status

This repository accompanies an original embedded systems research project.

The manuscript is currently **unpublished** and is shared exclusively for educational, academic, and portfolio purposes.

The repository showcases:

- Project documentation
- Hardware implementation
- Embedded firmware
- System architecture
- Experimental evaluation
- Supporting resources

**This work should not be cited as a published research paper.**

---

# 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

If you discover issues or have ideas for enhancing the project, feel free to open an Issue or submit a Pull Request.

---

# 📄 License

The software and source code in this repository are licensed under the **MIT License**.

The research manuscript, figures, diagrams, and documentation remain the intellectual property of the project authors.

Please do not redistribute or republish the manuscript without prior permission.

---

# 👨‍💻 Author

## Ravuru Tharun

B.Tech – Electronics and Communication Engineering

VIT University, Vellore

📧 Email:
tharunravuruofficial@gmail.com

🔗 GitHub:
https://github.com/THARUN2939

---

# ⭐ Support

If you found this project interesting, consider giving it a ⭐ on GitHub.

Your support helps showcase academic and embedded systems projects to the wider developer community.
