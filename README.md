# Experiment--03-Half-Subtractor-and-Full-subtractor
## Implementation-of-Half-subtractor-and-Full-subtractor-circuit
## AIM:
To design a half subtractor and full subtractor circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime
## Theory
Subtractor circuits take two binary numbers as input and subtract one binary number input from the other binary number input. Similar to adders, it gives out two outputs, difference and borrow (carry-in the case of Adder). There are two types of subtractors.

## Half Subtractor Full Subtractor
## Half Subtractor
The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed.
![half-subtractor9](https://user-images.githubusercontent.com/36288975/166112538-58c3bc7c-ee5d-4e6a-ac8d-8e8328efe27a.png)


Sum = X'Y+XY' = X ⊕ Y
Carry=X'Y

## Full Subtractor
A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow. 
![full-subtractor6](https://user-images.githubusercontent.com/36288975/166112541-24c68359-3de8-4674-ae22-8272ffc385ed.png)


Diff = A ⊕ B ⊕ Bin B = A'Bin + A'B + BBin

## Procedure:
1.Create a New Project:Open Quartus and create a new project by selecting "File">"New Project Wizard".Follow the wizard's instructions to set up your project,including specifying the project name,location,andtarget device(FPGA).
2.Create a New Design File:Once the project is created,right-click on the project name in the Project Navigator and select "Add New File".-Choose "Verilog HDL File" or "VHDL File",depending on your choden hardware description language.
3.Write the Combinational Logic Code:Open the newly created Verilog or VHDL file and write the code for your combinational logic.
4.Complete the Project:To compile the project,click on"processing">"Start Complication" in the menu.Quartus will analyze your code,synthesize it into a netlist,and perform optimization based on your target FPGA device.
5.Analyze and Fix Errors:If there are any erreors or warnings during the complication process,Quartus will display them in the message window.Review and fix any issues in your code if necessary.View the RTL diagram.
6.Verification:Click on "File">"New">"Verification/debugging Files">"University Program VWF".Once waveform is created Right Click on the input/output Panel>"Insert Node or Bus">Click on Node Finder>Click on "List">Select All.Give the Input Combinations according to the Truth Table and the simulate the Output Waveform.
## Program:
```
/*
Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
Developed by: Farhana H
RegisterNumber:23012987  
*/
```
## Code:
## Half Subtractor
![image](https://github.com/syedfayaz3105/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/147144126/5ddf5a96-95f4-49a2-874a-c1863155cfe4)
## Full Subtractor
![image](https://github.com/syedfayaz3105/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/147144126/d02a823c-d98f-4ed2-8419-02d9dcbe3472)
## Truthtable
## Half Subtractor
![image](https://github.com/syedfayaz3105/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/147144126/797acd71-fe4a-4acd-87f6-d6d8ad500d2c)
## Full Subtractor
![image](https://github.com/syedfayaz3105/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/147144126/48f12993-fee8-4731-a2d4-99839372919d)
## Output RLT Realization:
## Half Subtractor
![image](https://github.com/syedfayaz3105/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/147144126/cd0904e6-ea9e-43ff-b644-6438081951f3)
## Full Subtractor
![image](https://github.com/syedfayaz3105/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/147144126/e9090972-23ed-4a5d-a927-0a05bf68b995)
## Output:
## Half Subtractor
![image](https://github.com/syedfayaz3105/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/147144126/3c6b9eb4-0156-444b-a03d-434bead6370a)
## Full Subtractor
![image](https://github.com/syedfayaz3105/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/147144126/5a2ebaab-9702-4dca-adbc-7ae918892866)
## Result:
Thus the half subtractor and full subtractor circuits are designed and the truth tables is verified using quartus software.
