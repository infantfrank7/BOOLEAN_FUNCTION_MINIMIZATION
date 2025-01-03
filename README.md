Developed by:  S Infant Jesus

RegisterNumber: 24001856


# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
module exp1(A, B, C, D, W, X, Y, Z, F1, F2);

input A, B, C, D,W,X,Y,Z;

wire x1, x2,x3,x4, x5, x6, x7, x8, x9, x10;

output F1, F2;

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

**Logic Diagram**

![exp2 logic gates](https://github.com/user-attachments/assets/e912039a-441e-4d70-abc7-ccfe13349a47)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 




**RTL realization**

![EXP2 GATES](https://github.com/user-attachments/assets/979b5551-36f8-4db9-b999-75f8619cad92)

**Output:**

![EXP2 WAVEFORM](https://github.com/user-attachments/assets/d342cffd-3b2f-4f19-8225-ce38f5f1cd06)

**RTL**

![EXP2 CODE](https://github.com/user-attachments/assets/6fdc621b-25c0-4f4a-8e9d-798875b4e6fa)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
