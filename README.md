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



 # asic-design activity 3
 

TASK 1- 

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

![running](https://github.com/user-attachments/assets/1dd3b5dd-3d17-4218-9873-4390f189eb51)


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


 # asic-design activity 4
 
TASK- To write an Application in C, compile it with gcc and Risc-v gcc

APPLICATION- To find prime numbers till the given digit

STEP-1 The code to perform the given application

![image](https://github.com/user-attachments/assets/4a44541c-b335-454d-aaa5-e3ad2f5dfd6b)



STEP-2 Compiled using GCC

![image](https://github.com/user-attachments/assets/c67b5cb7-cb3f-409f-af13-b9ddee8cacae)



STEP-3 Compiled using RISC-V GCC and showing spike

![image](https://github.com/user-attachments/assets/d96c2a5e-f75d-4899-8040-88e709b9e455)



CONCLUSION- GCC and RISC-V GCC is compared for a simple program
 
 # asic-design activity 5
 
**Digital Logic with TL Verilog and Makerchip**
TL-Verilog is an advanced hardware description language created to streamline and expedite digital design by minimizing the complexity and verbosity found in traditional languages such as Verilog and VHDL. TL-Verilog offers a fresh perspective on design, prioritizing transactional-level modeling to simplify the management of intricate pipelined systems. With TL-Verilog, designers can concentrate on hardware behavior rather than detailed implementation specifics, benefiting from automatic pipeline management, a clean and succinct syntax, and robust abstraction features.


In TL-Verilog, combinational circuits are designed to model logic where the output depends only on the current inputs, with no dependence on previous states or clock signals. TL-Verilog’s high-level abstractions and syntax simplify the description of these circuits compared to traditional hardware description languages.

![image](https://github.com/user-attachments/assets/3ee5c984-c126-4ed5-a7aa-e9c99d6c72a8)

**inverter**
![Screenshot (2)](https://github.com/user-attachments/assets/09d96996-83a0-413d-beac-00dc2f4708e9)

**2 input AND gate**
![Screenshot (4)](https://github.com/user-attachments/assets/ea682154-7fc1-4ec0-9342-f56bd4fad663)

**2 input OR gate**
![Screenshot (4)](https://github.com/user-attachments/assets/c31ac25b-aa8f-4a2f-b65a-b16a31314722)


**2:1 MUX**

![Screenshot (6)](https://github.com/user-attachments/assets/33aac333-4280-4357-8f33-0879e11d57c7)

**2:1 MUX using Vectors**
![Screenshot (7)](https://github.com/user-attachments/assets/aae0cb7f-cca7-4f7a-bf96-e996bc70aa5a)


## **Sequential Circuits in TL-Verilog**
**Sequential Calculator**
![Screenshot (8)](https://github.com/user-attachments/assets/25d7e0ff-ee02-43ef-b488-4baf45812824)

**Pipelined Logic**
![Screenshot (10)](https://github.com/user-attachments/assets/f77b03fb-e3f4-415a-a627-bc0aa7558e30)


**Cycle Calculator**
![Screenshot (11)](https://github.com/user-attachments/assets/50731452-56bc-40fc-9cfa-ed80eae87da7)

## **Validity**
![Screenshot (12)](https://github.com/user-attachments/assets/04b7386c-b500-4d46-98b4-2831fdfb6448)

**validity in cycle calc**
![Screenshot (14)](https://github.com/user-attachments/assets/70bd5b20-4d7c-47b1-8dd3-9545ca59b276)

## **Day 4 Basic RISC V architecture**
**Program Counter**
The program counter is designed to increment by 4 to retrieve the subsequent instruction from memory, as illustrated in the image below. If a reset occurs, the program counter will be set to zero, preparing it to fetch the next instruction.

![Screenshot (19)](https://github.com/user-attachments/assets/5991d013-d018-4ede-bdb6-092a67743fb2)

**Fetch**
![Screenshot (22)](https://github.com/user-attachments/assets/74971975-bd6c-42c6-9e6a-4e0c11108ac3)
![Screenshot (23)](https://github.com/user-attachments/assets/1a76a468-4d6f-4798-8c46-731c21e6f94b)


### **Decode**
For decoding a particular instruction, it is necessary that the isntruction type and format is known to the processor. The decoding is a crucial part and has to be done properly according to the given format to avoid error. There are 6 instructions type in RISC-V :

1)Register (R) type
2)Immediate (I) type
3)Store (S) type
4)Branch (B) type
5)Upper immediate (U) type
6)Jump (J) type

#### **Instruction Type Decode**

![Screenshot (24)](https://github.com/user-attachments/assets/a5f7e2a1-2286-4d95-b24e-6cdce62e0735)

#### **INSTRUCTION IMMEDIATE DECODE**
![Screenshot (26)](https://github.com/user-attachments/assets/7d4f9901-ef19-499a-af0a-ffa84a79c27d)

#### **INSTRUCTION DECODE**
![Screenshot (28)](https://github.com/user-attachments/assets/98adaad6-e9ec-4ca0-9eba-44a2e84e59dc)
![Screenshot (29)](https://github.com/user-attachments/assets/e4f45ac3-3200-4990-a945-5eabd1496f0c)

#### **Decode Instruction Field Based**
![Screenshot (30)](https://github.com/user-attachments/assets/f58133d7-382d-4fe0-b38a-800140c50370)

#### **Individual Instruction Decode**
![Screenshot (31)](https://github.com/user-attachments/assets/270cff4a-de57-4319-8369-bc708cf95536)


### **Execute and Register file read/write**
![image](https://github.com/user-attachments/assets/5ab858a6-ab5c-4ac5-ada2-64dca10656aa)

![image](https://github.com/user-attachments/assets/b4321d89-83c6-4079-b838-72547c60f7f5)

### **Lab On ALU**
![image](https://github.com/user-attachments/assets/e6bbafbf-351d-46de-8496-1ab4a27b3a54)

![image](https://github.com/user-attachments/assets/0922abca-ee8b-4f98-a05f-02aafd67bf52)

### **Register File Write**
![image](https://github.com/user-attachments/assets/8ffc5c26-20d6-435d-a26d-4eab55a28ee8)

### **ARRAYS**
#### **Implementing Branch Instructions**
![image](https://github.com/user-attachments/assets/4f680717-2041-4ff0-8893-6f912ec13356)

#### **Complementing Branch Instructions**
![image](https://github.com/user-attachments/assets/f0ab1c45-82a8-4a8f-9724-4881a2709b4a)

### Testbench
![image](https://github.com/user-attachments/assets/5757c12c-4c06-4348-be89-4277a6ab13f9)

## DAY-5 Complete Pipelined RiscV CPU Micro-architecture
### **3 cycle valid signal**
![Screenshot (34)](https://github.com/user-attachments/assets/6c9ec6e5-a216-477f-8c0a-97c91c1512e3)
![Screenshot (35)](https://github.com/user-attachments/assets/164163e8-9129-4d3f-96d9-184146bad631)
![Screenshot (36)](https://github.com/user-attachments/assets/8fe0858a-f608-4704-a394-c41348a741c3)
### **generating valid signals for each instruction**
![Screenshot (38)](https://github.com/user-attachments/assets/62a3dad8-f325-48b7-b7cc-fcbecc76a447)
**For Register File Bypass To Address Rd-After-Wr Hazard**
![Screenshot (40)](https://github.com/user-attachments/assets/cadac882-7aca-494d-b27d-3d098e6ca05d)
**including load/store instructions:**
![Screenshot (41)](https://github.com/user-attachments/assets/5f6c3f23-a56a-429c-85d8-5693f84c13b2)
![Screenshot (42)](https://github.com/user-attachments/assets/91084491-21b1-4c99-84fa-e542becbd722)
![Screenshot (43)](https://github.com/user-attachments/assets/d35e8d8c-086e-4521-a596-7daa4c26e7e4)



### **Completing the RISC-V CPU**

![Screenshot (41)](https://github.com/user-attachments/assets/df105006-50cf-4765-ae95-799fb3ba9ad8)

![Screenshot (42)](https://github.com/user-attachments/assets/c9fd46d6-da9c-4324-be10-577f8b00f75d)




