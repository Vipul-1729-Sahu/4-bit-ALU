# 4-bit-ALU


**IMPORTANT POINTS TO NOTE**
1) OUTPUTS ARE DISPLAYED IN "HEXADECIMAL" NOT BINARY.
2) IN CASE OF SUBTRACTION ONLY MAGNITUDE IS CONSIDERED NOT SIGN.


**INSTRUCTIONS TO SIMULATE THE CIRCUIT**
1) FOR SUBTRACTION:     C3=0       C2=0
2) FOR ADDITION:        C3=0       C2=1
3) FOR LOGICAL AND:     C3=1       C2=0
4) FOR LOGICAL OR:      C3=1       C2=1


This is 4 bit ALU circuit . which can perform the following functions :
1) binary addition 
2) binary subtraction 
3) AND , OR operation

-> FOR BINARY ADDITION : 
# Here 4 bit binary ripple carry adder is used.
# for addition C2 = 0

-> FOR BINARY SUBTRACTION :
# CONTROL INPUT (C2) is used along with the xor gates to reverse the input B .
# for subtraction C2 = 1
# in case of subtraction if carry out comes to be 0 then, the ouput would come in 2's complement form
to convert it to binary back , we have used one more 4 bit adder is used , where values given by first
adder will be reversed when C2 = 0 & Cout = 0 , hence we will get the 1's complement and , in order to get 
it into binary we have added 1 as carry in (Cin = 1 only when C2=0 & Cout=0  else , Cin will remian 0 and the 
value given by the 1st adder will be pass as it is.) 
         
ROLE OF IC 74153N (CONTAINS TWO 4:1 MUX) :
-> used to choose which operation to be done. 
-> we have used 3 such IC (or five 4:1 mux) to make an 4 bit 4:1 mux.

DISPLAY :
-> Two hex displays has been used to convert 5 bit binary into hexadecimal.
