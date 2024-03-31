# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

## AIM:

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

## Full Adder and Full Subtractor

## Full Adder

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

## Figure -1 FULL ADDER

## Full Subtractor

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

## Truthtable


## Procedure

Write the detailed procedure here

### Program: Aim is to bulid a full adder and full subtractor using quartus
### Developed by: Vikamuhan reddy.N
### RegisterNumber:212223240181

Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.

## Full Adder:
```c
module exp3fa(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum a^b^cin;
assign carry =(a&b)|((a^b)&cin);
endmodule;
```



## Full Subtractor
```c
module exp4fs(a,b,bin,diff,borr);
input a,b,bin;
output diff,borr;
assign diff=a^b^bin;
assign borr=((~a)&b)|(b&bin)|((~a)&bin);
endmodule;
```

## RTL Schematic

## Full Adder:
![image](https://github.com/vikamuhan-reddy/FULL_ADDER_SUBTRACTOR/assets/144928933/8e385343-0fe0-467e-9ce5-c4188bf6ed5a)


## Full Subtractor
![image](https://github.com/vikamuhan-reddy/FULL_ADDER_SUBTRACTOR/assets/144928933/61fb99c9-4555-45c4-a46c-40cc0bf8fd02)



## Output Timing Waveform

## Full Adder:
![image](https://github.com/vikamuhan-reddy/FULL_ADDER_SUBTRACTOR/assets/144928933/582c8661-cd73-4549-9ccb-0c3b542c43b8)



## Full Subtractor

![image](https://github.com/vikamuhan-reddy/FULL_ADDER_SUBTRACTOR/assets/144928933/ba12b568-63e9-4922-8bdb-38969485e21b)


## Result:

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



