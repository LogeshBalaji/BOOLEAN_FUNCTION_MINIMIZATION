# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.
![WhatsApp Image 2025-04-23 at 8 46 02 PM](https://github.com/user-attachments/assets/8f5486e3-3cd7-4c7d-8c4d-77dfb2fc8a09)
![WhatsApp Image 2025-04-23 at 8 46 03 PM](https://github.com/user-attachments/assets/9f5b3c02-3f17-4b03-8f53-757e65ba448a)
![WhatsApp Image 2025-04-23 at 8 46 03 PM (1)](https://github.com/user-attachments/assets/edbbb4b2-8c7c-4dbf-9595-39c4a7637f6c)


**Program:**

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
```
Developed by: Logesh B
RegisterNumber:212224110034
```
## F1
```.py
module logic_circuit (
    input wire A,
    input wire B,
    input wire C,
    input wire D,
    output wire F1
);

    assign F1 = (~B & ~D) | (~A & B & D) | (A & B & ~C);

endmodule
```
## F2
```.py
module logic_expression (
    input wire x,
    input wire y,
    input wire z,
    input wire w,
    output wire F
);

    assign F = (~y & z & ~w) | (x & z) | (y & x) | (w & z) | (w & y);

endmodule
```
**Logic symbol & Truthtable:**
## F1
![Screenshot 2025-04-23 210423](https://github.com/user-attachments/assets/efb82b4c-362e-4dd4-8d47-b114b3c7f30e)
## F2
![Screenshot 2025-04-23 210608](https://github.com/user-attachments/assets/7e3d7419-2d72-4b8c-b3ee-f07fe40fd4c3)

**RTL realization**
## F1
![Screenshot 2025-04-23 203143](https://github.com/user-attachments/assets/fd1fb6bb-1a91-42ee-9af8-b7d89551eaf5)
## F2
![Screenshot 2025-04-23 204027](https://github.com/user-attachments/assets/9800d370-a3ab-44f6-81ca-ec4073b0b72c)

**Output:**
## F1
![Screenshot 2025-04-23 203623](https://github.com/user-attachments/assets/a7b139a1-8e09-47e5-ac50-4b9fe5bd8b9a)
## F2
![Screenshot 2025-04-23 204342](https://github.com/user-attachments/assets/dbaf2030-fce1-44ca-a7c6-05d5f23bdde1)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
