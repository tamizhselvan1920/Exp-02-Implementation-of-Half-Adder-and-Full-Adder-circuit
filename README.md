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
Program:
```

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: tamizh selvan.R
RegisterNumber: 212222230158
HALF ADDER  

module HalfAdder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b);
endmodule  

FULL ADDER  

module FullAdder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = ((a^b)^c);
assign carry = ((a&b)|(b&c)|(c&a));
endmodule 


```
## LOGIC SYMBOL:


[211144326-1577e59c-846f-4c49-8ca5-c8ef6e6fe8e6](https://user-images.githubusercontent.com/121148386/230773304-098aa7ad-5040-41fb-8144-7c7caabb252a.png)



### Output:

## HALFADDER


![228281863-61e4a539-83c7-4533-9147-27cc0907d9ce](https://user-images.githubusercontent.com/121148386/230775270-c0bd7e8e-519d-4a97-b1c1-2efb3886ba17.png)


## FULLADDER


![228282005-5af5d457-ef17-4ca3-b6e2-927e3b425e23](https://user-images.githubusercontent.com/121148386/230775280-ce3d0408-ed14-43db-ad57-8ab18a622634.png)

### RTL
### TIMING DIAGRAM

## HALFADDER

![228282470-c9baee44-896e-4d8c-ae4a-f56bcd56836a](https://user-images.githubusercontent.com/121148386/230775308-5fd63b02-a1f5-4d33-b8e6-065f2cd373f5.png)

## FULLADDER






### TRUTH TABLE 

## HALFADDER

![228282753-06896acf-5fbb-4022-801c-e1a6bc0474a3](https://user-images.githubusercontent.com/121148386/230775367-d3f21c35-19ef-4d1a-a01e-e495cd1b07e6.png)

## FULLADDER


![228282840-fb15b2fa-f483-49b7-be53-d4a148fab6f2](https://user-images.githubusercontent.com/121148386/230775415-21425694-4748-4f1b-94a2-641935f423fd.png)


### Result:

Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
