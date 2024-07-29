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
| Instruction      | Format | Operation              |
|------------------|--------|------------------------|
| ADD r11, r12, r13| R      | Add                    |
| SUB r13, r11, r12| R      | Subtract               |
|AND r12, r11, r13 | R      | Logical AND            |
| OR r8, r12, r5   | R      | Logical OR             |
| XOR r8, r11, r4  | R      | Logical XOR            |
| SLT r30, r20, r4 | R      | Set on Less Than       |
| ADDI r31, r21, 5 | I      | Add Immediate          |
| SW r21, r19, 4   | S      | Store Word             |
| SRL r26, r21, r20| R      | Shift Right Logical    |
| BNE r0, r19, 20  | B      | Branch if Not Equal    |
| BEQ r0, r0, 15   | B      | Branch if Equal        |
| LW r23, r21, 2   | I      | Load Word              |
| SLL r25, r21, r20| R      | Shift Left Logical     |


 
Upload the 32-bit pattern on Github"
The corresponding RISCV hexa decimal ISA for the above instructions is shown in the table below:

Assembly Instruction	Hexadecimal Representation
| Instruction      | Format | Operation              | RISC-V ISA    |
|------------------|--------|------------------------|---------------|
| ADD r11, r12, r13   | R      | Add                    | 0x00d60b33   |
| SUB r13, r11, r12   | R      | Subtract               | 0x40b60d33    |
| AND r12, r11, r13   | R      | Logical AND            | 0x00d6b733    |
|OR r8, r12, r5     | R      | Logical OR             | 0x00560b33    |
| XOR r8, r11, r4   | R      | Logical XOR            | 0x0045b333   |
| SLT r30, r20, r4  | R      | Set on Less Than       | 0x004aa733    |
|  ADDI r31, r21, 5   | I      | Add Immediate          | 0x005af093    |
| SW r21, r19, 4   | S      | Store Word             | 0x004a9b23    |
| SRL r26, r21, r20 | R      | Shift Right Logical    | 0x014ad333    |
| BNE r0, r19, 20  | B      | Branch if Not Equal    |0x014a1a63    |
| BEQ r0, r0, 15   | B      | Branch if Equal        | 0x00f0063    |
| LW r23, r21, 2  | I      | Load Word              | 0x002ad113    |
| SLL r25, r21, r20 | R      | Shift Left Logical     | 0x014a9323    |


Task 2 To execute in instructed assembly instructions using a given verilog code for a riscV processor.


Here's the table formatted for GitHub with the provided data:
Standard ISA vs Hardcoded ISA

| Operation         |   Standard RISCV ISA| Hardcoded ISA  |
|-------------------|---------------------|----------------|
| ADD r11, r12, r13    | 32'h00d6b33       | 32'h00d6b300   |
| SUB r13, r11, r12   | 32'h40b6d33        | 32'h40b6d380   |
| AND r12, r11, r13    | 32'h00d6f33        | 32'h00d6f400  |
| OR r8, r12, r5    | 32'h0056c33        | 32'h0056c400  |
|XOR r8, r11, r4    | 32'h0046c33        | 32'h0046c500   |
| SLT r30, r20, r4    | 32'h004a0f33        |32'h004a0f00   |
|  ADDI r31, r21, 5  | 32'h005af93        | 32'h005af200   |
| SW r21, r19, 4      | 32'h004bb3        | 32'h0040b300   |
| SRL r26, r21, r20   | 32'h014b6d33        | 32'h014b6d00   |
| BNE r0, r19, 20    | 32'h014be63        | 32'h014be200   |
| BEQ r0, r0, 15    | 32'h00fbe63        | 32'h00fbe000   |
| LW r23, r21, 2    | 32'h002b8513        | 32'h002b8100   |
|SLL r25, r21, r20  |32'h014b6933        | 32'h014b6900   |

EDITING THE VERILOG CODE TO ASSIGNED INSTRUCTIONS

![code](https://github.com/user-attachments/assets/7e69f984-1fe7-4a6c-ae9f-808f1f26cf6b)

RUNNING GTKWAVE

![code](https://github.com/user-attachments/assets/6486e0d5-160f-4e96-9445-9aac9220a6e4)

OUTPUT WAVEFROMS


 ADD r11, r12, r13
 


![and](https://github.com/user-attachments/assets/3d2ff4af-e50c-4a69-81ad-838ac76529f5)



SUB r13, r11, r12



![sub](https://github.com/user-attachments/assets/ae17da79-9fb8-4f4e-9f66-ff14305706fd)



AND r12, r11, r13

    
   
![and](https://github.com/user-attachments/assets/75d946b6-b965-4405-bf55-7e19301a7f1f)


OR r8, r12, r5



![or](https://github.com/user-attachments/assets/dda958c4-d648-4f43-83f1-84b00e4597ed)

XOR r8, r11, r4


![xor](https://github.com/user-attachments/assets/e79aa888-d2bc-4603-9133-0197fa08b4b2)


SLT r30, r20, r4

  ![slt](https://github.com/user-attachments/assets/178cdced-9c18-48fe-b723-b323f437d41e)

ADDI r31, r21, 5

![addi](https://github.com/user-attachments/assets/c4a1f6b4-adeb-457a-8a4f-c372b8b09b2e)

LW r23, r21, 2

![lw](https://github.com/user-attachments/assets/ecca3310-9c75-404c-9f35-fa2505a4ecee)




BEQ r0, r0, 15

![beq](https://github.com/user-attachments/assets/735caa9b-9f9b-42e4-8a31-34fac29b96ac)


SLL r25, r21, r20

![sll](https://github.com/user-attachments/assets/53c4fcdf-3757-4c8f-8be2-014aca679426)

SW r21, r19, 4 

![sw](https://github.com/user-attachments/assets/1dde50bb-59ea-4a33-b30b-7f1bad9ff7b0)

SRL r26, r21, r

![srl](https://github.com/user-attachments/assets/f0d1d4f8-113f-48aa-8d56-a21c2e345a3c)


 BNE r0, r19, 20 
 
![bne](https://github.com/user-attachments/assets/cdac749b-6d74-44e3-a63f-b759363aedab)


CONCLUSION-
GTK waveforms of riscv ISA codes have been generated according to required instructions and posted

 

