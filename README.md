AIM:

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

Equipments Required:

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

Half Adder

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

program:

```
module HalfAdd(
    input  wire a, b,     // Inputs
    output wire sum,      // Sum output
    output wire carry     // Carry output
);

    // Logic equations
    assign sum   = a ^ b;   // XOR for sum
    assign carry = a & b;   // AND for carry

endmodule
```
Image:
[HalfAdd RTL.pdf](https://github.com/user-attachments/files/24032648/HalfAdd.RTL.pdf)

[wave map img.bmp](https://github.com/user-attachments/files/24073513/wave.map.img.bmp)

output:
[EX3 HalfAdd wave.pdf](https://github.com/user-attachments/files/24073509/EX3.HalfAdd.wave.pdf)


We got the expected output in program

