# Experiment--04-Implementation-of-combinational-logic-using-universal-gates-
 ## Implementation-of-Half-subtractor-and-Full-subtractor-circuit
## AIM:
To implement the given logic function using NAND and NOR gates and to verify its operation in Quartus using Verilog programming.
F=((C'.B.A)'(D'.C.A)'(C.B'.A)')' using NAND gate
F=(((C.B'.A)+(D.C'.A)+(C.B'.A))')' using NOR gate


## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime
## Theory
 
 
 
 


## Procedure



Write the detailed procedure here 


## Program:
/*
Program to design a Implementation of combinational logic using universal gates-  and verify its truth table in quartus using Verilog programming.
Developed by: RAKSHITHA DEVI.J
RegisterNumber: 212221230082 
*/
```
module combinationallogic(a,b,c,d,p,q,r,s);
input a,b,c,d;
output p,q,r,s;
assign p=(c & ~b & ~a);
assign q=(d & ~c & ~a);
assign r=(~c & b & ~a);
assign s=(~p & ~q & ~r);
endmodule
```
```
module combo(A,B,C,D,F);
input A,B,C,D;
output F;
wire P,Q,R,S;
assign P=(C&~B&A);
assign Q=(D&~C&A);
assign R=(C&~B&A);
assign S=~(P|Q|R);
not(F,S);
endmodule
```

## Output:
```
F=((C'.B.A)'(D'.C.A)'(C.B'.A)')' using NAND gate
```

## Truthtable:



##  RTL realization:


## Timing diagram :

```
F=(((C.B'.A)+(D.C'.A)+(C.B'.A))')' using NOR gate
```

## Truthtable:

##  RTL realization:

## Timing diagram :


## Result:
Thus implementation of logic functions using NAND and NOR gates is done and its operation is verified in Quartus using Verilog programming.
 
