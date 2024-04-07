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
```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,X,Y,Z;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output F1,F2;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign x6=(X)&(~Y)&(Z);
assign x7=(~X)&(~Y)&(Z);
assign x8=(~W)&(X)&(Y);
assign x9=(W)&(~X)&(Y);
assign x10=(W)&(X)&(Y);
assign F1=x1|x2|x3|x4|x5;
assign F2=x6|x7|x8|x9|x10;
endmodule

Developed by:  NARASIMHAN S
Register Number:212223230133
```

### Logic symbol & Truthtable:
![Screenshot 2024-04-07 210020](https://github.com/Narasimhan05/BOOLEAN_FUNCTION_MINIMIZATION/assets/132819871/83997615-4dda-4349-84dc-635556d820da)
![image](https://github.com/Narasimhan05/BOOLEAN_FUNCTION_MINIMIZATION/assets/132819871/fdd19215-d235-4a94-8ce3-4686e05e9524)

### RTL realization
![image](https://github.com/Narasimhan05/BOOLEAN_FUNCTION_MINIMIZATION/assets/132819871/fb6bf7d0-777f-4398-b7de-60bb400c599a)

**Output:**
![image](https://github.com/Narasimhan05/BOOLEAN_FUNCTION_MINIMIZATION/assets/132819871/8e49c421-4121-4701-b665-093c0acdd52b)

### Result:

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

