# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

![image](https://github.com/user-attachments/assets/a7b3ef8d-0f2e-4c92-bb06-eca8d6e7bdff)


**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

![image](https://github.com/user-attachments/assets/0f22a5ac-e69a-4422-820a-14ae6b660d50)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Developed by: Varun A

RegisterNumber: 24900420

Half Adder

```
module lab4ha (a, b, sum, car) ;
input a,b;
output sum,car;
assign sum = a ^ b;
assign car = a & b;
endmodule
```

Half Subtractor

```
module lab4hs (a,b, dif, bor) ;
input a,b;
output dif, bor;
assign dif = a ^ b;
assign bor = (~a & b);
endmodule
```

**RTL Schematic**

Half Adder

![Screenshot (51)](https://github.com/user-attachments/assets/5d676eb9-ede1-4d2f-916e-91f582672aa9)

Half Subtractor

![Screenshot (54)](https://github.com/user-attachments/assets/c2ca7320-c408-4e96-860d-fa7de109af5c)


**Output/TIMING Waveform**

Half Adder

![Screenshot (52)](https://github.com/user-attachments/assets/61e4890e-89ef-4370-bef1-396a528d56da)

Half Subtractor


![Screenshot (55)](https://github.com/user-attachments/assets/f46b717b-7485-4b63-8085-e78d4a9c1dd4)


**Result:**

Successfully designed a half adder and half subtractor circuit and verified its truth table in Quartus using Verilog programming.
