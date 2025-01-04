# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

Boolean Function Minimization is the process of reducing a Boolean expression to its simplest form without changing its functionality. This minimization reduces the number of gates and inputs required, optimizing circuit design.

Logic Gates: Fundamental building blocks like AND, OR, and NOT gates are used to implement Boolean expressions. Karnaugh Map (K-map): A graphical technique for minimizing Boolean expressions by grouping terms based on commonalities. The given Boolean functions can be minimized as follows:

F1 = A’B’C’D’ + AC’D’ + B’CD’ + A’BCD + BC’D The terms can be simplified using K-map techniques to reduce the complexity of the circuit. F2 = xy’z + x’y’z + w’xy + wx’y + wxy Similar simplification can be done for this function to reduce the gate count. The resulting minimized expressions are implemented using Verilog HDL and simulated on the Quartus Prime tool. The outputs can then be verified on an FPGA board (e.g., Cyclone II).

**Truth Table**

F1
![image](https://github.com/user-attachments/assets/ff4858a7-2217-4a79-8c6c-969c1adfb587)

F2
![image](https://github.com/user-attachments/assets/ad787bfe-c50d-45a1-86aa-a29c739f8162)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.

**BOOLEAN MINIMIZATION**

F1
![image](https://github.com/user-attachments/assets/b6d9457f-6e42-40d9-94a9-70a7e9dabcb3)

F2
![image](https://github.com/user-attachments/assets/d0751222-31a9-461c-b7f8-afb85a0cbc21)


**Program:**

```
i)F1
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

ii)F2
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));0
endmodule

```



**RTL realization**

F1
![image](https://github.com/user-attachments/assets/c4e5e3aa-1317-4492-b1c7-7015bee1c5dd)

F2
![image](https://github.com/user-attachments/assets/3f639924-363e-4f9c-bca8-2ea5fdadb83e)


**Timing Diagram**

F1
![image](https://github.com/user-attachments/assets/c68ebb94-7212-46eb-81a6-93cd25ba051e)
F2
![image](https://github.com/user-attachments/assets/8c8efb37-dab1-4933-a61f-5e3d9c7790d9)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

