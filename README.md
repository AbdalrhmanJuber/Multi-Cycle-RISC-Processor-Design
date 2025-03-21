# Multi-Cycle RISC Processor Design
![(AND_Stage3)](https://github.com/user-attachments/assets/d99c2754-8f1b-48db-8e8f-e7f00b1775f1)
![(AND_Stage2)](https://github.com/user-attachments/assets/eeae907a-2d86-4935-b2ca-970bd4106a6a)
![(AND_Stage1)](https://github.com/user-attachments/assets/8a2ce9e7-b1e8-41c1-b8c2-681f9257ed67)
![(AND_Instruction)](https://github.com/user-attachments/assets/03f3b6ff-bd85-4aed-95de-44b971c3dca5)
![(AND_Stage4)](https://github.com/user-attachments/assets/4e62fcec-9caa-45c9-a76e-08b9f642bc00)

## Project Overview
This project involves designing and implementing a multi-cycle five-stage RISC processor. The processor supports a specific subset of RISC instructions, complete with individual components like ALU, register file, data memory, and control unit. It also includes extensive simulation and testing to verify functionality.

## Project Goals
- Analyze and implement a specific RISC instruction set architecture (ISA).
- Design modular components, including ALU, Register File, Instruction Memory, Data Memory, and Control Unit.
- Assemble the components into a functional datapath.
- Develop a finite state machine-based Control Unit to manage instruction execution.
- Simulate and validate the processor through various test programs.

## Components and Design
### 1. Instruction Memory
- Byte-addressable storage for instructions.

### 2. Data Memory
- Byte-addressable, with additional signals for byte/word operations (LBu, LBs).

### 3. Extender
- Supports zero and sign extension for immediate values.

### 4. ALU
- Performs ADD, SUB, AND operations.
- Outputs include result, zero flag, and negative flag.

### 5. Register File
- Contains eight registers (R0-R7), with R7 used specifically for CALL/RET instructions.

### 6. Branch Control
- Logic gates to determine branch conditions based on ALU flags.

### 7. Datapath
- Integrated modular components forming a multi-cycle pipeline (fetch, decode, execute, memory access, and write-back stages).

### 8. Control Unit
- Finite state machine handling all control signals for each instruction stage.
- Boolean equations derived for all control signals.

## Instructions Supported
- R-type: AND, ADD, SUB
- I-type: ADDI, ANDI, LW, LBu, LBs, SW
- Branch: BLT, BGTZ
- CALL, RET
- JUMP, SV

## Testing and Simulation
- Conducted comprehensive tests with different instruction sets (arithmetic, logic, load/store, branching, call/return, jump, store value).
- Simulation performed using waveforms to validate correctness at each pipeline stage.

## Project Deliverables
- Modular RTL design using Verilog.
- Testbench environment.
- Documentation (truth tables, Boolean equations, and detailed design descriptions).

## How to Run the Project
1. Clone this repository.
2. Load the provided Verilog files into a simulation environment (e.g., ModelSim, Quartus).
3. Run the testbench to simulate and validate the processor operation.

## Contributors
- Abdalrahman Juber (ID: 1211769)
- Ali Shaikh Qasem (ID: 1212171)


## Supervisors
- Dr. Ayman Hroub
- Dr. Aziz Qaroush

## University
Birzeit University, Faculty of Engineering and Technology, Department of Electrical and Computer Engineering.

## Date
June 20, 2024

