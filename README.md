# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory:
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.

## Logic Diagram:
![Screenshot 2023-04-20 210203](https://user-images.githubusercontent.com/120115840/233415475-51f134a4-225b-4dee-95b1-5a9018edba1b.png)

## Procedure:
1.Create a project with required entities.

2.Create a module along with respective file name.

3.Run the respective programs for the given boolean equations.

4.Run the module and get the respective RTL outputs.

5.Create university program(VWF) for getting timing diagram.

6.Give the respective inputs for timing diagram and obtain the results.

## Program:
```
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by:Preethi.A.A
RegisterNumber:212222110035

module expf1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & d) | (~a & b & d) | (a & b &~c));
endmodule

module exp2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((x & y) | (~y & z) | (w & y));
endmodule 
*/
```
## OUTPUT:
## RTL realization:
F1:

![Screenshot (12)](https://user-images.githubusercontent.com/120115840/233417174-29afee92-f8e8-4ea0-92f3-b446e155ccc6.png)

F2:

![exp2 (2)](https://user-images.githubusercontent.com/120115840/233417345-1a7e715d-42ba-4cf3-b0ce-891063b6a06e.png)

## Timing Diagram:
F1:

![Screenshot 2023-04-13 115020](https://user-images.githubusercontent.com/120115840/233417783-24ec1b9d-28f6-4768-9935-848462aa091f.png)

F2:

![exp2](https://user-images.githubusercontent.com/120115840/233417917-ac2d39ba-fc52-492b-82e6-f8877c012136.png)

## TRUTH TABLE:

![Screenshot 2023-04-20 211242](https://user-images.githubusercontent.com/120115840/233418234-8d70d002-01b7-4bb2-85f1-c0798d99e5aa.png)

![Screenshot 2023-04-20 211242](https://user-images.githubusercontent.com/120115840/233418415-e8180125-a4b8-47c1-abbc-2d31d122e11d.png)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
