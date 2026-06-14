## Day-5
## FIFO Design and Testbench


This project implements an 8-bit wide, 8-depth First-In First-Out (FIFO) memory using Verilog HDL. The design supports synchronous read and write operations and includes status flags to indicate FIFO full and empty conditions.

**Features**

- 8-bit data width
- 8 memory locations
- Synchronous read and write operations
- Full and Empty status flags
- Implemented using Verilog HDL
- Simulated and verified using AMD Vivado 2023.2

**Inputs**

- "clk" : System clock
- "rst" : Active-high reset
- "wr_en" : Write enable
- "rd_en" : Read enable
- "data_in[7:0]" : Input data

**Outputs**

- "data_out[7:0]" : Output data
- "full" : FIFO full indicator
- "empty" : FIFO empty indicator

**Functionality**

- Data is written into the FIFO when "wr_en" is asserted and the FIFO is not full.
- Data is read from the FIFO when "rd_en" is asserted and the FIFO is not empty.
- The FIFO uses separate read and write pointers to manage data flow.
- Full and empty conditions are determined using an internal counter.

### Verification

A SystemVerilog testbench was developed using an interface-based approach to verify FIFO functionality. The testbench performs:

- Reset operation
- Multiple write transactions
- Multiple read transactions
- Monitoring of FIFO status flags
- Waveform verification using Vivado Simulator


### Simulation Result

Simulation confirms correct FIFO operation, including successful data storage, retrieval, and proper assertion of Full and Empty status flags.
<img width="1613" height="647" alt="fifo_interface" src="https://github.com/user-attachments/assets/283b92e5-c8cc-47b7-9694-22343d92ed61" />

