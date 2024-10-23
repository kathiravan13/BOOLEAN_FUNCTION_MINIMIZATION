# BOOLEAN_FUNCTION_MINIMIZATION
### AIM:

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

### Theory

### Logic Diagram

### Procedure

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


### Program:
### Developed by: kathiravan
###  Registered number : 212222230063
Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 


```
module ex02(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d) | (a & b & ~c) | (~a & b & d));
endmodule
```
```
module ex02m1(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2= ((~y&z)|(w&y)|(x&y));
endmodule
```
### Logic Symbol & Truth Table 


![image](https://github.com/user-attachments/assets/7df010aa-4cf8-438a-bd30-5b79a220de04)


*F2*

![image](https://github.com/user-attachments/assets/2c174f66-6675-48ce-83c3-1e00840dcee1)





### RTL realization

*F1*
![image](https://github.com/user-attachments/assets/e9404872-b844-40f9-bdea-41da2768f7b8)

*F2*
![image](https://github.com/user-attachments/assets/3174f551-f14d-4b59-bb16-ed27e4436244)


### Output:
*F1*
![image](https://github.com/user-attachments/assets/a6b2de91-c02d-4bb5-9f42-db9e168d0611)

*F2*
![image](https://github.com/user-attachments/assets/5ad1ecc7-e1e3-4352-9f83-298cd33bb95b)

### Result:

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

