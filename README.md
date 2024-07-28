# asic-design activity 1

#GCC

Step1- Create new C program file

  ![1 1](https://github.com/user-attachments/assets/7ec05b8b-34fa-46c7-b890-dac290cd7dae)

Step 2 -  Write c code

  ![1 4](https://github.com/user-attachments/assets/e6b02d83-485e-414b-95f9-cf88dd4327c0)

Step 3 - compile

  ![1 5](https://github.com/user-attachments/assets/cfa23467-17c1-402e-a931-506464f9dfaa)



#RISC-V

Step-1
  1.1 Code
  
  ![1 4](https://github.com/user-attachments/assets/6c5df5b5-24b2-4dd9-9344-c5f04b935e6b)
    
  1.2  Compiling Code
  
   ![1 3](https://github.com/user-attachments/assets/95bee535-0fa2-4bad-bbfb-db1d41579e78)
    
  1.3 Output
  
   ![1 5](https://github.com/user-attachments/assets/87e46ee5-f90b-4de2-895a-5b9380fa14ea)
    
    
Step-2
  2.1 Run executable section
  
  ![2 1](https://github.com/user-attachments/assets/7a83d899-cd10-4dca-9812-c5be86fa5b6f)

  2.2 finding main  
  
   ![2 2](https://github.com/user-attachments/assets/6169b3fd-44b8-4463-9b02-e216d843412f)
    
  2.3 Finding value of main and adding 4 for each instruction
  
  ![2 3](https://github.com/user-attachments/assets/46d8bbcb-d963-491a-8e59-2bf31958612c)
    
  2.4 Finding next block address and subtracting, dividing by 4 to get no of instructions
  we get F which is unfortunately not in sc (3C/4=F(15))
  
  ![2 5](https://github.com/user-attachments/assets/d62c5c6e-ba1c-4c0e-9a44-414a59f50c2d)
    
Step-3 
3.1 Changing to ofast format

  ![2 6](https://github.com/user-attachments/assets/56b77bb6-2178-4ab4-942f-6e312f3b9a60)
    
3.2 Finding the value of main

   ![2 7](https://github.com/user-attachments/assets/b217261d-18ad-4d94-94f6-efad265b92be)
    
3.3 repeating the process to find the no of instructions (c=12)

  ![2 7](https://github.com/user-attachments/assets/3e17fa26-1ca3-4548-9a69-a0213f8e0d29)

  ![2 8](https://github.com/user-attachments/assets/ab22662a-e704-4f93-b8ee-7d3a96bf7961)


Conclusion -
  O1 is moderate in it's code optimization, Ofast is aggressive
  
  o1 has 15 while ofast has 12


  #ACTIVITY 2

  # asic-design activity 2
#spike debugger

STEP 1
  1.1 loading the file and initiating spike
  
  ![1 1](https://github.com/user-attachments/assets/cf532c70-b9fd-44b1-9d9d-5db14a0e3458)

  1.2 Inititing obj dump
  
  ![1 2_objdump](https://github.com/user-attachments/assets/e47a7bc6-a24c-4fe0-8625-0ce3a9c079f7)
  
  1.3 spike debug
  
  ![1 3](https://github.com/user-attachments/assets/a54f15b1-088d-4460-8615-7a6c40fa6089)

  1.4 initialising from 0 to 100b0
  
  ![1 5](https://github.com/user-attachments/assets/defbffca-b603-45c2-992b-7ec7ca7141c3)

  1.5 error - auic getting loaded insted of lui need help!
  
Conclusion-- encountering error





 To sort and organise a set of given instructions into their respective format type:

Assembly Instruction	Instruction format
ADD r5, r6, r7	R
SUB r7, r5, r6	R
AND r6, r5, r7	R
OR r8, r6, r5	R
XOR r8, r5, r4	R
SLT r10, r2, r4	R
ADDI r12, r3, 5	I
SW r3, r1, 4	S
SRL r16, r11, r2	R
BNE r0, r1, 20	B
BEQ r0, r0, 15	B
LW r13, r11, 2	I
SLL r15, r11, r2	R
The corresponding RISCV ISA fo the above instructions is shown in the table below:

Assembly Instruction	Hexadecimal Representation
ADD r5, r6, r7	0x00D302B3
SUB r7, r5, r6	0x40B383B3
AND r6, r5, r7	0x00F2B333
OR r8, r6, r5	0x00D322B3
XOR r8, r5, r4	0x00C292B3
SLT r10, r2, r4	0x004122B3
ADDI r12, r3, 5	0x00518293
SW r3, r1, 4	0x00312023
SRL r16, r11, r2	0x002585B3
BNE r0, r1, 20	0x00112163
BEQ r0, r0, 15	0x000003E3
LW r13, r11, 2	0x002585B3
SLL r15, r11, r2	0x002585B3 


    
   







  
