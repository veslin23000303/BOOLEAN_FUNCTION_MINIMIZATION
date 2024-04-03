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
~~~
module exp2(A,B,C,D,F1);
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
~~~

Developed by:  VESLIN ANISH A

RegisterNumber: 212223240175


**RTL realization**
![image](https://github.com/veslin23000303/BOOLEAN_FUNCTION_MINIMIZATION/assets/151148539/58d77dfa-ffac-4db9-bb83-14e39a416130)


**Truth Table**

![image](https://github.com/veslin23000303/BOOLEAN_FUNCTION_MINIMIZATION/assets/151148539/762980b5-90fe-4bd0-9e7e-d14fddd54424)

**Timing Diagram**
![image](https://github.com/veslin23000303/BOOLEAN_FUNCTION_MINIMIZATION/assets/151148539/ffc733cd-f926-4f7f-bcc6-a5ab7cc944d5)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

