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
![{659362BA-E356-4EF2-AA23-8074BA572C44}](https://github.com/user-attachments/assets/0f7ebfba-6cd6-4b52-9e63-07bf9c633d47)
![{74371027-2206-45D4-B16E-B2E248B47EAD}](https://github.com/user-attachments/assets/bc616def-fd35-4964-b99b-22c2b45c5e3f)

**Procedure**

Write the detailed procedure here

**Program:**
i)FULL ADDER

module fa(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=( (a ^ b)^c);
assign carry= ( (a & b)| ( cin &(a ^ b ));
endmodule

ii)FULL SUBTRACTOR

module fs(a,b,difference,borrow);

input a,b,bin;

output difference,borrow;

assign difference= ( (a ^ b)^bin);

assign borrow = ( ( a & b )| ( bin & ((a ^ b )));

endmodule


/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. Developed by: SANTHOSH V
RegisterNumber:24005918
*/

**RTL Schematic**
FULL ADDER
![{2376CF6B-C00C-4517-A35F-A3B5111F88DA}](https://github.com/user-attachments/assets/9adc55bb-f248-42c7-8aea-c14d72c89a95)

FULL SUBRACTOR
![{54D7AE82-4EC3-4BEE-8CFF-53909062784A}](https://github.com/user-attachments/assets/48f597ca-058d-4f42-8cc2-59c147996423)

**Output Timing Waveform**
FULL ADDER
![{8251A3E7-1E09-489E-B7E7-8A74C25B9339}](https://github.com/user-attachments/assets/4e1147f7-358e-449f-88a9-b5c2de43b9f2)

FULL SUBRACTOR
![{F39676B5-BD02-4386-B9E9-BA9C4A78917D}](https://github.com/user-attachments/assets/6981e672-6d48-4a35-ab40-ec7ca25dcd1d)



**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



