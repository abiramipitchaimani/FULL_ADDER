# FULL_ADDER

## AIM:
To simulate and synthesis Half adder using Xilinx ISE.
## APPARATUS REQUIRED: 
Xilinx 14.7 Spartan6 FPGA
## PROCEDURE: 
### STEP:1 
Start the Xilinx navigator, Select and Name the New project.
### STEP:2 
Select the device family, device, package and speed. 
### STEP:3 
Select new source in the New Project and select Verilog Module as the Source type.
### STEP:4 
Type the File Name and Click Next and then finish button. Type the code and save it. 
### STEP:5 
Select the Behavioral Simulation in the Source Window and click the check syntax. 
### STEP:6 
Click the simulation to simulate the program and give the inputs and verify the outputs as per the truth table.
### STEP:7 
Select the Implementation in the Sources Window and select the required file in the Processes Window.
### STEP:8 
Select Check Syntax from the Synthesize XST Process. Double Click in the Floorplan Area/IO/Logic-Post Synthesis process in the User Constraints process group. UCF(User constraint File) is obtained.
### STEP:9 
In the Design Object List Window, enter the pin location for each pin in the Loc column Select save from the File menu.
### STEP:10 
Double click on the Implement Design and double click on the Generate Programming File to create a bitstream of the design.(.v) file is converted into .bit file here.
### STEP:11 
Load the Bit file into the SPARTAN 6 FPGA
### STEP:12 
On the board, by giving required input, the LEDs starts to glow light, indicating the output.
# Truth Table
![image](https://github.com/RESMIRNAIR/FULL_ADDER/assets/154305926/02ead8f5-d958-4c89-ac51-368ca086cf41)
# Circuit Diagram
![image](https://github.com/RESMIRNAIR/FULL_ADDER/assets/154305926/418e00aa-ed19-4ab3-a413-bae9575bff0e)
![image](https://github.com/RESMIRNAIR/FULL_ADDER/assets/154305926/0c26fe47-d78c-43dd-ac0d-804e427a3bbc)
# PROGRAM:
```
SUBMITTED BY
P.ABIRAMI
212222060006
```
```
 module fulladder(a,b,cin,sum,carry);
       input a,b,cin;
       output sum,carry;
       wire w1,w2,w3;
       xor g1(w1,a,b);
       xor g2(sum,w1,cin);
       and g3(w2,w1,cin);
       and  g4(w3,a,b);
       or g5(carry,w2,w3);
  endmodule
```
# OUTPUT:
![Screenshot 2024-03-17 203854](https://github.com/abiramipitchaimani/FULL_ADDER/assets/163704307/adc605ef-887c-4383-a998-4a22efef9c69)
# RESULT:
Hence, the stimulation and synthesis of a half adder was run successfully by using Xilinx ISE.


