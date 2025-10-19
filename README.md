🧠 SPI with Single-Port RAM Verification using UVM
📘 Overview

This project implements a SystemVerilog UVM (Universal Verification Methodology) testbench to verify a Serial Peripheral Interface (SPI) Slave integrated with a Single-Port RAM.

The work was done as part of the Digital Verification course under the supervision of Eng. Kareem Waseem.
The project demonstrates modular testbench design, assertion-based verification, functional coverage, and UVM reusability for real-world SoC verification environments.

🧩 Project Parts

The verification is divided into three main phases:

1️⃣ SPI Slave Verification

Developed a complete UVM environment (Driver, Monitor, Agent, Scoreboard, Sequencer, Environment)

Used constraints to randomize MOSI data and SS_n timing

Validated FSM transitions using SystemVerilog Assertions (SVA)

2️⃣ Single-Port RAM Verification

Created an independent UVM environment to test all read/write scenarios

Implemented assertion-based protocol checks

Achieved full functional and code coverage

3️⃣ SPI Wrapper Verification

Integrated both SPI and RAM environments using passive agents

Reused existing UVM components to verify end-to-end data transfer

Connected all verification layers for complete system testing

⚙️ Tools & Technologies

SystemVerilog

UVM (Universal Verification Methodology)

QuestaSim for simulation and coverage analysis

Verilog RTL & Golden Models

🧪 Verification Highlights
Metric	Result
Functional Coverage	✅ 100%
Code Coverage	✅ 100% (excluding memory arrays)
Assertion Coverage	✅ 100% (0 fails)
FSM Transitions	All successfully validated
Reusability	Both SPI and RAM agents reused in Wrapper environment
💡 Key Learning Outcomes

Mastered UVM architecture and coverage-driven verification

Gained hands-on experience in assertion-based verification (ABV)

Learned how to manage multiple UVM agents (active/passive) in one environment

Practiced real-world debugging through waveform analysis and coverage closure

🧱 Project Structure
SPI-RAM-UVM-Verification/
│
├── part1_spi_slave/
│   ├── design/
│   ├── uvm_env/
│   ├── assertions/
│   ├── coverage/
│   └── do_files/
│
├── part2_ram/
│   ├── design/
│   ├── uvm_env/
│   ├── assertions/
│   ├── coverage/
│   └── do_files/
│
├── part3_wrapper/
│   ├── design/
│   ├── uvm_env/
│   ├── assertions/
│   ├── coverage/
│   └── do_files/
│
└── documentation/
    ├── UVM_Project_Requirements.pdf
    └── Final_Report.pdf

👨‍💻 Authors

Abdelrahman Mahmoud

Youssef Mohamed Abdelaal Bayoum

Nabil Ebrahim Abd ElAty Abd ElRazeq

🎓 Supervisor

Eng. Kareem Waseem
Digital Verification Course Instructor
