# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

Boolean Algebra is a branch of algebra that deals with boolean values—true and false. It is fundamental to digital logic design and computer science, providing a mathematical framework for describing logical operations and expressions

**Logic Diagram**

i)F1 TRUTHTABLE:


![Screenshot 2024-12-13 123617](https://github.com/user-attachments/assets/0aa6fb4c-2e02-44bb-af7d-b9dc5bd65deb)


ii)F2 TRUTHTABLE

![Screenshot 2024-12-13 123722](https://github.com/user-attachments/assets/a657a6f1-71ae-4537-9968-6680b255a37c)

**Boolean minimization**


![Screenshot 2025-01-03 134957](https://github.com/user-attachments/assets/545a879a-65e9-4e63-8fd3-060ec450f528)


![Screenshot 2025-01-03 135015](https://github.com/user-attachments/assets/afb48d07-0485-46fe-bda1-ba6cda13354a)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: MUKESH R

RegisterNumber:24000238
*/
```
i)
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

ii)
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));0
endmodule
```


**RTL**


![exp02f1 (2)](https://github.com/user-attachments/assets/962a8988-afc7-4c4a-991f-dca4c34c730e)


![exp02f2](https://github.com/user-attachments/assets/722cd00a-e640-4039-9e44-a52e5be266c0)

**Output:**


![output 02](https://github.com/user-attachments/assets/09de79e3-0b7c-4283-bbb2-56ef55bd1bdc)


![output 2-2](https://github.com/user-attachments/assets/68d16a35-754b-443a-b38a-082c0139a35c)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

