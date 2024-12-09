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

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:yashwanth.asv RegisterNumber:*/24900018



 i)function 1
 
 
 
 
    module funct1(a,b,c,d,f1);
    input a,b,c,d;
    output f1;
    assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
    endmodule
 
 
 
 ii) function 2
 
 
 
 
    module funct2(w,x,y,z,f2);
    input w,x,y,z;
    output f2;
    assign f2=((~y & z)|( w & y )|(x & y));
    endmodule

**Truthtable**

![Screenshot 2024-12-09 131350](https://github.com/user-attachments/assets/47b5738d-ca98-4f2a-841c-3179d492c337)


![Screenshot 2024-12-09 131423](https://github.com/user-attachments/assets/d635f219-ebba-496d-a54d-b6b707309115)

**RTL**

![Screenshot 2024-12-09 131534](https://github.com/user-attachments/assets/bc2615cf-97a3-4b04-abce-544afd08ef8d)


![Screenshot 2024-12-09 131611](https://github.com/user-attachments/assets/ffa37ea7-2128-4025-918b-33b5b052487f)




**Output:**

![Screenshot 2024-12-09 131643](https://github.com/user-attachments/assets/2d4562b2-f88c-4a0a-8d95-9577aab2f3e7)



**Timing Diagram**

![Screenshot 2024-12-09 131813](https://github.com/user-attachments/assets/60fe6bfb-8722-4ff0-a8ff-d383910a7e8a)

**kMAP**



![Screenshot 2024-12-09 131909](https://github.com/user-attachments/assets/aa0154b5-7af8-4dac-8791-1ef4bbe5f536)

![Screenshot 2024-12-09 132011](https://github.com/user-attachments/assets/e202eb16-764c-46c5-93f1-581156eed80a)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

