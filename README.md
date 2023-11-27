# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
 

## Logic Diagram
## Procedure
## Program:
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: LOKESHVARN S
RegisterNumber:  23012889
*/
## Program:
   module exp1(a,b,c,d,f);
   input a,b,c,d;
   output f;
   wire p,q,r;
   assign p=(~c & b & a);
   assign q=(~d & c & ~a);
   assign r=(c & ~b & a);
   assign f=(~(~p & ~q & ~r));
   endmodule
   ## Using NOR gate:
      module exp2(a,b,c,d,f);
   input a,b,c,d;
   output f;
   wire p,q,r;
   assign p=( c & ~b & a);
   assign q=( d & ~c & a);
   assign r=( c & ~b & a);
   assign f=(~(~( p | q | r)));
   endmodule
   ## Output:
   ![image](https://github.com/Lokeshvaran9600/Experiment--02-Implementation-of-combinational-logic-/assets/145972263/f80134f8-d5e3-47bb-863e-ba9735dc0cd0)
## Timing Diagram:
![image](https://github.com/Lokeshvaran9600/Experiment--02-Implementation-of-combinational-logic-/assets/145972263/9685d73f-a1b3-4fe4-8124-32b38af8a342)
## Trutn table:
![image](https://github.com/Lokeshvaran9600/Experiment--02-Implementation-of-combinational-logic-/assets/145972263/b2def3d7-9fed-4c02-b9e9-b10d0d95c368)
## Using NOR gate:
![image](https://github.com/Lokeshvaran9600/Experiment--02-Implementation-of-combinational-logic-/assets/145972263/126feca0-eff2-4601-82a9-308f318b0caa)
## Timing diagram:
![image](https://github.com/Lokeshvaran9600/Experiment--02-Implementation-of-combinational-logic-/assets/145972263/21180e1f-1abd-4456-9e4e-d00762e70d48)
## Truth table:
![image](https://github.com/Lokeshvaran9600/Experiment--02-Implementation-of-combinational-logic-/assets/145972263/e6e4e9af-b279-4efe-bc89-f0479da8d59c)
## Result:
Thus the given logic functions are implemented using NAND and NOR gates and their operations are verified using Verilog programming.
