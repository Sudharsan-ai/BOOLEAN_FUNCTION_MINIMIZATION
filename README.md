# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory :**

Boolean Algebra is a branch of algebra that deals with boolean values—true and false. It is fundamental to digital logic design and computer science, providing a mathematical framework for describing logical operations and expressions

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

F1:
```
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule


```
F2:

```
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule

```


/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: SUDHARSAN S RegisterNumber:24900437



**RTL realization**


F1:

![WhatsApp Image 2024-11-29 at 14 25 52_90281635](https://github.com/user-attachments/assets/c2426bf5-3854-4e1b-8c9e-d9321bd37415)


![Screenshot 2024-11-29 133213](https://github.com/user-attachments/assets/269c12dc-304f-4e17-a15f-6c61a4a76d36)

F2:

![WhatsApp Image 2024-11-29 at 14 26 40_a40d5d91](https://github.com/user-attachments/assets/a6764beb-fc93-494a-a2af-486f04f29bb3)


![Screenshot 2024-11-29 133329](https://github.com/user-attachments/assets/843dbd46-dd0b-4c1c-8ec7-49af8f78fedf)

**Output:**



**RTL**

**Timing Diagram :**

F1:

![WhatsApp Image 2024-11-29 at 14 26 09_16c0221f](https://github.com/user-attachments/assets/8105e5fb-113d-44aa-8d9e-c40011249265)

F2:

![WhatsApp Image 2024-11-29 at 14 26 47_89927366](https://github.com/user-attachments/assets/fd1ca882-9bf8-4902-abb7-3429114452f2)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

