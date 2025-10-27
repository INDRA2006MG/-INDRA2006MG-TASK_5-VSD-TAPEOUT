# Week-5-VSD-RISC-V-Tapeout-Program
`19/10/2025` to `25/10/2025`

In this experiment, we employ OpenROAD Flow Scripts to perform the Floorplanning and Placement phases of the physical design workflow for the GCD circuit. This experiment represents the progression from SPICE-level transistor design (Week 4) to the backend implementation stage, where the synthesized GCD logic is transformed into a tangible physical layout utilizing automated EDA tools.

---
## Objectives

- Configure the **OpenROAD Flow Scripts** environment for physical design automation.
- Perform the **Floorplan** and **Placement** phases of the backend implementation workflow.
- Progress from **SPICE-level transistor design (Week 4)** to the **physical layout** phase.
- Comprehend how synthesized logic is converted into an **actual chip layout** through EDA tools.

---
## Prerequisites and Environment Setup

### System Requirements

Ensure your development environment meets the following specifications:

- **Operating System**: Ubuntu 20.04 or later (Ubuntu 22.04 recommended)

- **Version Control**: Git (latest stable version)
- **Build Toolchain**:

   - CMake (version 3.14 or higher)
   - GCC/G++ compiler suite
   - GNU Make
   - Standard development libraries

- **Python Environment**: Python 3.6 or higher

- **Required EDA Tools**
The following Electronic Design Automation tools must be available:

- **OpenROAD**: Physical design automation platform
- **Yosys**: Logic synthesis framework
- **OpenSTA**: Static timing analysis engine

---
## Importance of Floorplanning and Placement

Floorplanning is a crucial stage in the physical design process that defines the overall structure and layout of the chip prior to cell placement. It includes:

- Determining the die and core dimensions.
- Positioning I/O pads along the die periphery.
- Strategically arranging macros (such as SRAMs and PLLs).
- Organizing the core area into standard cell rows.
- Designing an efficient power distribution network (PDN).
- Reserving regions for physical-only cells (e.g., tap cells, endcaps, and blockages).
## OpenROAD

- [**Floorplan+Placement**](https://github.com/Rahul-Sivesh-11/RISC-V_Tape_Out_Week_5/blob/main/Floorplan%2BPlacement.md)

---

## Acknowledgements

Special appreciation to Mr. [Kunal Ghosh](https://in.linkedin.com/in/kunal-ghosh-vlsisystemdesign-com-28084836) and the VSD team for supplying guidance and resources.  
Gratitude to the SKY130 PDK community, Contributors of VSDBabySoC repository and open-source tools contributors including OpenROAD, OpenSTA, Yosys, Icarus Verilog, and GTKWave.

---

## Contributor

Rahul Sivesh S ([LinkedIn](https://www.linkedin.com/in/rahul-sivesh-a78ab6329/)) 

---

Previous week, Week 4 (NgSpice Analysis) : [Week 4 Repository](https://github.com/Rahul-Sivesh-11/RISC-V_Tape_Out_Week_4/tree/main)

---
### Workflow Overview
The implementation followed a systematic three-phase approach:

**Phase 1**: Development Environment Configuration

- Successfully installed and integrated essential EDA tools including OpenROAD, Yosys, OpenSTA, and OR-Tools
- Configured a robust development environment on Ubuntu-based Linux distribution (Ubuntu/Zorin OS) with necessary dependencies: Git, CMake, GCC compiler suite, and Python 3.6+
- Compiled OpenROAD from source code and established proper build configuration
- Deployed OpenROAD Flow Scripts with correct binary linkages to installed tool executables

**Phase 2**: Floorplan Design Execution

- Accessed the workflow execution directory within OpenROAD-flow-scripts/flow
- Successfully generated the floorplan for the GCD design using automated make targets
- Conducted visual verification through the integrated GUI, confirming proper die boundaries, core area definition, and I/O pin placement

**Phase 3**: Physical Placement Implementation

- Executed the placement stage, optimizing standard cell positions within the floorplan
- Performed graphical inspection of placement results via GUI interface
- Validated the correct positioning of Sky130 standard cell library components with no design rule violations

**Key Achievements**
Upon completion of this laboratory exercise, the GCD module has been successfully transitioned through critical physical design stages:

- **Established Physical Foundation**: Created a well-defined floorplan with optimized die area and power distribution planning
- **Achieved Legal Placement**: Positioned all standard cells within design constraints, ensuring manufacturability
- **Prepared for Backend Flow**: Generated placement data ready for subsequent stages including clock tree synthesis, detailed routing, and comprehensive timing analysis

This work provides the essential groundwork for completing the full VLSI backend implementation flow, enabling progression toward tape-out readiness.

---
