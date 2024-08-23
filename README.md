# EXPERIMENT--01-ALP-FOR-8086
Name :
Roll no 
Date of experiment :





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
org 100h
MOV al,11h;
MOV bl,20h;
ADD al,bl;
MOV [6379h],al;
ret
```


## Output  
![image](https://github.com/user-attachments/assets/e6cfac51-6b3b-4eee-ba92-1c89d51c1f4e)

 
## Subtraction   of 8 bit numbers  ALP 
```
org 100h
MOV al,20h;
MOV bl,[8778h];
SUB bl,al;
MOV [8798h],bl;
ret
```
 
## Output  
![image](https://github.com/user-attachments/assets/b31809ac-1e18-4d2b-882f-488f8540c084)

## Multiplication alp 
```
org 100h
 MOV al,13h;
 MOV bl,2h;
 MUL bl;
 MOV [6063h],bl;
 ret
```
 ## Output  
![image](https://github.com/user-attachments/assets/954e49b5-78e6-434b-b975-9deb362e28ef)


## Division alp 
```
org 100h
mov ax,08h;
mov bx,02h;
div bx;
mov [5000h],ax;
ret
```

## Output  
![Screenshot 2024-08-19 084951](https://github.com/user-attachments/assets/4d772a1f-5242-4257-9cd2-6d2baf096c82)

## Programs For Logical Operators:
## AND
```
org 100h
mov bx,1000h;
and bx,1111h;
mov [0040h+02],bx;
ret
```
## Output
![image](https://github.com/user-attachments/assets/5bf37ef6-cc17-427d-b37a-88c06eeab2e9)

## OR
```
MOV SI,0532H;
MOV AX,0A32H;
MOV BX,0B13H;
OR AX,BX;
```
## Output
![image](https://github.com/user-attachments/assets/a11b2ca4-9860-4468-b047-ff1a1722425b)

## NOT
```
org 100h
mov bx,0040h;
mov ax,[bx]; 
not al;
mov [0040h+04],ax;
ret
```
## Output
![image](https://github.com/user-attachments/assets/f1c82272-f20f-45de-92b3-18c104f42426)
## XOR
```
MOV [SI+2],AX;
MOV AX,0A32H;
MOV BX,0B13H;
XOR AX,BX;
```
## Output
![image](https://github.com/user-attachments/assets/045bbc94-8a2f-44c4-aeb4-0606eaa5abc9)

## Result :
Thus, to write and execute ALP on fundamental arithmetic operations and Logical operations is successful.
 








