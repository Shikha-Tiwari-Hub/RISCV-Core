# RISCV-Core


# RV32IM RISC-V Processor

A 32-bit RISC-V processor design project covering processor architecture, RTL implementation, functional verification, logic synthesis, and physical design.

The project is organized into separate stages to document the journey from processor RTL to physical implementation.

## 1. Project Overview

The processor is based on the RV32IM instruction-set architecture and uses a three-stage in-order pipeline.

### Key Features

- 32-bit RISC-V RV32IM architecture
- Three-stage pipeline
- Fetch & Decode, Execute, and Memory Access & Write-back stages
- Register file and Control and Status Register (CSR) logic
- AXI4-Lite instruction and data interfaces

## 2. Processor Architecture

The processor is organized into three main pipeline stages:

1. **Fetch & Decode:** Fetches instructions and decodes their operation and operands.
2. **Execute:** Performs arithmetic, logical, and other supported operations.
3. **Memory Access & Write-back:** Handles data-memory operations and writes results back to the register file.

Additional modules provide register storage, control and status registers, and instruction/data interface functionality.

## 3. Overall ASIC Design Flow

<img width="800" height="500" alt="Digital_implementation Flow graph" src="https://github.com/user-attachments/assets/514f8633-4deb-41de-a71d-b0ebbfd50d96" />

## 4. Project Repositories

| Stage | Repository | Scope |
|---|---|---|
| RTL Design | This repository | Processor RTL, architecture, and design documentation |
| Functional Verification | [RISCV-Core-Verification]([VERIFICATION_REPO_URL](https://github.com/Shikha-Tiwari-Hub/RISCV-core-Verification.git)) | Testbenches, simulation, and verification evidence |
| Synthesis, DFT & LEC | [RISCV-Core-Synthesis-DFT-LEC]([SYNTHESIS_REPO_URL](https://github.com/Shikha-Tiwari-Hub/RISCV-Core-Synthesis.git)) | Gate-level synthesis, testability, and equivalence checks |
| Physical Design | [RISCV-Core-Physical-Design]([PHYSICAL_DESIGN_REPO_UR](https://github.com/Shikha-Tiwari-Hub/RISCV-Core-PhysicalDesign.git)L) | Floorplanning through routing, physical checks, and GDSII |


## 5. Tools and Technologies

Document the tools and versions actually used for each stage.

- **HDL:** Verilog
- **Architecture:** RISC-V RV32IM
- **Interfaces:** AXI4-Lite
- **Verification:** Iverilog, Gtkwave and Riscv Toolchain
- **Synthesis:** Genus
- **ATPG:** modus
- **LEC:** LEC 
- **Physical Design:** Innovus

## 6. Implementation Status

| Stage | Status |
|---|---|
| RTL Design | Implemented — verify current revision |
| Functional Verification | See verification repository |
| Logic Synthesis | Complete |
| DFT / ATPG | Complete |
| LEC | Complete |
| Physical Design | Complete |
| GDSII Generation | Complete |


## 7. Project Objectives

- Understand processor microarchitecture and RTL design.
- Validate functionality through reproducible simulation.
- Study RTL-to-gate-level synthesis and technology mapping.
- Explore design-for-testability and logic equivalence checking.
- Understand physical implementation from floorplanning to GDSII.
- Analyze area, timing, and physical verification reports.

## 8. Project Status

This repository serves as the central documentation page for the RISC-V processor project. Individual repositories contain stage-specific scripts, reports, methodology, and implementation evidence.
