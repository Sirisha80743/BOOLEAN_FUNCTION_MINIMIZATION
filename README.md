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

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.

**Minimization**

F1
![F1](https://github.com/user-attachments/assets/c9933c93-e6c0-487f-847c-eee48ac91267)

F2
![F2](https://github.com/user-attachments/assets/598f9acc-77c1-4fd3-86dd-efccded8a543)

**Truth table**

![TRUTH TABLE_page-0001](https://github.com/user-attachments/assets/c4a572cb-c37b-44ac-90d0-a9674ecbbab3)

**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: P Sirisha RegisterNumber:24002102

F1

```
module fun2a(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
```

F2

```
module fun2b(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y&z)|(w&y)|(x&y));
endmodule
```

**RTL**

F1

![ex 2a](https://github.com/user-attachments/assets/62bae329-672c-4a3f-b7b4-b4c65b2d7646)

F2

![ex 2b](https://github.com/user-attachments/assets/43dd96e2-ac21-4b5e-b299-a4022ebc00de)

**Output:**

F1

![ex 2 wave](https://github.com/user-attachments/assets/cdb8949a-0028-43a3-ae45-e2c0c015aadf)

F2

![ex 2b wave](https://github.com/user-attachments/assets/848f02b4-0e3e-4ae7-b617-39f2126c15cb)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

