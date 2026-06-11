 3

## Sequence Detector (1110 Overlapping)

Implemented a sequence detector in Verilog using FSM to detect the pattern 1110 with overlapping capability. Designed the corresponding testbench and verified the functionality through simulation waveforms.
<img width="1609" height="624" alt="sequencedetector" src="https://github.com/user-attachments/assets/ee457150-4768-4cd2-9174-2a46e15cb001" />

## Face Sensor Data Transfer Using FIFO

**Objective**
To transfer 8-bit sensor data from a high-speed face module to a slow output module using a FIFO buffer.

**Description**
This project consists of three modules:

1. Face Module
2. FIFO
3. Module Out

The Face Module receives 8-bit sensor input data and generates output on every positive edge of the clock. Since the face module operates at a higher speed than the output device, a FIFO is used as an intermediate buffer.

The FIFO stores incoming data and provides synchronized data transfer between the fast producer and slow consumer.

The Module Out acts as a slow device and updates its output only after every three clock cycles. This demonstrates how FIFO can be used to prevent data loss when transferring data between modules operating at different speeds.

## Modules
## Face Module
- Input : clk, sensor_in[7:0]
- Output : sensor_out[7:0]
- Captures sensor data on every positive clock edge.

## FIFO
- Stores 8-bit data.
- Supports write and read operations.
- Provides temporary storage between modules.
- <img width="1621" height="639" alt="fifo" src="https://github.com/user-attachments/assets/1bdcf0a5-8715-4351-9978-ec361fae5468" />


## Module Out
- Receives data from FIFO.
- Generates output after every three clock cycles.
- Simulates a slow device.

## Top Module
- Integrates Face Module, FIFO and Module Out.
- Provides complete data flow from sensor input to final output.
- <img width="1623" height="632" alt="top_module" src="https://github.com/user-attachments/assets/5c582282-870f-4831-9389-a8f064ff4b93" />


**Inputs**
- clk
- rst
- sensor_in[7:0]

**Output**
- d_out[7:0]

**Files**
- face_module.v
- fi_fo.v
- module_out.v
- top_module.v
- top_module_tb.v

**Result:**
The design was implemented and simulated in Vivado. The FIFO successfully buffered data between the high-speed face module and the slow output module, demonstrating reliable data transfer between modules operating at different speeds.
