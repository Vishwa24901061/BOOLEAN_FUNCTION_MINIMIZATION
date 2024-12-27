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

**Truthtable**

i)F1 TRUTHTABLE:


![Screenshot 2024-12-16 081905](https://github.com/user-attachments/assets/7f7f03cf-a4e8-4fa1-b577-3d54e3f5ce66)

ii)F2 TRUTHTABLE:


![Screenshot 2024-12-16 081944](https://github.com/user-attachments/assets/cb697db9-b680-4361-aeea-0f66a051265b)

**boolean minimization**

i)F1 

![boolean minimization 1](https://github.com/user-attachments/assets/052e552e-6356-41c8-bccd-a9ba4afd4f44)

ii)F2


![boolean minization 2](https://github.com/user-attachments/assets/36e1d04d-e4c0-41fd-be28-e8bbcf4ae1a4)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: vishwa v

RegisterNumber:24901061
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

i)F1 


![Screenshot 2024-12-16 082201](https://github.com/user-attachments/assets/32891e57-61f9-4bc2-b385-613f9592aae6)

ii)F2


![Screenshot 2024-12-16 082208](https://github.com/user-attachments/assets/6489de61-47ac-481f-b1ce-9a79aa0d5ad1)

**Output:**

i)F1 


![Screenshot 2024-12-16 082229](https://github.com/user-attachments/assets/cd30630f-14f4-4044-856f-920c65a021df)


ii)F2


![Screenshot 2024-12-16 082250](https://github.com/user-attachments/assets/00323f93-b83a-4b18-99c4-8c4a410f0ea3)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

