# MOS

MOS (Miniature or Minimal OS) is a small, from-scratch project OS intended primarily for learning about hardware-software co-design.

The intent is explicitly not to be a production quality or general purpose OS and is instead being built with a focus on implementing the minimum requirements an OS must meet to exercise and validate low-level system concepts and functions, including:
 - Bootstrapping on bare metal
 - Basic memory management
 - Interrupt handling
 - Preemptive scheduling
 - Simple device drivers

Explicit non-goals include:
 - File systems
 - User friendly GUIs
 - Intense performance analysis (optimizations may be made casually if they appear easily)
 - POSIX
 - Networking
 - SMP

MOS is specifically designed to run on a custom RISC-V CPU implemented on an FPGA rather than an existing platform. This allows for ample opportunity for co-development, optimization, and reasoning between them.

## Status
MOS is not functional and is the second in a line of three projects designed with the above intents in mind: the RISC-V CPU mentioned above, MOS, and an accelerator designed to work with them. The current repository is a placeholder until the CPU is functional. 

Progress will be published here once the initial skeleton and boot pipeline are functional.

## Project Context
As mentioned above, MOS is intended to function on the RISC-V CPU platform that is being developed on an FPGA and will work with an accelerator for it. The order they are planned to be tackled in is:
1. CPU (RV32-Base) [here](https://github.com/Aespekson/RV32-Base)
2. MOS [this repo](https://github.com/Aespekson/MOS)
3. Accelerator (RV32-Aux-Unit) [here](https://github.com/Aespekson/RV32-Aux-Unit)
