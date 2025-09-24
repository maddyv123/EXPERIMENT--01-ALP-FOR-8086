# EXPERIMENT--01-ALP-FOR-8086
 # Name : MATHAVAN V
 
 # Roll no : 212223110026

 # Date of experiment : 18/09/2025





## Aim: To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 8086  emulator 
## Theory 
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.


 ## Running the Emulator :
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	  Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color 
 
 
3.		write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 

4.	 Compile the program and check for the errors 
5.	Run (once there is no syntax error) 

6.	Click OK to see/view the output of your program on the Emulator screen. 


7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,
8.	 


![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)











9.	Click on emulate to start emulation 








![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)








10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 






![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)







## Programs for arithmetic  operations

## Addition  of 8 bit ALP 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
ADD AX,BX
JNC Loop
INC CL
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT 
```

## Output  
<img width="2559" height="1599" alt="Screenshot 2025-08-22 154322" src="https://github.com/user-attachments/assets/2d96c465-dba0-4653-bb16-b21c19eac003" />

 
## Subtraction   of 8 bit numbers  ALP 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
SUB AX,BX
JNC Loop
INC CL  
NOT AX
INC AX
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT      
```
 
## Output  
<img width="2555" height="1599" alt="Screenshot 2025-08-22 160654" src="https://github.com/user-attachments/assets/8c722a0f-cfc1-4d6f-854a-5cc752fb5ac3" />

## Multiplication alp 
```
MOV AX,[3001H]
MOV BX,[3003H]
MUL BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```
 ## Output  
 <img width="2557" height="1599" alt="Screenshot 2025-08-22 162151" src="https://github.com/user-attachments/assets/6b522db9-1ba4-4fda-8937-91cb22063cc0" />



## Division alp 
```
MOV AX,[3001H]
MOV BX,[3003H]
DIV BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```

## Output  
<img width="2559" height="1599" alt="Screenshot 2025-08-22 162711" src="https://github.com/user-attachments/assets/6d053ed4-119c-4313-903f-ca2b878f682c" />

## LOGICAL OPERATIONS

## TRUTH TABLE FOR LOGICAL OPERATIONS

![symbols-truth-tables-of-common-logic-gates](https://github.com/user-attachments/assets/6caae067-aca0-4b9c-83e3-d22429c1b3ec)



## AND alp
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
MOV [3005H],AX
HLT
```
## Output
<img width="1280" height="800" alt="image" src="https://github.com/user-attachments/assets/3371ccf2-0033-44d1-ae75-560957ab94a9" />

## OR alp
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
MOV [3005H],AX
HLT
```
## Output
<img width="2559" height="1570" alt="Screenshot 2025-08-29 153205" src="https://github.com/user-attachments/assets/1526823a-4dba-4227-8654-ec380e02f7c2" />

## NAND alp
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## Output
<img width="2559" height="1599" alt="Screenshot 2025-08-29 153632" src="https://github.com/user-attachments/assets/171fb046-c087-4683-bce9-aa44f327b465" />

## NOR alp
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## Output


<img width="2559" height="1596" alt="Screenshot 2025-08-29 153459" src="https://github.com/user-attachments/assets/29236046-f49b-47e4-86c9-802a3f8527dc" />

## NOT alp
```
MOV AX,[3001H]
MOV BX,[3003H]
NOT AX
MOV [3005H],AX
HLT
```
## output

<img width="1272" height="800" alt="image" src="https://github.com/user-attachments/assets/aa99567b-1b52-4c7e-acfa-fcf10eddfa0b" />

## XOR alp
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
MOV [3005H],AX
HLT
```
## output

<img width="1280" height="800" alt="image" src="https://github.com/user-attachments/assets/8e4af9b7-9066-4feb-b789-9f525df8ce55" />

## XNOR alp
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## output

<img width="1280" height="800" alt="image" src="https://github.com/user-attachments/assets/da692c06-e64c-47dc-945d-32eda1feec98" />

## Result :
 
The Write and execute ALP on fundamental arithmetic and logical operations is executed successfully.
