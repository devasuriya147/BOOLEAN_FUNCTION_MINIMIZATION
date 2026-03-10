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


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
```
Developed by:DEVASURYA M
RegisterNumber:212225230048
module exp2(w,x,y,z,a,b,c,d,f1,f2);
input w,x,y,z,a,b,c,d;
output f1,f2;
assign f1=(~a&~b&~c&~d)|(a&~c&~d)|(~b&c&~d)|(~a&b&c&d)|(b&~c&d);
assign f2=(x&~y&z)|(~x&~y&z)|(~w&x&y)|(w&~x&y)|(w&x&y);
endmodule
```
**truth table:**
<img width="1012" height="556" alt="Screenshot 2026-03-10 201334" src="https://github.com/user-attachments/assets/908cb5dc-e81d-47ce-a76d-f64b22d887b8" />
<img width="1006" height="542" alt="Screenshot 2026-03-10 201344" src="https://github.com/user-attachments/assets/120a870d-4e10-48b9-b477-1d8103d59e29" />




**RTL realization**
<img width="1898" height="1038" alt="Screenshot 2026-03-10 201050" src="https://github.com/user-attachments/assets/dfb5467e-1d90-46e3-a195-200aaa6c4b1b" />

**Timing Diagram**
<img width="1906" height="963" alt="Screenshot 2026-03-10 191222" src="https://github.com/user-attachments/assets/2c4e1c00-c47c-4dc1-a5b2-b2e98e1e83d3" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

