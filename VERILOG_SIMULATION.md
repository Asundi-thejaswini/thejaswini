# As per the Update given for the next task "Should Use the RISC-V Core Verilog netlist and testbench for functional Simulation.
# Veriog code is being executed and the waveforms are generated using the gtkwave

# Aim: To verify the Functional Simulation:-
# Table of contents
- [1.RISC-V RV32I](#1-RISC-V-RV32I)
 - [2.BLOCK DIAGRAM OF RISC-V RV32I](#2-BLOCK-DIAGRAM-OF-RISC-V-RV32I)
 - [3.INSTRUCTION SET OF RISC-V RV32I](#3-INSTRUCTION-SET-OF-RISC-V-RV32I)
 - [4.FUNCTIONAL SIMULATION](#4-FUNCTIONAL-SIMULATION)
    - [4.1 About iverilog and gtkwave](#41-About-iverilog-and-gtkwave)
    - [4.2 Installing iverilog and gtkwave](#42-Installing-iverilog-and-gtkwave)
    - [4.3 The output waveform](#43-The-output-waveform)
  
   ## 1. RISC-V RV32I

This project provides an insight into the working of a few important instructions of the instruction set of a Single cycle Reduced Instruction Set Computer - Five(RISC-V) Instruction Set Architecture suitable for use across wide-spectrum of Applications from low-power embedded devices to high-performance Cloud-based Server processors. The base RISC-V is a 32-bit processor with 31 general-purpose registers, so all the instructions are 32-bit long. Some Applications where the RISC-V processors have begun to make some significant threads are in Artificial intelligence and machine learning, Embedded systems, ultra-low power processing systems, etc.

## 2. BLOCK DIAGRAM OF RISC-V RV32I
![1](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/4748a6d4-1d79-4cb4-9834-61fca4df9abc)

## 3. INSTRUCTION SET OF RISC-V RV32I
![2](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/0212b82e-629d-4653-8b06-15199592a03e)

![3](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/fe623e0a-ca09-4bff-a3c5-b3bf5cdcd774)


## 4. FUNCTIONAL SIMULATION

### 4.1 About iverilog and gtkwave
- Icarus Verilog is an implementation of the Verilog hardware description language.
- GTKWave is a fully featured GTK+ v1. 2 based wave viewer for Unix and Win32 which reads Ver Structural Verilog Compiler generated AET files as well as standard Verilog VCD/EVCD files and allows their viewing.
  
### 4.2 Installing iverilog and gtkwave

- **For Ubuntu**

 Open your terminal and type the following to install iverilog and GTKWave
 ```
 $   sudo apt get update
 $   sudo apt get install iverilog gtkwave
 ```
![Screenshot from 2024-03-02 12-08-39](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/d30002f0-52f0-4772-8c08-f86084912958)

- **To clone the repository and download the netlist files for simulation, enter the following commands in your terminal.**

 ```
 $ git clone https://github.com/Abdulbitm/Abdul
 $ cd Abdul
```
![Screenshot from 2024-03-04 21-45-47](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/75e4e0df-c250-4da7-9375-cc4b2ed8253d)

- **To simulate and run the Verilog code, enter the following commands in your terminal.**

```
$ iverilog -o hello hello.v hello_tb.v
$ ./hello
```
![Screenshot from 2024-03-02 12-52-17.png](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/50497697-05fb-4b00-9853-c7cb24c2ab14)



- **To see the output waveform in gtkwave, enter the following commands in your terminal.**

`$ gtkwave hello.vcd`

![Screenshot from 2024-03-02 12-57-38](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/96d499b5-3242-4cbe-bf71-1be04a4f1eac)

### 4.3 The output waveform

 The output waveform showing the instructions performed in a 5-stage pipelined architecture.
 
 Instruction 1:add r6,r2,r1
<img width="1282" alt="309717644-9475de20-c117-476a-bebc-54dd3548c109" src="https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/2ce8edf3-0141-4508-8179-7f4db7d591d1">

 Instruction 2:sub r7,r1,r2
<img width="1280" alt="309717941-2c95f18f-191e-4500-9cda-e7e838d1e609" src="https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/0ded0c7d-3f1f-4289-861e-6df73f6e84d9">

Instruction 3:and r8,r1,r3
<img width="1282" alt="309718134-18bfdf76-1173-4984-b50b-83443ab48596" src="https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/ac4c3a4c-be89-4239-a24a-d4c38b7feda2">

Instruction 4:or r9,r2,r5
<img width="1294" alt="309718310-4f214bb2-c934-4778-bf46-841efe877fb8" src="https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/9c8d2f9f-ab9e-4a48-a39b-108587a95370">

 Instruction 5:xor r10,r1,r4
<img width="1293" alt="309718453-6fa91f49-5e73-4133-8bf6-84ec4aca64da" src="https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/93d69bd6-2f1f-47c3-b700-d6ec8213b511">

 Instruction 6:slt r11,r2,r4
<img width="1290" alt="309718574-c9c32048-62ed-4f55-8e11-9763816b1bd1" src="https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/a641d0c6-2c68-4463-9000-d4a53e3384fd">

 Instruction 7:addi r12,r4,5
<img width="1285" alt="309718717-308b8a9d-46c8-4a0e-8824-90e11d9a6a1e" src="https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/80c76b79-7610-4b89-b67a-c5b9b996c36a">

 Instruction 8:sw r3,r1,2
<img width="1280" alt="309718858-84f16d7f-9d16-4236-b64d-615e187a00ff" src="https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/149fd321-6926-44fd-bb30-9ca17b17e3b0">

 Instruction 9:lw r13,r1,2
<img width="1295" alt="309719046-c7bc7d9a-6745-4eeb-903d-fa723dca1394" src="https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/3a8f0614-e3e8-4887-acf1-342d2d0ceeba">

 Instruction 10:beq r0,r0,15
<img width="1287" alt="309719144-a1c6781f-c301-45d9-a502-fb32e6204e4c" src="https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/0d132698-b3e9-4a04-8c87-24777c8b832d">

 After branching, performing
 Instruction 11:add r14,r2,r2
<img width="1287" alt="309719297-56b50ce0-60aa-41fe-8f53-0b4583b39665" src="https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/92286760-87da-4d0c-affa-05bc90dc5cd6">

  Full 5-stage instruction pipeline and pc-increment description Waveform
<img width="1325" alt="309719447-e5ebc923-ad2c-44fc-a577-3ce7b8419bce" src="https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/05df603c-bbee-4d09-a61d-cf2aa0849670">

![Screenshot from 2024-03-02 12-54-10](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/46cf7bdb-3c56-41b6-8467-689ccaf03c46)

![Screenshot from 2024-03-02 12-41-22](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/96bd3bd6-36ba-4fd6-a7a3-2b0b85bea856)


