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
FULL ADDER
<img width="652" height="476" alt="Screenshot 2025-11-20 200555" src="https://github.com/user-attachments/assets/3caabeba-733e-49bb-a7ae-d8fc2e46f5c6" />
FULL SUBTRACTOR
<img width="661" height="480" alt="Screenshot 2025-11-20 200539" src="https://github.com/user-attachments/assets/a7679eb8-88e4-428b-8c53-dc0081787205" />

**Procedure**

Write the detailed procedure here

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. 
```
module exp5 (a,b,c,x,y,z,sum,dif,car,bor);
input a,b,c,x,y,z;
output sum,dif,car,bor;
assign sum = a^b^c;
assign car = a&b | a&c | b&c;
assign dif = x^y^z;
assign bor = ~x&z | ~x&y | y&z;
endmodule
```
Developed by: RegisterNumber:Ashlin Sweety.R
25011333

**RTL Schematic**
<img width="871" height="741" alt="Screenshot 2025-11-20 195504" src="https://github.com/user-attachments/assets/735cf23d-6ffb-4c7e-9994-b462d17aeb07" />

**Output Timing Waveform**
<img width="1911" height="531" alt="Screenshot 2025-11-20 195834" src="https://github.com/user-attachments/assets/f291b6e4-e728-4ef1-80a2-eb2196ede3af" />

**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



