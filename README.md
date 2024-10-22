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
