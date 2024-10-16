# BOOLEAN_FUNCTION_MINIMIZATION

*AIM:*

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

*Equipment Required:*

Hardware – PCs, Cyclone II , USB flasher

*Software – Quartus prime*

*Theory*

*Logic Diagram*

*Procedure*

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


## Program:

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: kathiravan

RegisterNumber: 212222230063

*/


module boolean_fun(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u,v,w1,w2,x1,x2,y1,y2,z1,z2;
not(adash,a);
not(bdash,b);
not(cdash,c);
not(ddash,d);
not(ydash,y);
and(p,bdash,ddash);
and(q,adash,b,d);
and(r,a,b,cdash);
or(f1,p,q,r);

and(w1,a,b,c);
and(w2,~a,~b,~c);
or(f2,w1,w2);
endmodule



## RTL realization:

*Output:*
![313560946-5de811ea-88d2-4110-9c32-1500f1af436c](https://github.com/Keerthi-Vasan-Adhithan/BOOLEAN_FUNCTION_MINIMIZATION/assets/107488929/348cd21b-bcc4-4d44-a425-f64f9fb056ae)


![313560653-408a4deb-3ddb-4789-9b64-aa5445cd7992](https://github.com/Keerthi-Vasan-Adhithan/BOOLEAN_FUNCTION_MINIMIZATION/assets/107488929/78f443f6-f744-4a6a-8f8f-50a14e716ee9)


*Result:*

Thus the given logic functions are implemented using and their operations are verified using Verilog programming
