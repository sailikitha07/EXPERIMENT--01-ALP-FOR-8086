# EXPERIMENT--01-ALP-FOR-8086
Name : Cholimgapuram Sai Likitha
Roll no : 212224230046
Date of experiment : 18.02.2026





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


## Output  :
## Arithematic operations:
### add
```
ORG 100H
MOV AX,[1001H]
MOV BX,[1003H]
ADD AX,BX
MOV [1200h],AX
MOV [1202h],DX
HLT
```
<img width="1919" height="1021" alt="Screenshot 2026-02-02 211355" src="https://github.com/user-attachments/assets/ba7875f7-ad03-49b9-a16f-d468f9c997df" />

### sub
```
ORG 100H
MOV AX,[1001H]
MOV BX,[1003H]
SUB AX,BX
MOV [1200h],AX
MOV [1202h],DX
HLT
```
<img width="1919" height="1117" alt="Screenshot 2026-02-02 211831" src="https://github.com/user-attachments/assets/d2a8fcd8-e5b3-4344-8783-bb1b013b97fe" />


### mul
```
ORG 100H
MOV AX,[1001H]
MOV BX,[1003H]
MUL BX
MOV [1200h],AX
MOV [1202h],DX
HLT
```
<img width="1919" height="1111" alt="Screenshot 2026-02-02 212349" src="https://github.com/user-attachments/assets/e0d261ea-456d-4c49-9c04-1611bf112a4d" />


### div
```
ORG 100H
MOV AX,[1001H]
MOV BX,[1003H]
DIV BX
MOV [1200h],AX
MOV [1202h],DX
HLT
```

<img width="1919" height="1119" alt="Screenshot 2026-02-02 212700" src="https://github.com/user-attachments/assets/547bed58-afef-4cb8-b6ea-04e7d9c826e4" />

## Logical operations:
### and
```
ORG 100H
MOV AX,[1001H]
MOV BX,[1003H]
AND AX,BX
RET
```
<img width="1919" height="1076" alt="Screenshot 2026-02-02 214432" src="https://github.com/user-attachments/assets/faa6b322-1ac5-4bf9-813b-ae52d6e03e3e" />

### or
```
ORG 100H
MOV AX,[1001H]
MOV BX,[1003H]
OR AX,BX
RET
```
<img width="1919" height="1083" alt="Screenshot 2026-02-02 215626" src="https://github.com/user-attachments/assets/ab62ca60-6dca-4313-b11b-81914564726c" />

### nand
```
ORG 100H
MOV AX,[1001H]
MOV BX,[1003H]
AND AX,BX 
NOT AX
RET
```
<img width="1919" height="1088" alt="Screenshot 2026-02-02 220314" src="https://github.com/user-attachments/assets/3c1e9552-17cf-41d3-960d-a104a7f99d72" />

### nor
```
ORG 100H
MOV AX,[1001H]
MOV BX,[1003H]
OR AX,BX
NOT AX
RET
```
<img width="1919" height="1039" alt="Screenshot 2026-02-02 220634" src="https://github.com/user-attachments/assets/dcfa6c8b-f9e9-4da8-a8bc-3f8c146d8911" />

### xor
```
ORG 100H
MOV AX,[1001H]
MOV BX,[1003H]
XOR AX,BX 
RET
```
<img width="1919" height="1005" alt="Screenshot 2026-02-02 220822" src="https://github.com/user-attachments/assets/19d93600-dab5-4858-b58f-a15778767ca3" />

### xnor
```
ORG 100H
MOV AX,[1001H]
MOV BX,[1003H]
XOR AX,BX
NOT AX 
RET
```
<img width="1919" height="1076" alt="Screenshot 2026-02-02 221026" src="https://github.com/user-attachments/assets/c0de4b95-1052-40ec-a03f-3e31a8d08a14" />

### not
```
ORG 100H
MOV AX,[1001H]
NOT AX 
RET
```
<img width="1919" height="1026" alt="Screenshot 2026-02-02 221516" src="https://github.com/user-attachments/assets/9148d28b-3a45-485b-b85d-1fd6dbe5a6a4" />

## Result :
Thus execution of ALP on fundamental arithmetic and logical operations is sucessfully verified









