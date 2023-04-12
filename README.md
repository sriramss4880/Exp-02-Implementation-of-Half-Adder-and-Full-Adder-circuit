# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
```
Program:

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: S.S.SRIRAM
RegisterNumber:212222230150
# Half Adder
module halfadd(A,B,C,S);
input A,B;
output S,C;
xor(S,A,B);
and(C,A,B);
endmodule

# Full Adder
module fulladd(a,b,ci,s,co);
input a,b,ci;
output s,co;
wire d,e,f;
xor(d,a,b);
xor(s,d,ci);
and(e,ci,d);
and(f,a,b);
or(co,e,f);
endmodule

```
### Output:

# RTL realization

HALF ADDER

![2 1](https://user-images.githubusercontent.com/120554177/231432282-69728b37-1509-4232-bbbf-c207aec8fdaf.png)

FULL ADDER

![2 2](https://user-images.githubusercontent.com/120554177/231432364-9ea08e35-df99-4abc-976e-335aafe215ea.png)

# TIMING DIAGRAM

HALF ADDER

![2 3](https://user-images.githubusercontent.com/120554177/231432558-ed4959e4-957e-43dd-b136-c1ab5cbc8f02.png)

FULL ADDER

![2 4](https://user-images.githubusercontent.com/120554177/231432987-540205f7-a862-4bdc-ae41-f096c9a27ea1.png)

# Logic symbol 

HALF ADDER

![2 5](https://user-images.githubusercontent.com/120554177/231433168-687569d9-202f-40f2-b753-5a6f19752274.png)

FULL ADDER

![2 6](https://user-images.githubusercontent.com/120554177/231433229-4101760f-0fa8-421e-954e-49f87e8a778c.png)

# TRUTH TABLE 

HALF ADDER

![2 7](https://user-images.githubusercontent.com/120554177/231433428-69270321-cf35-4bea-bd0c-61e48f6e0c9e.png)

FULL ADDER

![2 8](https://user-images.githubusercontent.com/120554177/231433707-d8a79493-899f-441b-9eb2-1a44b88c5720.png)



### Result:
Thus the half adder and full adder are studied and the truth table for different logic gates are verified.


