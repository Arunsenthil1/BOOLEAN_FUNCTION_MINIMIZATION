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
![truth table](https://github.com/user-attachments/assets/d75e959f-3611-4940-9a2a-170b1d19f401)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**



Developed by:ARUN.S RegisterNumber:24900177



 1  module exp_1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b&~d)|(~a&b&d)|(a&b&~c));
endmodule

2  module exp_2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y&z)|(w&y)|(x&y));
endmodule


**RTL realization**
1

![gates 2](https://github.com/user-attachments/assets/e63a4e0b-f04a-473c-8998-58653c6222a1)



2

![gates](https://github.com/user-attachments/assets/b6d18d16-3ff7-49e7-95bc-bb1e17ea96ac)




**Output:**

1   


![waveform 2](https://github.com/user-attachments/assets/ad9c8534-0a8e-4c72-872b-4a51233a52dd)

2


![waveform 1](https://github.com/user-attachments/assets/2ad3ddd7-b870-4a75-87e4-72df9ba02b8b)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

