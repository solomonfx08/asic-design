![WhatsApp Image 2024-11-26 at 6 11 15 AM](https://github.com/user-attachments/assets/0806f2f3-8e7a-4630-a107-43003214527d)![WhatsApp Image 2024-11-26 at 1 12 08 AM](https://github.com/user-attachments/assets/0201af9e-a1ca-48c5-b886-d0484080e869)![image](https://github.com/user-attachments/assets/3b3693e9-f6b1-42f5-a55c-82fec63ca12f)# asic-design activity 1

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
  
  ![dsad](https://github.com/user-attachments/assets/13767734-47ef-4910-af39-73706b0ed6ec)

  1.2 Inititing obj dump
  
  ![2dsad](https://github.com/user-attachments/assets/39cee9eb-71d9-4ed6-ab6c-2d3bb003decd)

1.3: Read the initial contents of the register a0 and then press enter to run the instruction.
1.4: Verify that the instruction is executed properly.
1.5: Now read the initial contents of sp register & run the next instruction.
  
 ![3dsad](https://github.com/user-attachments/assets/37d062fe-6fb8-4956-99ea-8d1009440e1f)


  1.6: Using calculator ensure that the difference between initial and final contents of the sp register should be as per the intruction set.
  
![4dsad](https://github.com/user-attachments/assets/b0bd5e79-2556-46ab-927d-8d2dbab8e903)


  



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
![image](https://github.com/user-attachments/assets/2ca1e972-a6e8-406f-bdc5-48fd6e455355)

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
S
The next task is to 'read from' and 'write into' the registers. In this operation, 2 read and write operation can be carried out simulatenously. The two src1_value/src2_value takes input from the two read register rf_read_data1/ rf_read_data2 and pass it on to the ALU unit. At present, ADDI and ADD is execute whose result is obtained in register rf_write_data. The figure below shows the input and output registers.
![image](https://github.com/user-attachments/assets/d444be03-77d3-427f-b8b5-efd109dc4cb8)

![image](https://github.com/user-attachments/assets/5ab858a6-ab5c-4ac5-ada2-64dca10656aa)

![image](https://github.com/user-attachments/assets/b4321d89-83c6-4079-b838-72547c60f7f5)

### **Lab On ALU**
![image](https://github.com/user-attachments/assets/daa77e3b-8b41-46d2-83cf-a9b7901c031b)

![image](https://github.com/user-attachments/assets/e6bbafbf-351d-46de-8496-1ab4a27b3a54)

![image](https://github.com/user-attachments/assets/0922abca-ee8b-4f98-a05f-02aafd67bf52)

### **Register File Write**
![image](https://github.com/user-attachments/assets/8ffc5c26-20d6-435d-a26d-4eab55a28ee8)

### **ARRAYS**
Typically, registers and memory are used in conjunction to implement arrays in RISC-V. Memory can be used to store arrays, where each element is kept at a distinct memory location. To access these components, the processor can employ load and store instructions. For instance, you could load a component into a register from a memory array, process it, and then put the outcome back into memory.

Registers are another option for partially storing arrays. The elements of an array can be put into registers for quicker processing if the array is small enough to fit into the available registers. Since register access is typically faster than memory access, this strategy can enhance speed for specific processes.








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


# asic-design assignment activity 6
Conversion from TLV into Verilog using Sandpiper-SaaS compiler, compile using Iverilog and plot the waveforms using GTKwave:
## Step-1 
Cloning

![WhatsApp Image 2024-08-26 at 11 54 08 PM (1)](https://github.com/user-attachments/assets/81a2e0b2-2b42-4e39-9a7f-6c560e7053b7)

## Step-2
The command used to convert the code is given below:
![WhatsApp Image 2024-08-26 at 11 54 08 PM](https://github.com/user-attachments/assets/eda4b1a7-1ee9-4155-9289-5b6a18f434de)
## Step-3
The command to compile the verilog code and project in gtkwave is as shown below:
![WhatsApp Image 2024-08-26 at 11 54 08 PM (2)](https://github.com/user-attachments/assets/86f3487d-bcd1-421e-8fde-1bea3bac7a93)
## Output

![WhatsApp Image 2024-08-26 at 11 53 40 PM](https://github.com/user-attachments/assets/fab7536c-4152-47e6-8d9a-1dad139c4e7b)
## Output in maker chip IDE
![image](https://github.com/user-attachments/assets/16ea2bd4-084d-4ed3-8716-5e665ec0be1e)




![image](https://github.com/user-attachments/assets/f2bfb0e2-c1d2-4da7-801c-e5cb941b65e0)


# asic-design assignment activity 7
generate waveform for DAC and PLL peripheral for Risc-V processor.
Risc-V core inside the VSDbabySoc and observe the ports of peripherals: 
![Screenshot from 2024-09-02 21-57-12](https://github.com/user-attachments/assets/5cc02e1b-608b-4fb5-9141-185622017478)

Below is the output for the waveforms:
![Screenshot from 2024-09-02 21-58-36](https://github.com/user-attachments/assets/2cc352e2-02f9-42f8-914b-1a8506e878bf)


# asic-design assignment activity 8
## RTL design using Verilog with SKY130 Technology
### DAY 1
#### Introduction to iverilog and GTKWave
-terminal
![Screenshot from 2024-10-21 19-54-07](https://github.com/user-attachments/assets/5ca719ac-c40b-475a-b282-1af06756a19d)
-gtkwave
![Screenshot from 2024-10-22 04-16-52](https://github.com/user-attachments/assets/9c401f8f-6eac-45a0-b9ee-ebd3cdc00347)
-code
//design
module good_mux (input i0, input i1, input sel, output reg y);
    always@(*)
    begin
    	if(sel)
  		y<=i1;
  	else
  		y<=i0;
    end
endmodule

//testbench
module tb_good_mux;
  reg i0,i1,sel;
  wire y;

   	good_mux uut(.sel(sel),.i0(i0),.i1(i1),.y(y));

  initial begin
  	$dumpfile("tb_good_mux.vcd");
  	$dumpvars(0,tb_good_mux);
  	sel=0;
  	i0=0;
  	i1=0;
  	#300 $finish;
  end
  always #75 sel = ~sel;
  always #10 i0 = ~i0;
  always #55 i1 = ~i1;
endmodule

#### introduction to yosys
-Installation and running good MUX
![Screenshot from 2024-10-21 20-07-19](https://github.com/user-attachments/assets/840ee17a-9757-444b-99c1-951082810caa)
![Screenshot from 2024-10-21 20-08-38](https://github.com/user-attachments/assets/68eb5cbc-6d8a-4346-8c0e-24f8fa585410)

![Screenshot from 2024-10-21 20-08-38](https://github.com/user-attachments/assets/8e00df2e-d6d2-4b60-97ef-350c9cc87e41)

-code
//Generated Netlist
module good_mux(i0, il, sel, y);
	wire _0_;
	wire _1_;
	wire _2_;
	wire_3_;
	input i0; wire i0;
	input il; wire il;
	input sel; wire sel;
	output y; wire y;
	
	sky130_fd_sc_hd__mux2_1 _4_ (.AO(_0_),.A1(_1_),.S(_2_),.X(_3_));
	
	assign_0_ = 10;
	assign 1 = il;
	assign 2 = sel;
	assign y = _3_;
endmodule

-DOT viewer
![Screenshot from 2024-10-21 20-10-17](https://github.com/user-attachments/assets/039c4f28-201a-46f0-ae5b-8a7714c40251)
### DAY 2
#### Yosys Synthesis for Multiple Modules
-Terminal
![Screenshot from 2024-10-21 21-01-26](https://github.com/user-attachments/assets/50628f7c-75b2-4ac1-9eb2-886dfda9c681)
![Screenshot from 2024-10-21 21-02-22](https://github.com/user-attachments/assets/11e38bfa-cb06-4a34-887c-7d4201993f41)
-DOT Viewer
![Screenshot from 2024-10-21 21-02-44](https://github.com/user-attachments/assets/95b0d7d4-ff18-4c4d-84ea-317ceb91fc67)

-code
//Generated Netlist
module multiple_modules (a, b, c, y);
	input a; wire a;
	input b; wire b;
	input c; wire c;
	wire net1;
	output y; wire y;

	sub_modulel ul (.a(a),.b(b),.y(net1));
	sub_module2 u2 (.a(net1),.b(c),.y (y));
endmodule

module sub_modulel (a, b, y);
	wire _0_;
	wire _1_;
	wire _2_;
	input a; wire a;
	input b; wire b;
	output y; wire y;
	
	sky130_fd_sc_hd_and2_0_3_(.A(_1_),.B(_0_),.X(_2_));
	
	assign _1_ = b;
	assign _0_ = a;
	assign y = _2_;
endmodule

module sub_module2 (a, b, y);
	wire _0_;
	wire _1_;
	wire _2_;
	input a; wire a;
	input b; wire b;
	output y;wire y;

	sky130_fd_sc_hd_or2_0_3_ (A(_1_), .B( 0 ), .X( 2 ));
	assign _1_ = b;
	assign _0_ = a;
	assign y = _2_;
endmodule
#### Use of Module Level Synthesis


![image](https://github.com/user-attachments/assets/43aeb567-b283-4399-84ec-367b38fabf68)

#### Use of Flattening
-terminal

![image](https://github.com/user-attachments/assets/3f942c19-9dae-4204-baa3-90bb03e3b2d6)
-dot viewer

![image](https://github.com/user-attachments/assets/75574633-1d66-4a90-b0a6-74d4e4b8423a)

-code
generated netlist
//Generated Netlist
module multiple_modules (a, b, c, y);
	wire _0_; wire _1_;
	wire _2_; wire _3_;
	wire _4_; wire _5_;
	input a; wire a;
	input b; wire b;
	input c; wire c;
	wire net1;
	wire \ul.a;
	wire \ul.b;
	wire \ul.y;
	wire \u2.a;
	wire \u2.b;
	wire \u2.y;
	output y; wire y;
	
	sky130_fd_sc_hd_and2_0 _6_ (.A(1),.B(0),.X(_2_));
	sky130_fd_sc_hd_or2_0 _7_(.A(4),.B(_3_),.X(5));

	assign 4 = \u2.b ;
	assign 3 = \u2.a ;
	assign \u2.y = _5_;
	assign \u2.a = net1;
	assign \u2.b = c;
	assign y = \u2.y;
	assign 1 = \u1.b;
	assign 0 = \ul.a ;
	assign \ul.y = _2_;
	assign \ul.a = a;
	assign \u1.b = b;
	assign net1 = \u1.y;
endmodule

#### Simulation of D-Flipflop using Iverilog and GTKWave

##### Async reset
-terminal

![Screenshot from 2024-10-21 21-20-34](https://github.com/user-attachments/assets/65b8082c-4063-4ea5-88be-cb7f317e2df5)

-GTKwave

![Screenshot from 2024-10-21 21-21-22](https://github.com/user-attachments/assets/342b0379-719f-496b-b12b-8587f10fb1bd)

-code
//Design
module dff_asyncres(input clk, input async_reset, input d, output reg q);
	always@(posedge clk, posedge async_reset)
	begin
		if(async_reset)
			q <= 1'b0;
		else
			q <= d;
	end
endmodule
//Testbench
module tb_dff_asyncres; 
	reg clk, async_reset, d;
	wire q;
	dff_asyncres uut (.clk(clk),.async_reset (async_reset),.d(d),.q(q));

	initial begin
		$dumpfile("tb_dff_asyncres.vcd");
		$dumpvars(0,tb_dff_asyncres);
		// Initialize Inputs
		clk = 0;
		async_reset = 1;
		d = 0;
		#3000 $finish;
	end
		
	always #10 clk = ~clk;
	always #23 d = ~d;
	always #547 async_reset=~async_reset; 
endmodule
##### Async set
-terminal
![image](https://github.com/user-attachments/assets/8fdf202d-bc1c-43ef-8e25-9c456286fd96)

-gtkwave

![image](https://github.com/user-attachments/assets/de3cba09-caf0-4c1b-9a9a-6779b521deaf)

-code
//Design
module dff_async_set(input clk, input async_set, input d, output reg q);
	always@(posedge clk, posedge async_set)
	begin
		if(async_set)
			q <= 1'b1;
		else
			q <= d;
	end
endmodule
//Testbench
module tb_dff_async_set; 
	reg clk, async_set, d;
	wire q;
	dff_async_set uut (.clk(clk),.async_set (async_set),.d(d),.q(q));

	initial begin
		$dumpfile("tb_dff_async_set.vcd");
		$dumpvars(0,tb_dff_async_set);
		// Initialize Inputs
		clk = 0;
		async_set = 1;
		d = 0;
		#3000 $finish;
	end
		
	always #10 clk = ~clk;
	always #23 d = ~d;
	always #547 async_set=~async_set; 
endmodule

##### Synchronous Reset
- terminal

  ![image](https://github.com/user-attachments/assets/cb75ccda-955b-40b0-8012-0a40ff16dfb9)

-GTKWAVE

![image](https://github.com/user-attachments/assets/96d438c5-50bb-4fbb-8439-e6a1c5ea3285)

-code
//Design
module dff_syncres(input clk, input sync_reset, input d, output reg q);
	always@(posedge clk)
	begin
		if(sync_reset)
			q <= 1'b0;
		else
			q <= d;
	end
endmodule
//Testbench
module tb_dff_syncres; 
	reg clk, syncres, d;
	wire q;
	dff_asyncres uut (.clk(clk),.sync_reset (sync_reset),.d(d),.q(q));

	initial begin
		$dumpfile("tb_dff_syncres.vcd");
		$dumpvars(0,tb_dff_syncres);
		// Initialize Inputs
		clk = 0;
		sync_reset = 1;
		d = 0;
		#3000 $finish;
	end
		
	always #10 clk = ~clk;
	always #23 d = ~d;
	always #547 sync_reset=~async_reset; 
endmodule

#### Synthesis of D-Flipflop using Yosys
##### Asynchronous Reset

- Terminal

  ![Screenshot from 2024-10-21 21-27-11](https://github.com/user-attachments/assets/9505954d-b8f7-4608-96c1-7f6afba95187)

![Screenshot from 2024-10-21 21-28-05](https://github.com/user-attachments/assets/1e05c733-eb0e-454c-900a-56ce232af470)

- Dot Viewer
![Screenshot from 2024-10-21 21-48-17](https://github.com/user-attachments/assets/95c70f60-e009-4e19-8d7c-521eb48163dc)

-netlist

![Screenshot from 2024-10-21 21-28-21](https://github.com/user-attachments/assets/0b66e71a-e2a0-4a1e-8801-4381956e257d)
##### Async Set
-terminal

![Screenshot from 2024-10-21 21-54-12](https://github.com/user-attachments/assets/ed3cb2f0-0974-431e-b43a-6de79f01f946)

-dot viewer

![Screenshot from 2024-10-21 21-53-37](https://github.com/user-attachments/assets/d16f88df-07fb-4c7c-ba3a-b664cead61d8)

-netlist

![Screenshot from 2024-10-21 21-54-23](https://github.com/user-attachments/assets/9b99b3aa-5f3b-45d1-8489-e3589c31c40b)

##### Sync reset
-terminal

![Screenshot from 2024-10-21 21-56-00](https://github.com/user-attachments/assets/eccece47-5ae8-4cd9-b548-111a7c723b95)

-dotviewer

![Screenshot from 2024-10-21 21-55-34](https://github.com/user-attachments/assets/2a0ec5b4-da86-4b04-acac-c0afcbb1072d)

-netlist

![Screenshot from 2024-10-21 21-56-11](https://github.com/user-attachments/assets/ac58e3a2-6fcf-4b66-8d61-94a64cc4f331)

##### Multiplication by 2

-terminal
yosys
read_liberty -lib ../lib/sky130_fd_sc_hd__tt_025C_1v80.lib
read_verilog mult_2.v
synth -top mul2
abc -liberty ../lib/sky130_fd_sc_hd__tt_025C_1v80.lib
show
write_verilog -noattr mul2_net.v
gvim mul2_net.v
-netlist

![Screenshot from 2024-10-21 21-58-51](https://github.com/user-attachments/assets/b51b6550-aa74-4806-a025-151dfa76c016)

-dot viewer

![Screenshot from 2024-10-21 22-26-00](https://github.com/user-attachments/assets/c128be51-1fa4-4d56-bfb3-56ffb9ed0047)

##### Multiplication by 9

-terminal 

yosys
read_liberty -lib ../lib/sky130_fd_sc_hd__tt_025C_1v80.lib
read_verilog mult_9.v
synth -top mult9
abc -liberty ../lib/sky130_fd_sc_hd__tt_025C_1v80.lib
show
write_verilog -noattr mul9_net.v
gvim mul9_net.v

-netlist
module mul9(a,y);
	input [2:0]a; wire [2:0]a;
	output [5:0]y; wire [5:0]y;

	assign y = {a,a};
endmodule

-dot viewer

![image](https://github.com/user-attachments/assets/dc59aba0-c443-4fce-8244-03a54b3f72cc)

### DAY 3
Optimization of Various Designs
#### 2 input AND Gate:
![image](https://github.com/user-attachments/assets/07620f9d-472b-4379-b7dd-12f794cca4f7)
![image](https://github.com/user-attachments/assets/95172258-43ae-4849-a11d-913d181bfdc6)

-code
//Design
module opt_check(input a, input b, output y);
	assign y = a?b:0;
endmodule

-dot viewer
![Screenshot from 2024-10-22 01-18-58](https://github.com/user-attachments/assets/592ba251-c575-4331-85e3-5b8800fce842)

#### 2 input OR Gate
-terminal
![image](https://github.com/user-attachments/assets/c0cd9e9f-7214-4002-aa74-da1b51bf3b40)
![image](https://github.com/user-attachments/assets/8f2123cb-2f75-4d24-a5bf-5e85a696122c)

-code
//Design
module opt_check2(input a, input b, output y);
	assign y = a?1:b;
endmodule

-dot viewer
![Screenshot from 2024-10-22 01-20-18](https://github.com/user-attachments/assets/2a4b630b-2cbe-4fbc-9c41-85707adac7c8)

#### 3 input AND Gate:
-terminal
![Screenshot from 2024-10-22 01-23-40](https://github.com/user-attachments/assets/081297e2-c887-4c0f-80c6-9a616034253a)

![Screenshot from 2024-10-22 01-23-58](https://github.com/user-attachments/assets/b4e5b929-a176-4d7b-b81f-f8f79d92ac52)

![Screenshot from 2024-10-22 01-26-30](https://github.com/user-attachments/assets/a57ebf34-e4a1-41c2-8637-b97531d70e4b)


-code
//Design
module opt_check2(input a, input b, input c, output y);
	assign y = a?(b?c:0):0;
endmodule

-dot viewer
![image](https://github.com/user-attachments/assets/2569c469-334a-4791-85b1-16450bbfdafe)

#### 2 input XNOR Gate (3 input Boolean Logic)

-terminal
![image](https://github.com/user-attachments/assets/55225978-f90d-46c4-8bd1-3c23cb79349c)
![image](https://github.com/user-attachments/assets/c04984a9-b110-417e-a5e6-9713824d87ed)

-code
//Design
module opt_check2(input a, input b, input c, output y);
	assign y = a ? (b ? ~c : c) : ~c;
endmodule

-dot viewer
![Screenshot from 2024-10-22 01-26-44](https://github.com/user-attachments/assets/f536e682-917a-45d6-9175-f15063be6409)
#### Multiple Module Optimization-1
-terminal
![Screenshot from 2024-10-22 01-33-55](https://github.com/user-attachments/assets/3fc5516f-5901-4e7a-a857-fee01d59cebc)

![Screenshot from 2024-10-22 01-33-35](https://github.com/user-attachments/assets/da705198-b9c8-4cf8-88e3-a08d4394ff41)
![Screenshot from 2024-10-22 01-33-19](https://github.com/user-attachments/assets/791b6a64-0ed3-4e5e-8733-37eefcf30c65)

-dot viewer
![Screenshot from 2024-10-22 01-34-13](https://github.com/user-attachments/assets/e599aba1-412a-47f6-a9f6-8333d92383d8)
-code
//Design

module sub_module1(input a, input b, output y);
	assign y = a & b;
endmodule

module sub_module2 (input a, input b output y);
	assign y = a^b;
endmodule

module multiple_module_opt(input a, input b input c, input d output y);
	wire n1,n2, n3;

	sub_module1 U1 (.a(a), .b(1'b1), .y(n1));
	sub_module2 U2 (.a(n1), .b(1'b0), .y(n));
	sub_module2 U3 (.a(b), .b(d), .y(n3));

	assign y = c | (b & n1);
endmodule

#### Multiple Module Optimization-2
-terminal
![Screenshot from 2024-10-22 01-38-31](https://github.com/user-attachments/assets/eb8ea8e7-eae0-409b-8dcc-dc885fcb0242)
![Screenshot from 2024-10-22 01-38-11](https://github.com/user-attachments/assets/19a12728-a978-4cfb-b963-b45722f2866a)

-code
//Design
module sub_module(input a input b output y);
	assign y = a & b;
endmodule

module multiple_module_opt2(input a, input b input c, input d, output y);
	wire n1,n2, n3;

	sub_module U1 (.a(a), .b(1'b0), y(n));
	sub_module U2 (.a(b), .b(c), .y(n2));
	sub_module U3 (.a(n2), .b(d), .y(n));
	sub_module U4 (.a(n3), .b(n1), .y(y));
endmodule

#### D-Flipflop Constant 1 with Asynchronous Reset (active low) 
-terminal
![Screenshot from 2024-10-22 01-53-08](https://github.com/user-attachments/assets/4b33b9d8-a90d-4a8a-a1bc-18ac19b1c9e1)

-gtkwave
![Screenshot from 2024-10-22 01-53-45](https://github.com/user-attachments/assets/bcbdfc24-b267-4c27-b267-66e165c140bb)

YOSYS Synthesis
-terminal
![Screenshot from 2024-10-22 01-55-13](https://github.com/user-attachments/assets/0f3e3516-4216-40e4-8fce-2d3677446992)

-dotviewer
![Screenshot from 2024-10-22 01-55-41](https://github.com/user-attachments/assets/a92ab1a5-5a4b-4cdf-b700-f05cc80356a4)

#### D-Flipflop Constant 2 with Asynchronous Reset (active high)
-terminal
![Screenshot from 2024-10-22 02-00-02](https://github.com/user-attachments/assets/a9aaa822-b488-4255-97eb-4cf2581f9e77)
![Screenshot from 2024-10-22 02-00-14](https://github.com/user-attachments/assets/650ab797-bff5-4a05-987f-0a18082c0ef2)
![Screenshot from 2024-10-22 01-59-41](https://github.com/user-attachments/assets/c2b8389f-35c5-42b7-a683-f10005054693)

-dot viewer
![image](https://github.com/user-attachments/assets/2599098b-6f3c-4f35-ad50-273ca53351d4)

-code
//Design
module dff_const2(input clk, input reset, output reg q); 
always @(posedge clk, posedge reset)
begin
	if(reset)
		q <= 1'b1;
	else
		q <= 1'b1;
end
endmodule
//Testbench
module tb_dff_const2; 
	reg clk, reset;
	wire q;

	dff_const2 uut (.clk(clk),.reset(reset),.q(q));

	initial begin
		$dumpfile("tb_dff_const1.vcd");
		$dumpvars(0,tb_dff_const1);
		// Initialize Inputs
clk = 0;
		reset = 1;
		#3000 $finish;
	end

	always #10 clk = ~clk;
	always #1547 reset=~reset;
endmodule

#### D-Flipflop Constant 3 with Asynchronous Reset (active low)
-terminal
![Screenshot from 2024-10-22 02-02-30](https://github.com/user-attachments/assets/6bde7399-fdd6-4972-a50f-8d7e3845bddd)
![Screenshot from 2024-10-22 02-02-44](https://github.com/user-attachments/assets/7b09a4d5-3998-4984-a7a6-f64aa7c8ac42)
-code
//Design
module dff_const3(input clk, input reset, output reg q); 
	reg q1;

	always @(posedge clk, posedge reset)
	begin
		if(reset)
		begin
			q <= 1'b1;
			q1 <= 1'b0;
		end
		else
		begin	
			q1 <= 1'b1;
			q <= q1;
		end
	end
endmodule

-dot viewer
![Screenshot from 2024-10-22 02-02-56](https://github.com/user-attachments/assets/8a4d7c25-9451-4c67-aaf2-9fddb69d27ec)

#### D-Flipflop Constant 4 with Asynchronous Reset (active high)
-terminal
![Screenshot from 2024-10-22 02-05-49](https://github.com/user-attachments/assets/4a07fbc0-95bd-4003-8e23-4ae265fb87ba)
![Screenshot from 2024-10-22 02-06-04](https://github.com/user-attachments/assets/ed49bc1d-49a2-4258-9a4e-c4ec265a1154)

-dot viewer
![Screenshot from 2024-10-22 02-06-19](https://github.com/user-attachments/assets/0d2a50fd-ea89-48dd-b8cf-a5fb799ba50f)

-code
//Design
module dff_const4(input clk, input reset, output reg q); 
	reg q1;

	always @(posedge clk, posedge reset)
	begin
		if(reset)
		begin
			q <= 1'b1;
			q1 <= 1'b1;
		end
		else
		begin	
			q1 <= 1'b1;
			q <= q1;
		end
	end
endmodule

#### D-Flipflop Constant 5 with Asynchronous Reset
- terminal
  ![Screenshot from 2024-10-22 02-07-43](https://github.com/user-attachments/assets/3a399010-2380-4ca4-864d-e250ebdcb997)
![Screenshot from 2024-10-22 02-08-47](https://github.com/user-attachments/assets/881c8f1f-a106-4ba5-8190-3d2567d12229)

-dot viewer
![image](https://github.com/user-attachments/assets/615b8c3d-02eb-4dc8-9d68-0e2568530c5a)

-code
//Design
module dff_const5(input clk, input reset, output reg q); 
	reg q1;

	always @(posedge clk, posedge reset)
	begin
		if(reset)
		begin
			q <= 1'b0;
			q1 <= 1'b0;
		end
		else
		begin	
			q1 <= 1'b1;
			q <= q1;
		end
	end
endmodule

#### Counter opt 1
-terminal
![Screenshot from 2024-10-22 02-09-22](https://github.com/user-attachments/assets/6744a7c7-de88-48c3-8758-350d5744fad8)
![Screenshot from 2024-10-22 02-08-59](https://github.com/user-attachments/assets/65c4dd67-d88c-4d53-b0af-e8ae77fd8f0b)
![Screenshot from 2024-10-22 02-08-47](https://github.com/user-attachments/assets/c31ae341-b76d-4caf-a228-8e9951484b34)

-code
//Design	
module counter_opt (input clk, input reset, output q);
	reg [2:0] count;
	assign q = count[0];
	
	always @(posedge clk,posedge reset)
	begin
		if(reset)
			count <= 3'b000;
		else
			count <= count + 1;
	end
endmodule

-dot viewer
![Screenshot from 2024-10-22 02-09-36](https://github.com/user-attachments/assets/a4688606-c532-4aab-9bc9-91e9895b658e)


#### Counter Optimization 2: 
-terminal
![Screenshot from 2024-10-22 02-11-40](https://github.com/user-attachments/assets/aa2e2693-04f5-4b7d-b24e-bba881d903c5)
![Screenshot from 2024-10-22 02-11-30](https://github.com/user-attachments/assets/8f265ed2-eef8-48bb-9d86-c4359be87f05)

-dot viewer
![Screenshot from 2024-10-22 02-11-51](https://github.com/user-attachments/assets/5bef7dee-9a90-4e9e-8dee-ae9a56a6e55d)

-code
//Design	
module counter_opt2 (input clk, input reset, output q);
	reg [2:0] count;
	assign q = (count[2:0] == 3'b100);
	
	always @(posedge clk,posedge reset)
	begin
		if(reset)
			count <= 3'b000;
		else
			count <= count + 1;
	end
endmodule

### DAY 4
#### Design of 2x1 MUX using Ternary Operator:
-Terminal
![Screenshot from 2024-10-22 02-15-36](https://github.com/user-attachments/assets/5eff0632-8396-425d-a935-f0212646b51a)

-![Screenshot from 2024-10-22 02-15-57](https://github.com/user-attachments/assets/487185e4-20ef-4a4c-a007-9a57efc28592)


-code
//Generated Netlist
module ternary_operator_mux(i0, il, sel, y);
	wire _0_;
	wire _1_;
	wire _2_;
	wire _3_;
	input i0; wire i0;
	input il; wire il;
	input sel; wire sel;

 SYNTHESIS

 -terminal
 ![Screenshot from 2024-10-22 02-18-37](https://github.com/user-attachments/assets/e7653208-7d73-4d90-adcd-5dad3bfbc29a)

 ![Screenshot from 2024-10-22 02-18-47](https://github.com/user-attachments/assets/30f6bd5e-bfaf-4fde-8bdc-2c2d3b63c2a0)

	-netlist
 ![Screenshot from 2024-10-22 02-18-58](https://github.com/user-attachments/assets/5a47d6b1-8353-473f-9357-cf47d46e5c5c)

- dot viewer
  ![Screenshot from 2024-10-22 02-19-11](https://github.com/user-attachments/assets/d1e9dcc5-9463-462b-833e-7ab7996b9860)

#### Design of a Bad 2x1 MUX: 

-terminal
![Screenshot from 2024-10-22 02-24-18](https://github.com/user-attachments/assets/4a797dcd-842b-4284-9f7b-13c2e344f3bd)

- gtkwave
  ![Screenshot from 2024-10-22 02-24-38](https://github.com/user-attachments/assets/392ae613-88fa-4fb1-934d-e66a60c923b7)

-code
//Design
module bad_mux(input i0, input i1, input sel, output reg y);
	always@(sel)
	begin
		if(sel)
			y <= i1;
		else
			y <= i0;
	end
endmodule

YOSYS Synthesis

-terminal
![Screenshot from 2024-10-22 02-27-10](https://github.com/user-attachments/assets/8c75718e-9fd9-417e-9ddb-e6e11b748cc0)
![Screenshot from 2024-10-22 02-26-53](https://github.com/user-attachments/assets/e35a27e4-5374-474b-8aa1-dbbc7fecdbca)

-netlist
![Screenshot from 2024-10-22 02-27-19](https://github.com/user-attachments/assets/86df6359-4549-4d1a-9303-64b10b65a423)

-dot viewer
![Screenshot from 2024-10-22 02-27-45](https://github.com/user-attachments/assets/91d2bfef-1d6e-4e17-a55a-b6b0c1f776a9)

#### Blocking Caveat: 

-terminal
![image](https://github.com/user-attachments/assets/921ba33f-3448-4adc-a268-2444694ac3b5)

-gtkwave
![image](https://github.com/user-attachments/assets/b1109b6c-884a-492d-9c18-99e0cc7d6ad9)

YOSYS Synthesis
-terminal
![Screenshot from 2024-10-22 02-29-03](https://github.com/user-attachments/assets/f6c47243-538d-4a4e-8281-c2f5104857d8)
![Screenshot from 2024-10-22 02-28-47](https://github.com/user-attachments/assets/188a848e-fda0-434d-b9e0-052d03689ff1)

-netlist
//Generated Netlist
module blocking_caveat(a,b,c,d);
	wire _0_;
	wire _1_;
	wire _2_;
	wire _3_;
	wire _4_;
	input a; wire a;
	input b; wire b;
	input c; wire c;
	input d; wire d;
	output d; wire d;
	
	sky130_fd_sc_hd__o21a_1 _5_ (.A1(_2_),.A2(_1_),.B1(_3_),.X(_4_));

	assign _2_ = b;
	assign _1_ = a;
	assign _3_ = c;
	assign d = _4_;
endmodule

- DOT viewer
![Screenshot from 2024-10-22 02-29-31](https://github.com/user-attachments/assets/2278076b-dd60-4039-a73e-105f7849ff15)




 # asic-design activity 9
 Synthesize the RISC-V core and compare its output with functional simulations.

 Steps:
 1. Copy source files:
    First copy the src folder from VSDBabySoC directory to your VLSI folder. Then, move this folder into the sky130RTLDesignAndSynthesisWorkshop directory using the following commands:
sudo -i
cd /home/nikhil-bhusari/VLSI/
cp -r src sky130RTLDesignAndSynthesisWorkshop/
2. Navigate to the target directory:
   Move to the correct directory to begin the synthesis process:
3. Start YOSYS
4. Load the Verilog design files and start Synthesis
	   ![Screenshot from 2024-10-25 22-49-46](https://github.com/user-attachments/assets/d5a7466b-0edb-41c2-ba69-2e942c3e809f)
   ![Screenshot from 2024-10-25 22-49-52](https://github.com/user-attachments/assets/1482573c-1939-4c34-b179-7483d71cce41)

 GVIM file
 ![image](https://github.com/user-attachments/assets/47d09a77-ccc3-4a40-987c-287757e2e6b9)
 ![Screenshot from 2024-10-25 22-51-23](https://github.com/user-attachments/assets/e353f168-bc06-4fae-8c1e-de7ae3b6b211)

 The Heirarchy of the Net list is shown below :
 ![Screenshot from 2024-10-26 00-35-43](https://github.com/user-attachments/assets/2c028ca9-933c-48d0-aa7c-0824ad6b931d)

5.Use iverilog to simulate the synthesized RISC-V and generate the waveform:
![Screenshot from 2024-10-26 00-11-37](https://github.com/user-attachments/assets/dddad07c-69a8-4f44-a0e4-15fd332978b9)

"Functional Simulations (Previously done in LAB-7)":
Command Steps:
cd ~
cd VSDBabySoC
iverilog -o ./pre_synth_sim.out -DPRE_SYNTH_SIM src/module/testbench.v -I src/include -I src/module/
./pre_synth_sim.out
gtkwave pre_synth_sim.vcd




COMPARISON of Functionality vs Synthesized output waveform:

![dasdsad](https://github.com/user-attachments/assets/56b7086f-6318-478b-8807-03bb6a54abc1)
![Screenshot from 2024-10-26 00-11-37](https://github.com/user-attachments/assets/52685894-0824-4e84-ba77-1f7d8b16c0c1)

CONCLUSION : The Functionality vs Synthesized output waveform matches, i.e, O1 = O2.



# asic-design activity 10
Static Timing Analysis for a Synthesized RISC-V Core with OpenSTA
## Tools Installation
### CUDD Download:-
cd
tar xvfz cudd-3.0.0.tar.gz
cd cudd-3.0.0
./configure
make
### openSTA:-
cd
sudo apt-get install cmake clang gcc tcl swig bison flex

git clone https://github.com/parallaxsw/OpenSTA.git
cd OpenSTA
cmake -DCUDD_DIR=/home/solo/cudd-3.0.0
make
app/sta
![Screenshot from 2024-10-28 21-43-56](https://github.com/user-attachments/assets/e3f833db-ea8b-4823-9f21-e6f6a9c1b1cb)

## Steps to do Timing Analysis
Clock period = 10.55ns
Setup uncertainty and clock transition will be 5% of clock
Hold uncertainty and data transition will be 8% of clock.
 ### CODE-
 cd /home/solo/OpenSTA/app
./sta

read_liberty /home/solo/OpenSTA/lab10/sky130_fd_sc_hd__tt_025C_1v80.lib
read_verilog /home/solo/OpenSTA/lab10/likith_riscv_netlist.v
link_design rvmyth

create_clock -name clk -period 10.55 [get_ports clk]
set_clock_uncertainty [expr 0.05 * 10.55] -setup [get_clocks clk]
set_clock_uncertainty [expr 0.08 * 10.55] -hold [get_clocks clk]
set_clock_transition [expr 0.05 * 10.55] [get_clocks clk]
set_input_transition [expr 0.08 * 10.55] [all_inputs]


report_checks -path_delay max
report_checks -path_delay min

![Screenshot from 2024-10-28 21-56-13](https://github.com/user-attachments/assets/bcb67230-ea13-467a-abfa-d41937c9a5e8)
![Screenshot from 2024-10-28 21-56-29](https://github.com/user-attachments/assets/ca08a3cc-10fc-448a-aba2-43a42a43c5c5)



# asic-design activity 11
## Static Timing Analysis for the synthesized VSDBabySoC with OpenSTA
### TERMINAL WINDOW
![Screenshot from 2024-11-05 00-04-24](https://github.com/user-attachments/assets/dcc2e422-9346-4216-b831-79f5c8897df1)
![Screenshot from 2024-11-05 00-04-15](https://github.com/user-attachments/assets/c2361f4b-4b1a-4006-984a-977fbd2319b6)


### TCL FILE
![Screenshot from 2024-11-05 00-05-34](https://github.com/user-attachments/assets/ec5eceef-cde1-4d9a-b3c1-8546a66d9b42)



### CONSTRAINT FILE
![Screenshot from 2024-11-05 00-04-52](https://github.com/user-attachments/assets/f91009cf-93e0-4391-900c-9b3f77a68996)

### VALUES
![Screenshot from 2024-11-05 00-03-16](https://github.com/user-attachments/assets/7934527a-81c4-4043-9223-45ce2d9d173b)

### OUTPUT GRAPHS
![1](https://github.com/user-attachments/assets/82d91dab-ab43-48f1-9e31-edf3f4c9a5e7)

![2](https://github.com/user-attachments/assets/710ee4ee-8aed-4eec-ac64-a086d8b0bd11)
![3](https://github.com/user-attachments/assets/01ffb185-41c0-4872-89a2-eb37d93b7071)


# asic-design activity 12
## Day 1 - Introduction to open-source EDA, OpenLANE and Sky130 PDK

1) Run 'picorv32a' design synthesis using OpenLANE flow and generate necessary outputs. Commands to invoke the OpenLANE flow and perform synthesis

![1 1](https://github.com/user-attachments/assets/fb428c37-a254-4874-af43-6e2bdf623f03)
![1 1 2](https://github.com/user-attachments/assets/80e22495-3281-4be7-a334-7c30a6b3a96b)
![1 1 3](https://github.com/user-attachments/assets/b9d5198b-2421-46e1-afd1-da7b4158a640)

2) Calculate the flop ratio. Screenshots of synthesis statistics report file with required values

   ![Screenshot 2024-11-13 155303](https://github.com/user-attachments/assets/f69d544b-b161-4c47-bbeb-fc41a354bb2b)

   Calculation of Flop Ratio and DFF % from synthesis statistics report file

Flop Ratio = 1613/14876 = 0.108429685 Percentage of DFFs = 0.108429685*100 = 10.8429685


## Day 2 - Good floorplan versus bad floorplan, and introduction to library cells

1) Run 'picorv32a' design floorplan using OpenLANE flow and generate necessary outputs. Commands to invoke the OpenLANE flow and perform floorplan
   ![2 1 2](https://github.com/user-attachments/assets/d182247f-0c69-44b4-b679-4e43e2cf1916)
   ![1 1 4](https://github.com/user-attachments/assets/83237242-3fcb-484b-b7cf-65a92472caa7)
2) Calculate the die area in microns from the values in floorplan def. Screenshot of contents of floorplan def
   ![image](https://github.com/user-attachments/assets/21607bd9-bdd9-4d2c-90d6-24ca79973074)
   1000 unit distance = 1 Micron Die width in unit distance = 660685-0 = 660685 Die height in unit distance = 671405-0 = 671405 Distance in microns = Value in unit distance/1000 Die width in microns = 660685/1000 = 660.685 Microns Die heigth in microns = 671.405 Microns
3) Load generated floorplan def in magic tool and explore the floorplan. Commands to load floorplan def in magic in another terminal
   ![2 1 3](https://github.com/user-attachments/assets/9c075f73-5905-4be1-bb03-4f05b533ccbd)
Equidistant placement of ports

![image](https://github.com/user-attachments/assets/73750aa5-e076-42c9-8917-9cd849574614)

Port layer as set through config.tcl
![image](https://github.com/user-attachments/assets/013a8f74-59ee-4df9-afdd-d35b9206f624)
Decap Cells and Tap Cells
![image](https://github.com/user-attachments/assets/0193f61c-c7e4-4b27-a9cc-177e8b5f53c8)

Diagonally equidistant Tap cells
![image](https://github.com/user-attachments/assets/a46bf596-c06c-49c8-bf27-5faa711f4098)

4) Run 'picorv32a' design congestion aware placement using OpenLANE flow and generate necessary outputs. Command to run placement
   ![2 1 4](https://github.com/user-attachments/assets/7b53b712-e96b-4c88-bd0f-02482c82059e)
5) Load generated placement def in magic tool and explore the placement. Commands to load placement def in magic in another terminal
   ![2 1 5](https://github.com/user-attachments/assets/8ab707c0-fb49-4db7-a400-7c5c78fc7a7a)
![image](https://github.com/user-attachments/assets/242fad22-6f7e-4a66-a41f-a4e9bbfb21ac)

## Day 3 - Design library cell using Magic Layout and ngspice characterization

1) Clone custom inverter standard cell design from github repository
   ![3 1](https://github.com/user-attachments/assets/bb78b3f2-6274-47ee-a9bc-a0a176b2704e)

2)Load the custom inverter layout in magic and explore.
	![3 2](https://github.com/user-attachments/assets/fdf8e9f9-89bc-4af2-93fa-7e2c37dd0cab)

3) NMOS and PMOS identified, Output Y connectivity to PMOS and NMOS drain verified, PMOS source connectivity to VDD (here VPWR) verified, NMOS source connectivity to VSS (here VGND) verified
   ![3 3](https://github.com/user-attachments/assets/63c13ed7-d2c6-4167-a8e4-13d026193b97)
   ![3 4](https://github.com/user-attachments/assets/b33f71f8-b2b3-4d7a-b77e-153682d7de16)
   ![3 5](https://github.com/user-attachments/assets/79b51505-c43e-4f74-a41c-1e7884569dcd)
   ![3 6](https://github.com/user-attachments/assets/0082e115-71ca-45d8-9058-5b23c4bf63da)


4) Spice extraction of inverter in magic. Commands for spice extraction of the custom inverter layout to be used in tkcon window of magic
   ![3 7](https://github.com/user-attachments/assets/2880a212-dca7-443c-9521-9027ecca041e)

5) Screenshot of created spice file
 ![3 8](https://github.com/user-attachments/assets/ab3c03f7-23c7-40e7-91f0-0b0bd34d762f)

6) Post-layout ngspice simulations. Commands for ngspice simulation
   ![3 13](https://github.com/user-attachments/assets/5e66d95c-7633-4a4c-b865-b3610fd87117)
Screenshot of generated plot
![3 14](https://github.com/user-attachments/assets/801df72b-bbf4-4af0-85a2-bdbc31458f3c)
Rise transition time calculation

Rise transition time = Time taken for output to rise to 80% - Time taken for output to rise to 20%

20% of output = 660 mV 80% of output = 2.64 V

20% Screenshots

![3 15](https://github.com/user-attachments/assets/0c16984f-4b2b-410d-9422-54482d2a47d3)
![3 16](https://github.com/user-attachments/assets/99c1a3db-fe90-496b-9552-3faa156717d0)


80% screenshots
![3 18](https://github.com/user-attachments/assets/755ff3f7-6903-4562-9da5-2c4434c5d732)
![3 19](https://github.com/user-attachments/assets/dbf13256-2475-4d3e-9e2e-0fc868140c7c)

Rise transition time =

Fall transition time calculation

Fall transition time = Time taken for output to fall to 20% - Time taken for output to fall to 80%

20% of output = 660 mV 80% of output = 2.64 V

20% screenshots

![3 20](https://github.com/user-attachments/assets/aeb3811d-bdbf-4cc8-8548-a54f60c47beb)
![3 21](https://github.com/user-attachments/assets/357d27b3-a106-403a-8dc1-ec0790d9b305)
80% screenshots
![3 22](https://github.com/user-attachments/assets/4dd45ffe-d4fb-4a80-be8c-5db3e6937c28)
![3 23](https://github.com/user-attachments/assets/a1e27d6e-6fea-4c7a-aade-8d48c9999d6a)

Fall transition time =

Rise Cell Delay Calculation

Rise Cell Delay = Time take for output to rise to 50% - Time taken for input to fall to 50%

50% of 3.3 V = 1.65 V

50% screenshots

![3 24](https://github.com/user-attachments/assets/bad797ab-9a13-44f9-abed-6e6f3ebae425)
![3 26](https://github.com/user-attachments/assets/3a09e04d-be96-4a5c-992b-5955e49b1b52)

7) Find problem in the DRC section of the old magic tech file for the skywater process and fix them.
   ![3 27](https://github.com/user-attachments/assets/a4fe9d40-3a6e-4e81-a999-df8dd86f6089)
![3 28](https://github.com/user-attachments/assets/ec594bbc-8808-4197-ae8a-a6b93ea76836)
Incorrectly implemented poly.9 simple rule correction
![Screenshot 2024-11-13 194021](https://github.com/user-attachments/assets/3e7e175a-cd4a-45f7-9276-3bd956802f01)

8)making changes

![3 31](https://github.com/user-attachments/assets/609d0b1a-196e-49e4-a84a-b4a63f95e85d)
![3 30](https://github.com/user-attachments/assets/53602ca2-83d1-4535-b913-45450d1c8d92)
![3 29](https://github.com/user-attachments/assets/c7ebd684-ba8b-4fba-b662-6527a3d95eab)

## DAY 4 : Pre-layout timing analysis and importance of good clock tree

1. Fix up small DRC errors and verify the design is ready to be inserted into our flow.

  
   ![5 1](https://github.com/user-attachments/assets/6aef5355-c525-4b76-91ea-7ca905a1b1bc)
Commands for tkcon window to set grid as tracks of locali layer

![5 2](https://github.com/user-attachments/assets/4a9ba92f-4b03-40c2-8fda-aa72bc72fdf0)
![5 3](https://github.com/user-attachments/assets/e2bebc16-b3c0-4c20-b527-c84c8b916013)
![5 4](https://github.com/user-attachments/assets/b7414559-fc4e-49fc-b841-70ded0dbb071)
Condition 1 verified
![5 5](https://github.com/user-attachments/assets/955f4251-7afd-4f5a-993a-c8608cc791c9)

2) Saving it by giving a custom name

3) Generate lef from the layout.

   ![5 6](https://github.com/user-attachments/assets/8aae8e5b-faf3-474e-9a02-ce46f29d1e02)
 ![5 7](https://github.com/user-attachments/assets/31be2bd3-cb79-4fa9-a759-3595047de9a8)
![5 8](https://github.com/user-attachments/assets/e3d19f73-cb2f-407f-8275-f6a5129a83e5)
5)Copy the newly generated lef and associated required lib files to 'picorv32a' design 'src' directory.
![5 9](https://github.com/user-attachments/assets/9904f591-0117-402d-8d39-76501d0bd498)

6) Modify config.tcl:

7) Now, run openlane flow synthesis:

  ![5 10](https://github.com/user-attachments/assets/0e367b45-c83e-4e98-80a5-1dc4e55891ac)

  8) Remove/reduce the newly introduced violations with the introduction of custom inverter cell by modifying design parameters.


Screenshot of merged.lef in tmp directory with our custom inverter as macro
![5 11](https://github.com/user-attachments/assets/090a9f54-dfcf-48bc-b721-ebe9c8d00be8)

Screenshots of commands run
![5 14](https://github.com/user-attachments/assets/aadbe7ad-4586-494a-9b58-3894308f8c89)
![5 15](https://github.com/user-attachments/assets/79410a47-bfe6-44e1-af0b-d3241547d740)



9) open a new terminal and run the below commands to load placement def in magic

![5 16](https://github.com/user-attachments/assets/24d46ef8-f5a0-47be-b945-f3a688bc07fb)
![5 17](https://github.com/user-attachments/assets/7eae6e09-e846-4ecf-ba4b-69abaf9cf03b)
Now, select the cell and type expand in tkcon window to view internal layers of cells

![5 18](https://github.com/user-attachments/assets/6ef3497d-fb57-412c-9446-8edfe7380ae5)

10) Timing analysis with ideal clocks using openSTA


![5 24](https://github.com/user-attachments/assets/fc18f940-558d-43fb-a638-6c4bab6e49dd)


11) We now try to optimise synthesis.

![5 21](https://github.com/user-attachments/assets/fe0875c1-6e04-4744-b2b7-0b3d5274f282)

![5 25](https://github.com/user-attachments/assets/3e69e609-ad2f-4f96-a916-b40cc6d59348)

12) Basic timing ECO
    NOR gate of drive strength 2 is driving 5 fanouts

![eco1](https://github.com/user-attachments/assets/320b577e-eb13-4838-82ac-c68ab62ed58a)



![eco2](https://github.com/user-attachments/assets/ef043f66-4ef1-4467-850b-8328717a088b)


13)  Replace the old netlist with the new netlist generated after timing ECO fix and implement the floorplan, placement and cts.

Verified that the netlist is overwritten

 ![5 26](https://github.com/user-attachments/assets/a6922f2f-bf5b-4583-9dd5-5ddc512b9e6b)
Now, run the following commands:

![v1](https://github.com/user-attachments/assets/7406415b-bfea-44d0-a840-5406788e823f)
![v2](https://github.com/user-attachments/assets/dac4a421-2c3d-4ec3-8fea-a17c1a764ed1)
![v3](https://github.com/user-attachments/assets/a25ec402-b268-4431-890b-57a74119f9d7)
![v4](https://github.com/user-attachments/assets/585ba1b2-bda4-4008-8123-75cb28394d23)
![v5](https://github.com/user-attachments/assets/c6bee699-15b1-478e-9884-a67048fbbb89)
![v6](https://github.com/user-attachments/assets/82993611-24c8-41f4-9b94-61a6f837bfb4)

14) Setup timing analysis using real clocks
    ![v7](https://github.com/user-attachments/assets/0a996151-7888-4457-a280-d74942da8e14)
    ![v8](https://github.com/user-attachments/assets/a713bd0a-2507-472b-8e2f-be3fff8ca228)
    ![v9](https://github.com/user-attachments/assets/24a4b227-ad6a-4e7d-bb6c-8adf62967690)
![v10](https://github.com/user-attachments/assets/94396c5e-a6bd-48dd-96d7-47eaefba03a2)

![v11](https://github.com/user-attachments/assets/406abe80-61fd-4e29-b5cb-8eaa2cdcb111)
![v8](https://github.com/user-attachments/assets/a55072b2-b317-4750-84dc-a9842c83584e)
![v9](https://github.com/user-attachments/assets/2e31853c-d933-484c-98dd-ed082de8e909)
![v11](https://github.com/user-attachments/assets/798c506a-3982-40dd-bb81-ec99a49b6b72)



15) Now, enter the following commands for exploring post-CTS OpenROAD timing analysis by removing 'sky130_fd_sc_hd__clkbuf_1' cell from clock buffer list variable 'CTS_CLK_BUFFER_LIST':

![v12](https://github.com/user-attachments/assets/c18604fd-52d3-4661-81d9-e0b9682043f5)
![v13](https://github.com/user-attachments/assets/5c87306b-1caa-437f-8cba-77b93b2b968c)
![v14](https://github.com/user-attachments/assets/ba972165-8a67-49b6-a841-d62d1b995c00)
![v15](https://github.com/user-attachments/assets/bd274930-9259-4156-9aeb-6cb44ba6062a)
![v16](https://github.com/user-attachments/assets/4f228a98-fcf0-42d3-9030-8071c6a8e3df)

## Day 5 - Final steps for RTL2GDS using tritonRoute and openSTA
### Design Rule Check
1)Command to generate Power Distribution Network (PDN):
gen_pdn
![20 1](https://github.com/user-attachments/assets/d75691bf-16f0-41aa-9c72-ec5d89453651)
Now, in a new terminal
![20 2](https://github.com/user-attachments/assets/6df68341-9853-44c2-a97b-e4a08c9fdb28)
![20 3](https://github.com/user-attachments/assets/07d00f0c-cbb4-46ac-808f-419dc3375bf2)
searching for soloinv
![20 4](https://github.com/user-attachments/assets/cc050bf7-1a68-4167-96c6-30c808f0138c)
![20 5](https://github.com/user-attachments/assets/277d9925-6cd7-40df-8426-fd92436e3f7d)

2) Now, we perfrom detailed routing using TritonRoute:
   ![20 6](https://github.com/user-attachments/assets/7b8d448f-f1e6-441a-a91c-50a525933faf)

![20 7](https://github.com/user-attachments/assets/df804cc9-c3ce-4f96-b7d2-cd4a168c5126)
![20 8](https://github.com/user-attachments/assets/f86955c7-71ea-4586-bfdd-afe831f174ae)
![20 9](https://github.com/user-attachments/assets/b33c3db4-e3ba-4c5f-bfce-e76dd6f00747)
Now, in a new terminal
![20 10](https://github.com/user-attachments/assets/3e416d25-33d2-4c4f-b7e0-9b70c2d2da20)

![20 11](https://github.com/user-attachments/assets/d194fd6d-4c27-46c1-9b5f-62b4b8f6fb6a)
![20 12](https://github.com/user-attachments/assets/948ceac6-e018-4d76-ac91-0161447a0420)
searching for soloinv
![20 13](https://github.com/user-attachments/assets/a7da2358-d264-4fda-9042-8a5acd4a0089)
![20 14](https://github.com/user-attachments/assets/46a84637-e0cf-41a7-bd10-09ee33509dcc)
3) Fast route guide present in openlane/designs/picorv32a/runs/25-03_18-52/tmp/routing
![20 15](https://github.com/user-attachments/assets/6b5e308b-d2e0-4a29-a03c-85f5cbc607d4)
4) Commands for SPEF extraction Post-Route parasitic extraction using SPEF extractor
![20 16](https://github.com/user-attachments/assets/5bc8c40d-3c06-459d-b9f3-ca0de3c07a73)
![20 17](https://github.com/user-attachments/assets/591fb74e-c425-44b8-8439-74f069a4c956)

5) Commands for Post-Route OpenSTA timing analysis with the extracted parasitics of the route:
   ![20 18](https://github.com/user-attachments/assets/b1639d4d-c69a-403f-b392-9cc4a1f2c68b)
   ![20 19](https://github.com/user-attachments/assets/7b5cbc8d-1f99-4bc0-876d-67a8d7361d56)
   ![20 20](https://github.com/user-attachments/assets/8de830e9-128c-498f-99c1-901078eaabb5)
   ![20 21](https://github.com/user-attachments/assets/72ac9664-c81a-4a4f-9eb5-e079abb08129)

--------------------------end----------------------

# Task-13: OpenRoad Physical Design
## Introduction
### Bombe  
The Bombe was an electro-mechanical machine developed during World War II to decrypt messages encrypted by the German Enigma machine. Built by Alan Turing and Gordon Welchman at Bletchley Park in the UK, it systematically analyzed potential rotor settings of the Enigma by leveraging known patterns in plaintext. The machine's logical operations greatly reduced the number of possible keys, significantly expediting the decryption process. Its contributions were pivotal to the Allied victory in the war.  

### ENIAC (Electronic Numerical Integrator and Computer)  
ENIAC, developed during World War II by John Presper Eckert and John Mauchly at the University of Pennsylvania, was the first fully electronic, general-purpose digital computer. Completed in 1945, it was designed to calculate artillery firing tables for the U.S. Army. Unlike earlier machines, ENIAC relied on vacuum tubes rather than mechanical or electromechanical parts. Although it lacked the ability to store programs internally and required manual reconfiguration for new tasks, it showcased the vast potential of electronic computing for solving large-scale numerical problems.  

### EDVAC (Electronic Discrete Variable Automatic Computer)  
EDVAC, also developed by Eckert and Mauchly with conceptual guidance from John von Neumann, introduced the stored-program architecture, a breakthrough in computing. Completed in 1949, it used binary representation instead of decimal and stored both instructions and data in memory, simplifying programming and enabling more complex operations. This innovation laid the foundation for the modern von Neumann architecture and marked a significant evolution from ENIAC.

## Installing and setting up ORFS
![Screenshot from 2024-11-25 16-10-16](https://github.com/user-attachments/assets/ab351212-4841-4736-b2f0-611cf3a854d8)
Verify Installation
![Screenshot from 2024-11-25 16-37-48](https://github.com/user-attachments/assets/24843358-f216-460f-ab4b-b2406025e205)
![Screenshot from 2024-11-25 16-37-48](https://github.com/user-attachments/assets/74c1ad27-9f44-4318-b998-4ea60d39828a)

 
![Screenshot from 2024-11-25 17-20-58](https://github.com/user-attachments/assets/3b6db3e7-2992-454a-8683-bb03b3cb76a2)

![Screenshot from 2024-11-25 17-23-48](https://github.com/user-attachments/assets/1df845b8-136c-4176-97fa-a969320987c1)

## make gui_final

![Screenshot from 2024-11-25 17-41-14](https://github.com/user-attachments/assets/00459056-1dd8-4b02-82c5-23d6650519c2)

![Screenshot from 2024-11-25 17-36-58](https://github.com/user-attachments/assets/e06ff10f-a49a-4595-adf4-f094a07b948a)

## file directory
![image](https://github.com/user-attachments/assets/aced30c4-f13e-4e96-a080-6c355139d1cb)

├
![image](https://github.com/user-attachments/assets/90c08ab7-dd67-4473-b1f8-63796f808c8b)

        

## Commands for synthesis:

![Screenshot from 2024-11-25 23-31-28](https://github.com/user-attachments/assets/020a957f-7e1d-4321-af3c-b472cfecbd7d)

![Screenshot from 2024-11-25 23-31-16](https://github.com/user-attachments/assets/317ccc26-24de-479e-b7ec-8d8fa48f04cf)

### Synthesis netlist:


![image](https://github.com/user-attachments/assets/052b3fcc-370c-4c85-94b4-0c86deb651d2)

### Synthesis log:
![image](https://github.com/user-attachments/assets/3e123f4f-aef2-4b45-98c1-5415583aa6af)

![image](https://github.com/user-attachments/assets/12f4a653-ec83-44cf-a65e-e8645c4b5b06)

### Synthesis Check:


![Screenshot from 2024-11-25 23-58-07](https://github.com/user-attachments/assets/c05143ff-ff31-4043-b364-be7e9bb20c0f)

### Synthesis Stats:
![image](https://github.com/user-attachments/assets/447f8671-2d9e-4b43-a497-1557fb51fe9d)

![image](https://github.com/user-attachments/assets/3e453d41-3d7a-49d9-9817-bfac98ba95a1)


## Commands for floorplan:

![Screenshot from 2024-11-25 23-55-04](https://github.com/user-attachments/assets/bc629443-c588-4903-bd99-14335258b713)

![Screenshot from 2024-11-25 23-54-37](https://github.com/user-attachments/assets/f950e371-1658-4ad1-af7a-cc947a808d80)


### make gui_floorplan
![image](https://github.com/user-attachments/assets/09501e0b-206b-491e-9afc-ef79207d873e)


![image](https://github.com/user-attachments/assets/ad14d3e9-9d01-419b-83ed-f6cbdf64104d)
![image](https://github.com/user-attachments/assets/bc509033-230f-483a-80b0-35d093b44f17)

### FLOORPLAN_LOG
![image](https://github.com/user-attachments/assets/b81f9a06-0d38-485c-a538-6f12c18e9b0e)

### FLOORPLAN TIMING REPORT
![image](https://github.com/user-attachments/assets/1805b479-57ee-48bb-a8bd-31723f53a619)
![image](https://github.com/user-attachments/assets/231ab041-9a40-46bd-92e5-6290c4c29ad0)


### sudo make DESIGN_CONFIG=./designs/sky130hd/vsdbabysoc/config.mk gui_floorplan
![image](https://github.com/user-attachments/assets/4e285503-305f-4539-a4ce-f726f3315195)

![image](https://github.com/user-attachments/assets/53a96a0d-a17a-491d-8e30-ac2dfab15ce6)


## For Placement
### sudo make DESIGN_CONFIG=./designs/sky130hd/vsdbabysoc/config.mk place

![image](https://github.com/user-attachments/assets/f0d85ad1-f1c5-4627-a57f-cce4a00453b6)

![image](https://github.com/user-attachments/assets/f5feacb0-a28d-4fc4-bc86-56b8443a527f)


## make gui_place

![image](https://github.com/user-attachments/assets/190010c8-e962-485b-beb7-3ad3f8153988)


![image](https://github.com/user-attachments/assets/b14a164e-79a9-492a-b149-2517096c8a5c)


![image](https://github.com/user-attachments/assets/b72a6698-8b3c-4b77-9e5b-a4fc5339466d)


![image](https://github.com/user-attachments/assets/fc265a64-6e4f-44d8-85df-8a5fb303faf1)

### PLACE_REPORT
![image](https://github.com/user-attachments/assets/d2c93956-c18d-47b3-821e-7230658d3291)
![image](https://github.com/user-attachments/assets/64871043-158a-4093-8d4f-c464179dbe27)
![image](https://github.com/user-attachments/assets/8d8525c6-94ee-40e5-925e-172fc4e59f6d)

## CTS Command

![image](https://github.com/user-attachments/assets/bf50762f-3b58-47b4-9661-0439ad3afafc)
![image](https://github.com/user-attachments/assets/3e07f9e1-71e3-4a98-a8f6-f811c4f010e2)

### make gui_cts

![image](https://github.com/user-attachments/assets/b73eb10c-2ec6-4ca0-b8be-54da8a833a27)



![image](https://github.com/user-attachments/assets/42884ddd-982d-44bb-bda3-76cbd2b04a15)

![image](https://github.com/user-attachments/assets/11fa41ab-d71a-44ca-b714-375ca65dfdc5)

## MACRO PLACEMENT
for the fllowing file
![image](https://github.com/user-attachments/assets/ea8a2aa9-56b1-456a-9afd-4b084ea07aa6)

###  ORFS
![Screenshot from 2024-11-26 03-25-51](https://github.com/user-attachments/assets/1de11ab9-484b-4394-a107-3fa1152314f5)

![Screenshot from 2024-11-26 03-25-57](https://github.com/user-attachments/assets/3d7bb9a5-29f0-4024-a508-1517f34ba94b)
![image](https://github.com/user-attachments/assets/110ad351-52c6-4dad-a6fe-a74d623d89f0)


### clock tree synthesis 

![image](https://github.com/user-attachments/assets/7058806c-b00e-47f2-b2f3-a879ed6dae2f)

![image](https://github.com/user-attachments/assets/dc5e0d9a-7354-4300-809d-257cdc955fcc)

![image](https://github.com/user-attachments/assets/2ab31385-2536-417b-bd00-209af4860b57)

![image](https://github.com/user-attachments/assets/619398c0-a953-4f19-8ed0-795d0cd12e61)


### HEAT MAP
![WhatsApp Image 2024-11-26 at 6 11 15 AM](https://github.com/user-attachments/assets/8fd1ea20-b9cb-4789-bd5f-79213bc2a6dc)
![WhatsApp Image 2024-11-26 at 6 11 15 AM](https://github.com/user-attachments/assets/270d7f72-aadb-4354-a1f4-8e73bf9b44b4)
![WhatsApp Image 2024-11-26 at 6 11 11 AM](https://github.com/user-attachments/assets/e1784bc6-4b64-4354-a850-c0094725b8e8)

## For Route
### make gui_route

![image](https://github.com/user-attachments/assets/eae736db-8f03-42f3-b811-6471411c0438)



![image](https://github.com/user-attachments/assets/b86f4f82-48c5-4514-9d31-44d3c9f7161e)

### make gui_final
![image](https://github.com/user-attachments/assets/85e519f7-48ea-4c68-bf9d-fe32499bba65)
![image](https://github.com/user-attachments/assets/77ca1e68-e41b-43aa-971c-55bef00c54d3)
	![image](https://github.com/user-attachments/assets/0b06d4a6-d276-4477-871e-b437c44d9339)
![image](https://github.com/user-attachments/assets/9bdb443b-556d-4f7d-81a1-f106055a23a7)
### To give the GDS file in the klayout type the following commands
![image](https://github.com/user-attachments/assets/0b470bd2-3722-4f17-9760-b6eb715e9585)

![image](https://github.com/user-attachments/assets/95353c05-81d9-46f0-a437-0a43fa9b2342)
![image](https://github.com/user-attachments/assets/fc1907be-f8b5-40fc-a52e-9c71f18c07b6)
![image](https://github.com/user-attachments/assets/795791e3-ad85-49a7-b33d-5d347f91a79a)
## ROUTING
### Route Command
![image](https://github.com/user-attachments/assets/4b6dbb29-3cec-4879-8556-752a75482ba7)
![image](https://github.com/user-attachments/assets/08c99b0e-0bc0-4b45-ac81-d0e12db6dddc)
![image](https://github.com/user-attachments/assets/3eabc211-49f9-4f2b-aac1-d95a1fdc8405)

![image](https://github.com/user-attachments/assets/3a45da2e-b79a-4a0f-b4e1-8547ae2f66b9)
### make gui_route
![image](https://github.com/user-attachments/assets/c89552d5-9631-4065-9b95-a331ee242388)

![image](https://github.com/user-attachments/assets/cab75a21-afa1-4c93-b739-97de51595a94)
![image](https://github.com/user-attachments/assets/3e72adb8-39ba-4e64-baed-fdc843432477)
