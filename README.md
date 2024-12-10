# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

Boolean Algebra is a branch of algebra that deals with boolean values—true and false. It is fundamental to digital logic design and computer science, providing a mathematical framework for describing logical operations and expressions

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.

**Truthtable**


i)F1 TRUTHTABLE:

![exp02f1 truthtable](https://github.com/user-attachments/assets/84a81658-86b7-4060-a978-9d1b1670dc17)


ii)F2 TRUTHTABLE

![exp02f2truthtable](https://github.com/user-attachments/assets/269a5435-8b24-4d0d-a0f6-9fffbdd336d4)


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:Tharun R

RegisterNumber:24005919
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


![exp02f1 (2)](https://github.com/user-attachments/assets/4bd27e78-943d-4acd-abf4-aaa58665b7d9)



![exp02f2](https://github.com/user-attachments/assets/69d95b47-57a7-487b-bace-cb700d84c24b)

**Timing Diagram**


![output 02](https://github.com/user-attachments/assets/766139d9-38f8-42b3-9013-4a14b22180fd)



![output 2-2](https://github.com/user-attachments/assets/56939dcf-32a9-4fbc-aad4-6ec14d5990d2)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

