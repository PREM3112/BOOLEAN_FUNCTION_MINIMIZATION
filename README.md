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
 

## Developed by:PREM.R
## RegisterNumber:212223240124
```
module combinationalcircuit(A,B,C,D,F1);
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
```


**RTL realization**
![Screenshot 2024-04-01 184059](https://github.com/PREM3112/BOOLEAN_FUNCTION_MINIMIZATION/assets/145449383/a5170256-982a-48a6-9687-67dcddbde139)


**Output:**

**RTL**
![Screenshot 2024-04-01 184121](https://github.com/PREM3112/BOOLEAN_FUNCTION_MINIMIZATION/assets/145449383/ee3bb1de-5a91-455c-8de4-4d4e8aa10016)


**Timing Diagram**
![Screenshot 2024-04-01 184136](https://github.com/PREM3112/BOOLEAN_FUNCTION_MINIMIZATION/assets/145449383/2b2624b5-03e6-4c9c-93d3-d0bd3cd58710)


**Result:**
Thus the output got successfully.

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

