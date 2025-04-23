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
```````
Developed by: RegisterNumber:212223230061

 module exp_2(A,B,C,D,F1);
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
````````
**RTL realization**

![image](https://github.com/user-attachments/assets/72709309-e3c6-4677-83aa-7a254b0b8f91)

 ## TRUTH TABLE
 ![image](https://github.com/user-attachments/assets/c0b17d8d-d746-4f7b-b379-1fa54dfcc8c4)

**Timing Diagram**
![image](https://github.com/user-attachments/assets/853995fb-c9f6-43cd-b208-28780295134e)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

