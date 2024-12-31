# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Logic Diagram**
![boolean func](https://github.com/user-attachments/assets/b60551a8-8c93-44df-bfaf-637aedcef769)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:Priyan U RegisterNumber:24900703*/
```
f1
```
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

```
f2
```
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule

```

**RTL realization**




![f1](https://github.com/user-attachments/assets/5655f823-98ae-4540-abee-874651eac3da)







![f2](https://github.com/user-attachments/assets/e9177c25-859e-4fe6-a27d-327ed4a2742e)






**Timing Diagram**





![f1 (2)](https://github.com/user-attachments/assets/addcc60a-bb4d-427d-8c19-3d6131776460)






![f2 (2)](https://github.com/user-attachments/assets/d60690e2-a159-4c73-98c9-045d505f7da3)






**Result:**





Thus the given logic functions are implemented using and their operations are verified using Verilog programming.






