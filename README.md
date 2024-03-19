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
```
1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.
```

**Program:**
```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: Kanimozhi P
RegisterNumber:212222230060
module (A,B,C,D,F1);
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
**Logic Gate**

![exp 2](https://github.com/ahalyaselvakumar/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870759/32c1d4ce-952b-4d79-a231-52d75800d4e8)
**Waveform**

![screenshot 2024-03-15 084324](https://github.com/ahalyaselvakumar/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870759/69156394-d6ad-4d4d-9db9-1bdc2d49aec1)
**Truth Table**

![screenshot 2024-03-15 0842323](https://github.com/ahalyaselvakumar/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870759/2b485e40-1b92-4d24-9d5f-d4be448a5c5a)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

