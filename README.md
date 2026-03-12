# 8-bit Spike Processor

## Overview
This repository contains the logic diagram implementation of a processor with an 8-bit data path architecture. The project is based on the main circuit named `Processador8bitSpike` and was entirely developed and structured in the `Processador_8bit_Spike_T16.circ` file.

## Software Requirements
To open, edit, or simulate the execution flow of this processor, the following logic simulation software is required:
* **Logisim-evolution v3.9.0** (https://github.com/logisim-evolution/).

## Architecture and Circuit Components
The processor was built using several native logic blocks, supporting the classic functions of a CPU. The circuit takes advantage of the following key modules:
* **Arithmetic Modules:** Implements elementary mathematical operations using integrated components such as the `Adder`, `Subtractor`, and `Negator`.
* **Control and Data Path:** Extensively uses `Multiplexer` blocks for routing branches and selecting input signals. It also includes modular selectors and bit manipulators (`Bit Extender` and `Splitter`) for fractional manipulation of the 8-bit word.
* **Memory and Temporary Storage:** Incorporates RAM memory elements and `Registers` to temporarily store ALU values and program variables, alongside logic blocks like `D Flip-Flops`. The instructions to be executed are encoded in a base `ROM` memory.
* **Classic Digital Logic:** The control structure is based on fundamental logic gates such as `NOT`, `AND`, `OR`, `XOR`, `NAND`, and `NOR`.
* **Synchronization:** The sequential progression of the processor and its instructions is orchestrated by a centralized `Clock` module.

## How to Run and Simulate
1. Ensure you have **Logisim-evolution** (version 3.9.0) installed on your machine.
2. Open the simulator and load the main project file: `Processador_8bit_Spike_T16.circ`.
3. Start the *Clock* signal in the simulation toolbar to see the instructions flow through the data path.
4. You can manually interact with the circuit's internal state using Logisim's native mapping tools, such as the "Poke Tool", and other interactive buttons provided in the project.

## Authors
**Group T16** *(Based on the repository/project file identification).*

## License

MIT License © 2025 Guilherme Marques.
