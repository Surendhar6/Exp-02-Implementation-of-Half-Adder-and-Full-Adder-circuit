# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

module Hsub(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b); 
and(carry,a,b);
endmodule

module FAdd (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = ((a^b)^c);
assign carry = ((a&b)|(b&c)|(c&a));
endmodule

Developed by: Surendhar A
RegisterNumber:  22009022
*/
Logic symbol & Truthtable
RTL realization

### Output:
### RTL
![Screenshot_20230106_034616](https://user-images.githubusercontent.com/118352907/210993278-f9ec176c-1ef8-491f-b305-4be7b940a40f.png)
 ![Screenshot_20230106_042624](https://user-images.githubusercontent.com/118352907/210999051-9f3fead1-075f-46c3-940d-10aa255ff01f.png)

### TIMING DIAGRAM
![Screenshot_20230106_035147](https://user-images.githubusercontent.com/118352907/210993366-c26a8aa0-311c-4aca-9a62-1b16b3a72208.png)
![Screenshot_20230106_043301](https://user-images.githubusercontent.com/118352907/211000110-c32ffac8-5e54-4bd1-9e62-0f002286440a.png)

### TRUTH TABLE 
### Result:
Thus the half adder and full adder circuits are designed and the truth tables is verified using quartus software.
