# Pipelined RISC-V Processor

## Overview

This project focuses on the design and implementation of a pipelined RISC-V processor using Verilog HDL.

Pipelining is a processor design technique that improves instruction throughput by dividing instruction execution into multiple stages. This allows multiple instructions to be processed simultaneously, with each instruction occupying a different stage of the pipeline.

The project explores pipelined datapath design, pipeline registers, instruction execution, and control logic.

## Key Features

- Pipelined RISC-V processor architecture
- Multi-stage instruction execution
- Pipeline register design
- Datapath and control unit implementation
- Instruction decoding and execution
- Arithmetic and logical operations using the ALU
- Program Counter (PC) update logic
- Pipeline control mechanisms

## Pipeline Architecture

The processor follows a five-stage pipeline architecture:

1. **Instruction Fetch (IF):** Fetches the instruction from instruction memory.
2. **Instruction Decode (ID):** Decodes the instruction and reads source registers.
3. **Execute (EX):** Performs arithmetic and logical operations or calculates memory addresses.
4. **Memory Access (MEM):** Performs data memory operations when required.
5. **Write Back (WB):** Writes the result back to the register file.

Pipeline registers transfer intermediate data and control signals between consecutive stages.

The exact pipeline structure depends on the implemented design.

## Pipeline Hazards

Pipeline hazards are potential challenges that can affect the correct execution of instructions.

The main types of hazards are:

- **Data Hazards:** Occur when an instruction depends on the result of a previous instruction.
- **Control Hazards:** Arise from branch and jump instructions that affect the flow of execution.
- **Structural Hazards:** Occur when multiple instructions require the same hardware resource simultaneously.

Hazard detection, forwarding, stalling, and flushing mechanisms may be used to handle these situations, depending on the implementation.

## Technologies

- **Hardware Description Language:** Verilog HDL
- **Instruction Set Architecture:** RISC-V
- **Processor Architecture:** Pipelined

## Learning Objectives

This project provides practical experience with:

- Computer organization and processor architecture
- RTL design using Verilog HDL
- Pipelined datapath implementation
- Pipeline registers and control signals
- Instruction-level parallelism
- Pipeline hazards and their handling
- Digital system design and verification


## Author

Amirhossein Mohammadi
