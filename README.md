# Carry-Look-Ahead

A 4-bit Carry Look-Ahead Adder (CLA) serves as a digital circuit tailored for the addition of two 4-bit binary numbers. Differing from ripple carry adders that sequentially transmit carry bits through each stage, the CLA utilizes logic gates to concurrently generate carry signals for all bit positions. This parallel carry signal generation significantly enhances computation speed for the final sum without the delay characteristic of ripple carry mechanisms.

The CLA's architecture primarily comprises two essential components: Generate (G) and Propagate (P) signals. The Generate signal discerns the moment a carry is created for a specific bit position based on input bits, while the Propagate signal indicates if a carry should be carried forward from a lower bit position to a higher one.

By utilizing these G and P signals, the CLA computes the carry-out (Cout) for each bit position in parallel. This approach accelerates addition by concurrently determining carries across the entire adder, reducing reliance on prior carry bits. Moreover, the CLA's design permits easy scalability for larger bit-width additions, enabling extension of the same logic for handling more bits while preserving efficiency in carry propagation.

Regarding the source code and test bench in the `iverilog` bin and generating output tables in `gtkwave`, I'd need the specific code you'd like to use in order to assist with integrating it into `iverilog` and `gtkwave`. If you have code you'd like help with, please share it and I can assist with incorporating it into these tools!

Command for the output table of carry look ahead
```shell
iverilog -o cla cla.v cla_tb.v
```

Command for generating a gtkwave

```shell
gtkwave CLA_4bit.vcd
```
