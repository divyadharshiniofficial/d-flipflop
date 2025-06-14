# D Flip-Flop using SystemVerilog

This project demonstrates the design and simulation of a *D Flip-Flop* using SystemVerilog. It includes a simple and effective module for the D Flip-Flop along with a testbench to verify its behavior.

## 📁 Repository Contents

- d_flip_flop.sv – D Flip-Flop design module  
- tb_d_flip_flop.sv – Testbench to simulate and validate the design  
- README.md – Project documentation

## 🔧 Key Features

- Positive edge-triggered operation  
- Clean and minimal SystemVerilog code  
- Testbench verifies expected functionality  
- Behavioral simulation tested

## ▶️ How to Simulate

Make sure you have a SystemVerilog-compatible simulator like *Icarus Verilog* installed.

1. *Compile the files*:

bash
iverilog -g2012 -o dff_sim tb_d_flip_flop.sv d_flip_flop.sv


2. *Run the simulation*:

bash
vvp dff_sim


## 🧪 D Flip-Flop Behavior

- On the *rising edge* of the clock, the output Q takes the value of the input D.  
- If the clock does not toggle, the output remains unchanged.  

### Truth Table Example

| Clock Edge | D | Q (Output) |
|------------|---|------------|
| Rising     | 0 | 0          |
| Rising     | 1 | 1          |
| Rising     | 0 | 0          |



Author: Divyadharshini J  
