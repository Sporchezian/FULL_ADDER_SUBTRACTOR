# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**
FULL ADDER:
<img width="1335" height="981" alt="Screenshot 2025-11-18 202321" src="https://github.com/user-attachments/assets/d6110bb3-a2d7-4da2-9b4a-de7cc0a6b524" />

FULL SUBTRACTOR:
<img width="1341" height="968" alt="Screenshot 2025-11-18 202348" src="https://github.com/user-attachments/assets/52dc6674-204a-4148-aa78-7fc7cf56807c" />

**Procedure**

Write the detailed procedure here

**Program:**

Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. 

Developed by: PORCHEZIAN S 

RegisterNumber:25017994

FULL ADDER:
```
module exp4a(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=a^b^c
assign carry=(a&b)|(b&c)|(c&a);
endmodule
```
FULL SUBTRACTOR:
```
module exp4b(a,b,cin,diff,borr);
input a,b,cin;
output diff,borr;
assign diff=(~a)&c|b&c|(~a)&b;
assign borr=a^b^c;
endmodule
```
**RTL Schematic**

FULL ADDER:
<img width="1735" height="846" alt="Screenshot 2025-11-18 114018" src="https://github.com/user-attachments/assets/bcd71cb5-692c-4dbc-a9aa-d731e42ac169" />

FULL SUBTRACTOR:
<img width="1708" height="827" alt="Screenshot 2025-11-18 115150" src="https://github.com/user-attachments/assets/cc253ab9-e8af-47a2-ab8a-a7b0e53b0466" />

**Output Timing Waveform**

FULL ADDER:
<img width="1919" height="362" alt="Screenshot 2025-11-18 114426" src="https://github.com/user-attachments/assets/e52eeb12-c8c5-40a1-abd2-605c5152ce99" />

FULL SUBTRACTOR:
<img width="1906" height="335" alt="Screenshot 2025-11-18 115704" src="https://github.com/user-attachments/assets/403e7bc9-54af-41e6-bed8-34179f6ded04" />

**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



