# D Flip-Flop using SystemVerilog

This project demonstrates the design and simulation of a D Flip-Flop using SystemVerilog. A D Flip-Flop is a fundamental building block in digital electronics used for data storage and synchronization.

## 📁 Files Included

- d_flip_flop.sv - D Flip-Flop module
- tb_d_flip_flop.sv - Testbench to verify functionality
- dump.vcd - Waveform file generated after simulation
- README.md - Project documentation

## 🔧 Features

- Positive edge-triggered behavior
- Optional asynchronous reset (can be added if required)
- Simulation-ready
- Waveform generation support for EPWave or GTKWave

## 🚀 How to Simulate

Make sure you have a SystemVerilog simulator like *Icarus Verilog* installed.

1. *Compile the design and testbench*:

bash
iverilog -g2012 -o dff_sim tb_d_flip_flop.sv d_flip_flop.sv


2. *Run the simulation*:

bash
vvp dff_sim


3. *View the waveform*:

bash
gtkwave dump.vcd


## 🧪 Functionality

- On every *rising edge* of the clock, the output Q takes the value of the input D.
- If an asynchronous reset is used and asserted, Q is set to 0 immediately.

## 🖼️ Logic Diagram


     +-------------+
D -->|             |
     |   D Flip    |--> Q
CLK->|    Flop     |
     +-------------+


## 📌 Example Behavior

| Clock (↑) | D | Q (output) |
|-----------|---|------------|
| ↑         | 0 | 0          |
| ↑         | 1 | 1          |
| ↑         | 0 | 0          |

## 📄 License

This project is open-source and available under the MIT License.

---

*Author:* Divyadharshini J  
Feel free to ⭐ this repo if it helped you!
