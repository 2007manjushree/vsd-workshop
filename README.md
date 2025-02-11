# Advanced Physical Design using Openlane/SKY130
## Day 1

Arduino Board: Commonly used electric board. The main processor chip is circled.

![image](https://github.com/user-attachments/assets/6360ee07-a056-4908-ae02-6bc8a9cad416)

Diagram of the typical Chip

![image](https://github.com/user-attachments/assets/4b4f2b0b-9165-4139-94b2-72487f50aa3c)

Chips are professionally known as Package. 
Example: QFN-48 (here, 48 is the number of pins), Quad Flat No-leads

Components: 

- Chip: placed at the centre
- Pins: allows to receive information from the outside world
- Wire Prongs: connects the pins to the chip

![image](https://github.com/user-attachments/assets/15ccf588-f35c-4187-91e4-240993343637)

Chip Components:

- Pads: allows signal to be sent in and out the chip
- Core: all the digital logic gates are present
- Die: part of semiconductor wafer used independently in devices

![image](https://github.com/user-attachments/assets/f7032ec3-c1b7-4d0c-bfc8-f63462aefdb7)

Example: RISK-V SoC

Core Components:
- Foundry IPs (Intelectual Properties): Components designed in a foundry (a manufacturing unit for chips) which require intelligence to operate. Communication with the foundry happens through interface files. Includes SRAM, PLL, adc, dac, etc.
- Macros: Pure digital logic. Includes RISK-V SoC, SPI, etc.

![image](https://github.com/user-attachments/assets/78cc3d48-338e-4039-8b29-b2b77fd63254)

RISC-V ISA (Instruction Set Architecture): Language used to talk to the computer (C program onto hardware)

- C program compiled in RISK-V Assembly language program and converted to machine language program i.e. binary language
- RISK-V specs implemented onto hardware using a Hardware Description Language (example: picorv32 cpu core)
- Layout takes in the program and gives desired output

![image](https://github.com/user-attachments/assets/326b0439-44b1-4067-988a-9fd7e0b406fa)

Application Software → System Software → Hardware i.e. Chip

System Software:

- Operating System OS: Handles IO i.e. Input/Output operations, allocates memory, low-level system functions
- Compiler: Converts C/C++/VB/JAVA/etc. to Instructions file *.exe (syntax of instructions based on the type of chip)
- Assembler: Converts Instructions to Machine Language Program i.e. Binary Language for chip

![image](https://github.com/user-attachments/assets/a4701241-e7aa-4679-8c25-b3977675aeff)

Example: Stop Watch Application

![image](https://github.com/user-attachments/assets/8fa4ec5c-b1d8-4de8-bb44-631c4fffab96)

Image 1 - Compiler Input
Images 2 & 3 - Compiler Output (Hexadecimal numbers is output of assembler)

<img width="585" alt="image" src="https://github.com/user-attachments/assets/5255a9b9-6ad4-487f-a5bc-71f2299b2ee6" />

Instruction File aka Abstract Interface Instruction Set Architecture: acts as abstract interface between C/C++/VB/JAVA/etc. and Machine Language Program i.e. architecture of the computer

Step 1: Output of compiler is specifications 
Step 2: Hardware Description Language aka RTL Descriptional Language implements the specs of instruction set
Step 3: RTL gets synthesised into netlist (converted into logic gates)
Step 4: Physical Design Implementation of netlist into hardware layout
Step 5: Output of assembler is binary numbers
Step 6L Binary numbers fed into Hardware layout

![image](https://github.com/user-attachments/assets/2fa060da-2d09-49ca-ba91-56b20bedfbcb)













