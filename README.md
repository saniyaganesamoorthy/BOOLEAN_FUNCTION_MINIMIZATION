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

Developed by: SANIYA G
RegisterNumber: 212223240147
```
module combinationalcircuit(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule
```
*/


**RTL realization**
![Screenshot 2024-03-27 101125](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742583/4512d741-7a60-44b3-ace4-f9601cc3f6b7)
**Time Table**
![Screenshot 2024-03-27 101159](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742583/18e1a651-c6d5-4eb2-99a6-85528b31e729)


**Timing Diagram**
![Screenshot 2024-03-27 101237](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742583/7fe7c2e6-b349-46a8-952e-2ab6c9991c59)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

