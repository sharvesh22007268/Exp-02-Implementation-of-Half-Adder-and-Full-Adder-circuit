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
```
Program:
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: V.Sharvesh
RegisterNumber:  212222050056

## HALF ADDER :
module exp3(A,B,c,s);
input A,B;
output s,c;
assign s=A^B;
assign c=A&B;
endmodule

## FULL ADDER
module exp03(A,B,c,sum,carry);
input A,B,c;
output sum,carry;
assign sum=A^B^c;
assign carry=((A&B)|(B&c)|(c&A));
endmodule
```
Developed by: 
RegisterNumber:  
*/
Logic symbol & Truthtable
RTL realization

### Output:
### HALF ADDER RTL  :
![image](https://github.com/sharvesh22007268/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/143207601/0ea8742e-6e4a-49ab-bbbe-1bf08fe31162)

### HALF ADDER WAVEFORM :
![image](https://github.com/sharvesh22007268/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/143207601/79720e1d-b97f-4f5a-b255-2eae517a253b)

### HALF ADDER TRUTH TABLE :
![image](https://github.com/sharvesh22007268/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/143207601/651c6c24-e561-409c-a4f6-6bf4d7aca84b)

### FULL ADDER RTL  :
![image](https://github.com/sharvesh22007268/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/143207601/131ade68-c7c5-4e07-b6b1-846b58fea92e)

### FULL ADDER WAVEFORM :
![image](https://github.com/sharvesh22007268/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/143207601/20d55e92-c2bc-4c1f-b8be-9a64e5f43ca9)

### FULL ADDER TRUTH TABLE :
![image](https://github.com/sharvesh22007268/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/143207601/530738b2-ea3e-4082-bdcb-8139f963b3dc)

### Result:
