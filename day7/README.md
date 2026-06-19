# Day-7
# APB Protocol Verification using SystemVerilog

## Project Overview

This project demonstrates the verification of the Advanced Peripheral Bus (APB) protocol using SystemVerilog. The objective is to validate APB read and write transactions through a structured testbench environment consisting of generator, driver, monitor, scoreboard, and interface components.

## Features

- APB Read Transaction Verification
- APB Write Transaction Verification
- Transaction Monitoring
- Functional Checking using Scoreboard
- Mailbox-Based Communication
- Modular Verification Environment
- Easy-to-Understand Testbench Architecture

## APB Protocol

The Advanced Peripheral Bus (APB) is part of the ARM AMBA protocol family and is widely used for communication with low-speed peripherals such as timers, GPIOs, UARTs, and control registers.

## APB Characteristics

- Simple master-slave architecture
- Low power consumption
- Non-pipelined transfers
- Suitable for control and configuration operations


## Verification Environment

**Generator:**
Generates APB transactions and sends them to the driver.

**Driver:**
Drives transaction data onto the APB interface according to protocol timing.

**Monitor:**
Observes APB bus activity and captures transaction information.

**Scoreboard:**
Compares expected and actual transaction results to determine correctness.

**Interface:**
Provides a common communication structure between DUT and verification components.

## APB Transaction Flow

**Write Operation**

1. Master places address and write data on the bus.
2. PSEL is asserted.
3. PENABLE is asserted in the next cycle.
4. Slave accepts data and asserts PREADY.
5. Transaction completes.

**Read Operation**

1. Master places address on the bus.
2. PSEL is asserted.
3. PENABLE is asserted in the next cycle.
4. Slave places data on PRDATA.
5. PREADY indicates completion.
6. Master captures the read data.

**Simulation Flow**

1. Compile all SystemVerilog files.
2. Run simulation.
3. Generator creates APB transactions.
4. Driver drives transactions to DUT.
5. Monitor captures bus activity.
6. Scoreboard verifies correctness.
7. Results are displayed in simulation logs.

## Learning Outcomes

- Understanding of APB protocol operation
- SystemVerilog testbench development
- Verification component interaction
- Mailbox communication mechanism
- Transaction-based verification methodology
- Scoreboard-based checking techniques

## RESULT
<img width="966" height="496" alt="Screenshot 2026-06-17 154000" src="https://github.com/user-attachments/assets/d95215a1-07a8-4d54-b884-07685e386a11" />
