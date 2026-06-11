## Day 2

## Objective

The objective of Day 2 was to understand the design and implementation of basic combinational and sequential circuits using Verilog HDL. The functionality of each design was verified through simulation in Vivado.

## 4×2 Encoder

A 4×2 Encoder was implemented using Verilog HDL. The encoder converts one active input among four input lines into a corresponding 2-bit binary code at the output.

The design consists of:

* Four input lines (`I[3:0]`)
* Two output lines (`Y[1:0]`)

The encoder generates the binary representation of the active input line.

**Verification:**
A Verilog testbench was developed to verify the encoder operation by applying different input combinations and observing the corresponding encoded outputs.
<img width="1256" height="621" alt="encoder" src="https://github.com/user-attachments/assets/daae41c0-1824-411d-99ed-05fe4aac04ce" />

## SR Flip-Flop

An SR (Set-Reset) Flip-Flop was implemented using Verilog HDL. The flip-flop stores a single bit of information and changes its state based on the Set and Reset inputs.

The design consists of:

* Set input (`S`)
* Reset input (`R`)
* Outputs (`Q` and `Q̅`)

The SR Flip-Flop can set, reset, hold its state, or enter an invalid condition depending on the input combination.

**Verification:**
A Verilog testbench was created to verify the behavior of the SR Flip-Flop under different input conditions.
<img width="1271" height="615" alt="sr_flipflop" src="https://github.com/user-attachments/assets/996eb2c5-43be-4edd-9a94-72997acb4758" />


## D Flip-Flop

A D (Data) Flip-Flop was implemented using Verilog HDL. The D Flip-Flop stores the input data and transfers it to the output on the triggering edge of the clock signal.

The design consists of:

* Data input (`D`)
* Clock input (`CLK`)
* Output (`Q`)

The flip-flop eliminates the invalid state present in the SR Flip-Flop and serves as a basic storage element in digital systems.

**Verification:**
A Verilog testbench was developed to verify the operation of the D Flip-Flop by applying different data inputs and clock transitions.
<img width="1255" height="558" alt="dff" src="https://github.com/user-attachments/assets/1c892f4a-3545-457a-8cb7-91a1a54f45a3" />



## Universal Shift Register

A Universal Shift Register was implemented using Verilog HDL. The register supports multiple operations including hold, shift left, shift right, and parallel loading of data.

The design consists of:

* Clock input (`CLK`)
* Control inputs
* Serial inputs
* Parallel data inputs
* Register outputs

The Universal Shift Register provides flexibility in data movement and storage operations within digital systems.

**Verification:**
A Verilog testbench was developed to verify all operating modes of the Universal Shift Register, including shifting and parallel loading operations.
<img width="1256" height="603" alt="usr (2)" src="https://github.com/user-attachments/assets/f7b503ab-5a16-4467-88a9-e31da5e79a3e" />

**Result:**
The 4×2 Encoder, SR Flip-Flop, D Flip-Flop, and Universal Shift Register were successfully implemented and verified using simulation in Vivado. These designs provided practical experience with both combinational and sequential logic circuits, as well as fundamental data storage and data transfer operations in digital systems.
