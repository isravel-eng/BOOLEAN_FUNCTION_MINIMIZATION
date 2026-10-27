# BOOLEAN_FUNCTION_MINIMIZATION

### Name: Isravel Y
### Registered number: 212225240054

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
```verilog
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: Isravel y
RegisterNumber: 212225240054*/

 module ex2 (a,b,c,d,w,x,y,z,f1,f2);
 input a,b,c,d,w,x,y,z; output f1,f2;
 assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
 assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
 endmodule
```
 
**RTL realization**

<img width="741" height="665" alt="image" src="https://github.com/user-attachments/assets/92366261-f5b7-4c5f-8ef5-b76adc2176ce" />


**Output:**
**RTL**
**Timing Diagram**
<img width="1321" height="337" alt="image" src="https://github.com/user-attachments/assets/23030c17-ff03-4583-b2cb-18c1334e973d" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

