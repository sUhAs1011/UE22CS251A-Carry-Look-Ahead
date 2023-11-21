# Carry-Look-Ahead

This was my third sem DDCO(Digital Design And Computer Organisation) mini project, which is about carry look ahead.
A 4-bit Carry Look-Ahead Adder (CLA) is a digital circuit designed to perform addition on two 4-bit binary numbers. Unlike ripple carry adders, which propagate carry bits sequentially through each stage, a CLA employs logic gates to generate carry signals in parallel for all bit positions. This parallel generation of carry signals allows for faster computation of the final sum without the delay associated with ripple carry.

The CLA architecture consists of two main components: Generate (G) and Propagate (P) signals. The Generate signal identifies when a carry is generated for a particular bit position based on the input bits, while the Propagate signal indicates whether a carry should be propagated from a lower bit position to a higher one.

Using these G and P signals, the CLA computes the carry-out (Cout) for each bit position in parallel. This accelerates the addition process by enabling simultaneous carry determination across the entire adder, minimizing the dependency on previous carry bits. Additionally, the CLA architecture facilitates easy scalability for larger bit-width additions by extending the same logic to handle more bits while maintaining efficiency in carry propagation.

Please store the source code and the test bench code in the bin of the iverilog in order to generate the output table and gtkwave

The commands in 1.png are used for generating the output table and the command in 2.png is used for generating gtkwave
