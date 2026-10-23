<div align="center">

# Pranay V

**Embedded Systems · VLSI Design & Verification · Edge AI**

Final-year B.E. Electronics & Communication Engineering (VLSI Honors) at Sri Venkateswara College of Engineering, Chennai.
I build connected hardware end to end and design and verify digital hardware in Verilog.

[![Portfolio](https://img.shields.io/badge/Portfolio-pranayviswaraj.github.io-7c3aed?style=for-the-badge&logo=googlechrome&logoColor=white)](https://pranayviswaraj.github.io)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-pranayviswaraju-0a66c2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/pranayviswaraju/)
[![Email](https://img.shields.io/badge/Email-vpranay2005%40gmail.com-ea4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:vpranay2005@gmail.com)

</div>

---

## About me

- 🔧 **Now:** Embedded Engineer Intern at **Tivor**, building end-of-line test software for automotive electronics (CAN / CAN FD, LIN, SCPI, GigE vision).
- 🧠 **Focus:** RTL design and verification, embedded and IoT systems, and on-device machine learning.
- 📜 **Two published Indian patent applications** (Patent Office Journal 24/2026).
- 🏆 **Hackathons:** Smart India Hackathon 2025 national finalist, K-Hacks (CEG) Special Track winner, plus 10+ hackathon wins and top finishes.
- 🎯 **Looking for:** full-time roles in RTL design, design verification, FPGA prototyping and embedded systems.

---

## Experience

| Role | Organization | Period | Highlights |
|---|---|---|---|
| **Embedded Engineer Intern** | Tivor, Chennai | Sep 2026 – Present | End-of-line functional test platform for automotive electronics; hardware abstraction layer with runtime driver binding across CAN, DAQ, SCPI and GigE devices; proof of concept on a live production line |
| **Embedded & Software Engineer Intern** | Rela Hospitals, Chennai | Feb 2026 – Apr 2026 | Non-invasive blood group prediction from fingerprints on ESP32 hardware: **94% accuracy, under 5 s**; tested against clinical requirements |
| **Industrial IoT Project Intern** | Ashok Leyland, Chennai | Nov 2025 – Apr 2026 | ESP32 → MQTT battery and GPS monitoring for **30+ forklifts**: **−60%** manual inspection, **−40%** unplanned downtime, **+20%** battery life |
| **RAG & Application Development Intern** | Playful Python, Chennai | Dec 2024 – Jan 2025 | Production RAG assistant over **1,000+ documents**; **+35%** retrieval precision with chunk-aware indexing and query rewriting |

---

## Featured projects

### VLSI design & verification

| Project | What it is | Key results |
|---|---|---|
| [**Adaptive Reconfigurable Cache Controller**](https://github.com/PranayViswaraj/Mini-Project---Cache-Memory-Management) | 32-bit, 1–16 KB, 2/4-way write-through cache in Verilog with Random, LRU and Pseudo-LRU replacement and a set-dueling runtime policy selector | **218/218** regression tests vs a Python reference model (~3.7 M requests); **+0.43%** area; up to **−38.7%** stall cycles vs LRU (Yosys + Nangate 45 nm) |
| [**ARINC 429 Health-Aware Controller**](https://github.com/PranayViswaraj/ARINC429) | Transmitter, receiver and controller RTL for the ARINC 429 avionics bus, with a fault-injection testbench (final-year project) | **271/271** tests; **100%** single-bit parity error detection |
| **Gesture-to-Speech on FPGA** | FSM-based RTL turning flex-sensor and MPU6050 data into speech | **200 MHz** in Cadence Genus, critical path **< 2 ns**, power **< 25 mW**; validated on an Altera FPGA |

### Embedded systems & IoT

| Project | What it is | Key results |
|---|---|---|
| **AgroSmart** · *patent published* | ESP32 → MQTT → Flask → MongoDB → React precision-agriculture platform with a sensor rover, ML-driven drip irrigation and rainwater harvesting | **92%** oilseed yield-forecast accuracy; **−30%** water use |
| [**PROTECT-R: AI-Powered Offline Women Safety Wearable**](https://github.com/PranayViswaraj/ProtectR-Intelligent-Safety-and-Emergency-Response-System) | ESP32-S3 wearable running three on-device models (TinyML audio, CNN gesture, LSTM motion), with GSM, GPS and LoRa 433 MHz alerting, MongoDB telemetry and a custom KiCad PCB | **96%** model accuracy; zero cloud dependency; Top 10 at PEC Hacks 4.0 |
| **Forklift Fleet Monitoring** (Ashok Leyland) | Battery health, charge cycles and GPS across a forklift fleet with predictive alerts | 30+ forklifts; −40% downtime |
| **End-of-Line Test Platform** (Tivor) | Configurable automotive ECU test platform with a hardware abstraction layer | In progress |

### AI, ML & software

| Project | What it is | Key results |
|---|---|---|
| **B-Logic** · *patent published* | Blood group prediction from fingerprints with a MobileNet / EfficientNet-B0 / ResNet-50 ensemble, ESP32 capture unit, Flask and React | **94%** accuracy, all 8 ABO/Rh groups |
| [**RecoverAI**](https://github.com/PranayViswaraj/RecoverAI) | AI agent that ranks failed payments by expected recovery, picks an intervention and passes it through guardrails | Next.js, FastAPI, OpenAI, Razorpay (test mode) |
| **RAG Knowledge Assistant** (Playful Python) | Retrieval-augmented generation over large document collections | +35% retrieval precision |
| [**AgriOS (GIS & field data)**](https://github.com/PranayViswaraj/AgriOS-Sample) | FastAPI services for farm registration, field observations, pest traps and hotspot mapping | Team project |

➡️ Full case studies with diagrams and results: **[pranayviswaraj.github.io/projects](https://pranayviswaraj.github.io/projects/)**

---

## Patents & research

- **A Non-Invasive Biometric System for Blood Group Prediction Using Fingerprint Analysis and Adaptive Deep Learning**: IN202641051215 A1, published 12 Jun 2026
- **An IoT-Enabled Intelligent System for Adaptive Irrigation and Rainwater Harvesting Using Machine Learning**: IN202641051218 A1, published 12 Jun 2026
- **Smart-Wear: IoT-Enabled AI Healthcare System for Women and Geriatric Care**: published
- Paper presentations: [AI-powered health bands, energy management, 5G to 6G, radar and sonar signal processing](https://github.com/PranayViswaraj/papers_presented)

---

## Tech stack

**VLSI & digital design**
![Verilog](https://img.shields.io/badge/Verilog-HDL-222?style=flat-square)
![Cadence Genus](https://img.shields.io/badge/Cadence-Genus-222?style=flat-square)
![Quartus Prime](https://img.shields.io/badge/Intel-Quartus%20Prime-0071c5?style=flat-square&logo=intel&logoColor=white)
![ModelSim](https://img.shields.io/badge/ModelSim-simulation-222?style=flat-square)
![Icarus Verilog](https://img.shields.io/badge/Icarus-Verilog-222?style=flat-square)
![Verilator](https://img.shields.io/badge/Verilator-lint-222?style=flat-square)
![Yosys](https://img.shields.io/badge/Yosys-synthesis-222?style=flat-square)

**Embedded & protocols**
![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=flat-square&logo=espressif&logoColor=white)
![Embedded C](https://img.shields.io/badge/Embedded-C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![CAN](https://img.shields.io/badge/CAN%20%2F%20CAN%20FD-LIN-555?style=flat-square)
![I2C SPI UART](https://img.shields.io/badge/I2C%20·%20SPI%20·%20UART-555?style=flat-square)
![LoRa](https://img.shields.io/badge/LoRa-GSM%20·%20GPS-555?style=flat-square)
![MQTT](https://img.shields.io/badge/MQTT-660066?style=flat-square&logo=mqtt&logoColor=white)
![KiCad](https://img.shields.io/badge/KiCad-314CB0?style=flat-square&logo=kicad&logoColor=white)

**AI / ML & software**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![TensorFlow Lite](https://img.shields.io/badge/TinyML-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Flask](https://img.shields.io/badge/Flask-000?style=flat-square&logo=flask&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

---

## Achievements & leadership

- **National-level results:** Smart India Hackathon 2025 (AICTE), national finalist · K-Hacks 2025 (CEG, Anna University), Special Track winner · PEC Hacks 4.0, Top 10 · IETE Convention, finalist
- **Hackathon wins & top finishes (10+):** Hack-Erupt 2026 · Hack-Infinity 2025 · Make-a-thon 2025 · Hack-Elite 2024 · Elite-Com · Startup Surge
- **Leadership:** Joint Secretary, ECE Association, SVCE · Web Developer, Science Club, SVCE

## Certifications

VLSI Digital Design: Chip Design and Verilog Programming (Infosys Springboard) · Application-Driven Electronics & Embedded Technology with IoT (IITM Pravartak) · Oracle Agentic AI Foundations (Oracle University) · GenAI, LLMs, AI Agents & RAG (Yuva AI, MeitY) · Concepts of Cybersecurity (Microsoft) · Getting Started with Docker (Simplilearn)

---

<div align="center">

**Open to full-time opportunities in VLSI, embedded systems and IoT.**
[Portfolio](https://pranayviswaraj.github.io) · [LinkedIn](https://www.linkedin.com/in/pranayviswaraju/) · [Email](mailto:vpranay2005@gmail.com)

</div>
