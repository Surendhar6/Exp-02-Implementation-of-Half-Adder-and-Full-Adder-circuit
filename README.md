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
module HSub (a,b,sum,carry);
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
![Screenshot_20230106_034616](https://user-images.githubusercontent.com/118352907/211159006-47a07560-b8a9-4db1-86ed-0667383a9f2b.png)
![Screenshot_20230106_042624](https://user-images.githubusercontent.com/118352907/211159020-4f10d24d-56ce-467d-a266-d3e29143b570.png)

### TIMING DIAGRAM
![Screenshot_20230106_035147](https://user-images.githubusercontent.com/118352907/211159034-da6e81fd-0e8e-4f52-94e7-0050b4777cef.png)
![Screenshot_20230106_043301](https://user-images.githubusercontent.com/118352907/211159044-4ce62876-d986-4c77-b387-2234282a7298.png)

### TRUTH TABLE 
![Screenshot_20230107_092638](https://user-images.githubusercontent.com/118352907/211159575-0241472d-029c-416f-bc9a-195a5385b578.png)
![Screenshot_20230107_092650](https://user-images.githubusercontent.com/118352907/211159586-37ce7a19-3d04-4b0e-8236-6c8567d95fd8.png)

### Result:
Thus the half adder and full adder circuits are designed and the truth tables are verified using quartus software.
