# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
*
Boolean Algebra is a branch of algebra that deals with boolean values—true and false. It is fundamental to digital logic design and computer science, providing a mathematical framework for describing logical operations and expressions

**Logic Diagram**

![logic symbol and truth table](https://github.com/user-attachments/assets/f45bfccb-52ce-4c2a-bb03-aeb42d0c9e8b)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: P SIRISHA RegisterNumber: 24002102 */
```
module fun2a(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
```
```
module fun2b(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y&z)|(w&y)|(x&y));
endmodule
```


**Output:**

![ex 2 wave](https://github.com/user-attachments/assets/653f4479-ef3e-40ea-a5b6-e3613cff315a)
![ex 2b wave](https://github.com/user-attachments/assets/885ad502-51c8-4344-a907-f4e969ea3516)

**RTL**

![ex 2a](https://github.com/user-attachments/assets/e5aade9d-8b8b-4b6f-8f62-eb26f6738502)
![ex 2b](https://github.com/user-attachments/assets/28207677-47a0-4eac-86a5-253bd4b5a2fc)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

