## Experiment--02-Implementation-of-combinational-logic
## Implementation of combinational logic gates

## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming. F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D F2=xy’z+x’y’z+w’xy+wx’y+wxy

## Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
## Theory
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.

## Procedure
Step 1:

Create a project with required entities.

Step 2:

Create a module along with respective file name.

Step 3:

Run the respective programs for the given equations.

Step 4:

Run the module and get the respective RTL outputs.

Step 5:

Create university program(VWF) for getting timing diagram.

Step 6:

Give the respective inputs for timing diagram and obtain the results.

## Program:
F1:

module ff(a,b,c,d,f1);

input a,b,c,d;

output f1;

assign f1 = (~b&~d) | (~a&b&d) | (a&b&~c);

endmodule

F2:

module de (w,x,y,z,f2);

input w,x,y,z;

output f2;

assign f2 = (x&y)|(w&y)|(~y&z);

endmodule Developed by: A.DIVYA RegisterNumber: 212222230034 */

## RTL realization
F1
![243106713-029331d5-e82d-4b3e-9c0a-58de6af1fb76](https://github.com/sivabalan28/Experiment--02-Implementation-of-combinational-logic-/assets/113497347/05d84403-ac46-4219-ae8a-307694dfb201)

F2
![243106796-d618a026-b3bc-4445-ae04-9e1e55f13bbc](https://github.com/sivabalan28/Experiment--02-Implementation-of-combinational-logic-/assets/113497347/5121034a-cbed-4bff-a0ed-21494be2f788)


## Output:
## Timing Diagram
F1
![243106813-dfc3ae1f-ab5a-4dd5-a447-fa5fd1b2267e](https://github.com/sivabalan28/Experiment--02-Implementation-of-combinational-logic-/assets/113497347/22ee367e-f362-4f38-98ae-e4c4e539da44)



F2
![243106832-8938c25f-0a89-431d-9c47-ee1053e17ea1](https://github.com/sivabalan28/Experiment--02-Implementation-of-combinational-logic-/assets/113497347/0e1a1f89-2c15-4918-b776-0afea1252053)


## Truth Table
![241525320-2992336b-e9b1-4be4-b11c-2fe9db388021](https://github.com/sivabalan28/Experiment--02-Implementation-of-combinational-logic-/assets/113497347/631c5ced-0e17-47da-94cc-ca8cee81d64c)


## Result:
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
