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
~~~
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
~~~

**RTL realization**


**Output:**

**RTL**
![image](https://github.com/user-attachments/assets/39ff5764-c77b-489f-9747-a965604f2963)

**Timing Diagram**
![image](https://github.com/user-attachments/assets/d1fb97c0-fa42-4640-81e2-fc0f409610a4)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

