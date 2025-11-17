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



**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.


Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**

**Procedure**
1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.





**Program:**
module fulls(a,b,c,diff,borrow);
input a,b,c;
output diff,borrow;
xor g1(diff,a,b,c);
assign borrow=((~a&c)|(~a&b)|(b&c));
endmodule 


/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. Developed by:Suwetha T RegisterNumber:25002663
*/

**RTL Schematic**

<img width="1389" height="754" alt="Screenshot 2025-11-17 133754" src="https://github.com/user-attachments/assets/48a2ec3c-7d1f-4de9-b580-67a8b476835e" />

<img width="1375" height="706" alt="Screenshot 2025-11-17 135300" src="https://github.com/user-attachments/assets/e39fb6a0-6285-4ef2-97b5-baab8ff1d899" />


**Output Timing Waveform**

<img width="1897" height="875" alt="Screenshot 2025-11-17 134043" src="https://github.com/user-attachments/assets/422a51c0-4b2f-417a-b634-c863c88d25f7" />

<img width="1889" height="851" alt="Screenshot 2025-11-17 135458" src="https://github.com/user-attachments/assets/bb4b7f3d-346f-4031-b63a-da76067a19e1" />


**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



