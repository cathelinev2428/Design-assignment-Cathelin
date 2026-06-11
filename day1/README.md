## Day 1

## Objective

The objective of Day 1 was to understand the design and implementation of combinational arithmetic circuits using Verilog HDL. The designs were verified through simulation in Vivado.

## 4-Bit Ripple Carry Adder

A 4-bit Ripple Carry Adder (RCA) was implemented using Verilog HDL. The adder performs binary addition of two 4-bit inputs along with a carry input. The carry generated from each full adder stage propagates to the next stage, resulting in the name "Ripple Carry Adder."

The design consists of:

* Two 4-bit inputs (`A[3:0]`, `B[3:0]`)
* Carry input (`Cin`)
* 4-bit Sum output (`Sum[3:0]`)
* Carry output (`Cout`)

The adder was designed by cascading four full adders, where the carry output of one stage becomes the carry input of the next stage.

### Verification
A Verilog testbench was developed to verify the functionality of the Ripple Carry Adder. Different combinations of input values were applied, and the generated sum and carry outputs were observed through simulation.

<img width="1403" height="746" alt="rca" src="https://github.com/user-attachments/assets/af2313a5-e359-4be9-ae66-6b7bcf6ff189" />

## BCD Adder

A Binary-Coded Decimal (BCD) Adder was implemented using Verilog HDL. The circuit performs decimal addition of two BCD digits along with an optional carry input. Whenever the binary sum exceeds 9, a correction value of 6 is added to obtain a valid BCD result.

The design consists of:

* Two 4-bit BCD inputs (`A[3:0]`, `B[3:0]`)
* Carry input (`Cin`)
* 4-bit BCD Sum output (`Sum[3:0]`)
* Carry output (`Cout`)

The design ensures that the output remains a valid BCD representation after addition.

### Verification
A Verilog testbench was created to verify the BCD Adder. Various BCD input combinations were tested, and the outputs were analyzed to confirm proper BCD correction and carry generation.

<img width="1563" height="724" alt="bcd" src="https://github.com/user-attachments/assets/76782fd2-e0f4-4b76-9472-e75ea00974b0" />


### Conclusion

Both the 4-bit Ripple Carry Adder and BCD Adder were successfully implemented and verified using simulation in Vivado. These designs provided a strong foundation in combinational circuit design, arithmetic operations, and Verilog-based verification.
