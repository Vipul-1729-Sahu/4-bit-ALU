# 4-bit-ALU

---

## IMPORTANT POINTS TO NOTE
1) OUTPUTS ARE DISPLAYED IN "HEXADECIMAL" NOT BINARY.  
2) IN CASE OF SUBTRACTION ONLY MAGNITUDE IS CONSIDERED NOT SIGN.

---

## INSTRUCTIONS TO SIMULATE THE CIRCUIT

1) FOR SUBTRACTION:  
C3 = 0  
C2 = 0  

2) FOR ADDITION:  
C3 = 0  
C2 = 1  

3) FOR LOGICAL AND:  
C3 = 1  
C2 = 0  

4) FOR LOGICAL OR:  
C3 = 1  
C2 = 1  

---

## This is 4 bit ALU circuit which can perform the following functions:
1) Binary Addition  
2) Binary Subtraction  
3) AND operation  
4) OR operation  

---

## ➤ FOR BINARY ADDITION
- Here 4 bit binary ripple carry adder is used.  
- For addition C2 = 0  

---

## ➤ FOR BINARY SUBTRACTION
- CONTROL INPUT (C2) is used along with the XOR gates to reverse the input B.  
- For subtraction C2 = 1  

- In case of subtraction if carry out comes to be 0 then, the output would come in 2's complement form.

To convert it to binary back:
- One more 4 bit adder is used.  
- Values given by first adder will be reversed when C2 = 0 & Cout = 0.  
- Hence we will get the 1's complement.  
- In order to get it into binary we have added 1 as carry in.

Cin = 1 only when C2 = 0 & Cout = 0  
Else Cin will remain 0 and the value given by the 1st adder will pass as it is.

---

## ➤ ROLE OF IC 74153N (CONTAINS TWO 4:1 MUX)
- Used to choose which operation to be done.  
- We have used 3 such IC (or five 4:1 mux) to make a 4 bit 4:1 mux.

---

## ➤ DISPLAY
- Two hex displays have been used to convert 5 bit binary into hexadecimal.
