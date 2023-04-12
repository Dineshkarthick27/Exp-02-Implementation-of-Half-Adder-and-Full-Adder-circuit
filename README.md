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
/*Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by:D.Dhanumalya 
RegisterNumber:212222230030

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

Logic symbol & Truthtable
RTL realization

### Output:
# Half Adder:

![image](https://user-images.githubusercontent.com/120552008/231431134-70039bc2-ab55-418c-b06b-efbde1b23950.png)

# Full Adder:

![image](https://user-images.githubusercontent.com/120552008/231431251-6f6f15b2-c0f4-4c99-98b0-0e651652f1dc.png)

### RTL
### TIMING DIAGRAM
# Half Adder:

![image](https://user-images.githubusercontent.com/120552008/231431668-da507147-b971-49a8-b562-4e76675eabf4.png)

# Full Adder:

![image](https://user-images.githubusercontent.com/120552008/231431766-37086750-a05b-4aad-a4d2-26aafa7d88d3.png)
### LOGIC SYMBOL

# Half Adder

![image](https://user-images.githubusercontent.com/120552008/231432486-1bd1b48c-6214-49b0-a438-f6e480b368ac.png)

# Full Adder

![image](https://user-images.githubusercontent.com/120552008/231432519-b7c31dd2-fcc6-4f61-a6a0-bb3a6ca78b02.png)

### TRUTH TABLE 
# Half Adder:
![image](https://user-images.githubusercontent.com/120552008/231432170-a5452a50-16be-419e-8d34-b3f9eed3e9b3.png)

# Full Adder:
![image](https://user-images.githubusercontent.com/120552008/231432410-b318f2c3-ee7d-4df8-b0e6-a68a150b9af9.png)


### Result:
Thus the half adder and full adder are studied and the truth table for different logic gates are verified.


