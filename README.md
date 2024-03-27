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
Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

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

**RTL realization**

![Screenshot 2024-03-27 101125](https://github.com/saniyaganesamoorthy/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742583/1ea99d16-0a27-4888-bc05-2f2e5d074646)

**Time Table**

![Screenshot 2024-03-27 101159](https://github.com/saniyaganesamoorthy/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742583/7c712ac5-db10-4fa0-84e8-279c03480df0)


**Timing Diagram**
![Screenshot 2024-03-27 101237](https://github.com/saniyaganesamoorthy/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742583/8e17a916-b6d8-4b39-9859-8c395734a36b)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

