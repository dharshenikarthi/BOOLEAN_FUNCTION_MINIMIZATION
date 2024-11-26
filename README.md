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
module bool(a,b,c,d,w,x,y,z,f1,f2); input a,b,c,d,w,x,y,z; wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output f1,f2; assign x1=(~a)&(~b)&(~c)&(~d); assign x2=(a)&(~c)&(~d); assign x3=
(~b)&(c)&(~d); assign x4=(~a)&(b)&(c)&(d); assign x5=(b)&(~c)&(d); assign x6=(x)&
(~y)&(z); assign x7=(~x)&(~y)&(z); assign x8=(~w)&(x)&(y); assign x9=(w)&(~x)&(y);
assign x10=(w)&(x)&(y); assign f1=x1|x2|x3|x4|x5; assign f2=x6|x7|x8|x9|x10; endmodule

Developed by:Dharsheni.K RegisterNumber:24006589*/


**RTL realization**

![Screenshot 2024-11-26 142952](https://github.com/user-attachments/assets/135437b1-8c7c-4147-adb9-73e188232413)

**Output:**

![Screenshot 2024-11-26 142936](https://github.com/user-attachments/assets/d2f88b38-bd4f-4fad-b72b-30798ea7c488)

**RTL**

![Screenshot 2024-11-26 143200](https://github.com/user-attachments/assets/bc75ae42-ab7a-433a-a7b5-199f6ffdeb39)

![Screenshot 2024-11-26 143221](https://github.com/user-attachments/assets/3f7200fa-ce9e-4a80-a218-0c2a988a26df)

**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

