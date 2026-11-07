# RTL-to-GDSII Implementation of an 8-bit ALU

## Project Overview

This project focuses on the design and physical implementation of an 8-bit Arithmetic Logic Unit (ALU) using Verilog HDL and the OpenLane RTL-to-GDSII flow.

The project initially started with a basic 2-bit calculator and was progressively extended into an 8-bit ALU supporting arithmetic and logical operations, along with status flags.

The design was implemented using the SKY130 Process Design Kit (PDK), followed by synthesis, physical design, verification and GDSII layout generation.

## Features

The 8-bit ALU supports eight operations:

| Select | Operation |
|:---:|---|
| 000 | Addition |
| 001 | Subtraction |
| 010 | Bitwise AND |
| 011 | Bitwise OR |
| 100 | Bitwise XOR |
| 101 | Bitwise NOT |
| 110 | Logical Shift Left |
| 111 | Logical Shift Right |

### Status Flags

- **Carry Flag:** Indicates carry generated during arithmetic operations.
- **Overflow Flag:** Indicates signed arithmetic overflow.
- **Zero Flag:** Indicates whether the ALU output is zero.

## Tools and Technologies

- **HDL:** Verilog
- **Simulation:** Icarus Verilog
- **Synthesis:** Yosys
- **Physical Design:** OpenLane 2
- **Technology:** SKY130 PDK
- **Layout Inspection:** KLayout
- **Environment:** Ubuntu, WSL
