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

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by:P.Kevin

RegisterNumber:24901145*/

**Half Adder**

module Experiment3a(a,b,sum,carry);

input a,b;

output sum,carry;

assign sum= (a ^ b);

assign carry= ( a & b);

endmodule

**Half Subtractor**

module Experiment3b(a,b,difference,borrow);

input a,b;

output difference,borrow;

assign difference= (a ^ b);

assign borrow= ( ~a & b);

endmodule


**RTL Schematic**

**Half Adder**

![Screenshot 2024-11-23 103551](https://github.com/user-attachments/assets/add8bd7f-2627-4d3e-b629-f10b81c43e9b)

**Half Subtractor**

![Screenshot 2024-11-23 104349](https://github.com/user-attachments/assets/01767356-3e8a-4e74-943f-61e22573f104)


**Output/TIMING Waveform**

**Half Adder**

![Screenshot 2024-11-23 103752](https://github.com/user-attachments/assets/371b402d-5790-43cb-a3eb-1f5217dbab8a)


**Half Subtractor**

![Screenshot 2024-11-23 104510](https://github.com/user-attachments/assets/30cc9c3b-373c-465e-9114-e9da35ecbabe)


**Result:**

Thus the Half adder and Half subtractor are studied and truth table is verified
