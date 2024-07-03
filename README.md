# Floating-Point-Digital-Multiplier-Project
---> Description

The project involves the design and analysis of 16, 32, and 64-bit digital floating-point multipliers using the Verilog hardware description language.
The design leverages the Vedic algorithm Urdhva Tiryakbhayam Sutra. Simulations were conducted using Xilinx Vivado, specifically targeting a Spartan 6 FPGA board. 
During the simulations, the 32-bit multiplier was found to consume 48.464W and achieved a processing time of 13.712ns.

---> Principle

The project is based on the principles of digital arithmetic and Vedic mathematics. 
Floating-point multiplication is a fundamental operation in digital signal processing and scientific computing. 
The Vedic multiplier algorithm, Urdhva Tiryakbhayam Sutra, is known for its efficiency and simplicity in hardware implementation. 
This algorithm performs multiplication by decomposing the operands and computing partial products in parallel, which are then summed to get the final result.

---> Operation

1. Design Phase:
   - Implemented 16, 32, and 64-bit floating-point multipliers using Verilog.
   - Incorporated the Urdhva Tiryakbhayam Sutra for efficient computation.

2. Simulation Phase:
   - Used Xilinx Vivado for simulation and analysis.
   - Deployed the design on a Spartan 7 FPGA board.

3. Performance Measurement:
   - Measured power consumption and processing time.
   - The 32-bit multiplier was observed to consume 48.464W and had a processing time of 13.712ns.

---> Tools

* Xilinx Vivado: A comprehensive FPGA design suite used for writing, simulating, and implementing the Verilog code.
* Spartan 6 FPGA Board: The hardware platform for deploying and testing the digital multiplier designs.
