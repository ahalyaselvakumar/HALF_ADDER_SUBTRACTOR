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
## Half adder:
![half adder](https://github.com/ahalyaselvakumar/HALF_ADDER_SUBTRACTOR/assets/144870759/7d719732-8afa-4325-9a39-5c6dc0c4013f)

## Half subtractor:
![half subtractor](https://github.com/ahalyaselvakumar/HALF_ADDER_SUBTRACTOR/assets/144870759/9ccc3b69-f7ed-452e-8b2a-7a0d02f96469)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: AHALYA S
RegisterNumber: 212223230006

## Half Adder
```
module exp3(sum, carry,a,b); 
input a,b; 
output sum,carry; 
xor sum1(sum,a,b); 
and carry1(carry,a,b); 
endmodule
```
## Half Subtractor
```
module exp3(diff,carry,a,b);
input a,b;
output diff,carry;
xor(diff,a,b);
assign carry=(~a)&b;
endmodule
```

**RTL Schematic half adder:**
![rtl](https://github.com/ahalyaselvakumar/HALF_ADDER_SUBTRACTOR/assets/144870759/47c22c93-7417-4dd3-9e16-539a8b54c708)

**Half subtractor:**
![half sub rtl](https://github.com/ahalyaselvakumar/HALF_ADDER_SUBTRACTOR/assets/144870759/0de4bae7-9be6-4cbc-a949-969a5ac0e69e)


**Output/TIMING Waveform**
## Half adder:
![op half adder](https://github.com/ahalyaselvakumar/HALF_ADDER_SUBTRACTOR/assets/144870759/7ff34afb-8c7b-4c94-9810-9f306740a051)

## Half subtractor:
![op half sub](https://github.com/ahalyaselvakumar/HALF_ADDER_SUBTRACTOR/assets/144870759/db531f9c-96d3-47d8-9e0a-ecaa02d5b453)


**Result:**
Thus the half subtractor and half adder circuits are designed and the truth tables are verified using quartus software
