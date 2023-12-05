***
**Representing Instructions in the Computer**

![[Pasted image 20231203225309.png]]

- MIPS R-format:

op | rs | rt | rd | shamt | funct
:--:|:--:|:--:|:--:|:--:|:--:
6 bits| 5 bits|5 bits|5 bits | 5 bits | 6 bits
  1. op: Operation code(Opcode)
  2. rs: First source register number
  3. rt: second source register number
  4. rd: destination register number
  5. shamt: shift amount
  6. funct: function code (extends opcode)

- MIPS I-format

op | rs | rt | constant or address
:--:|:--:|:--:|:--:
6 bits| 5 bits | 5 bits | 16 bits
1. op: Operation code(Opcode)
2. rs: First source register number
3. r: destination or second source register number
4. Constant: $-2^{15} to + 2^{15} - 1$
5. Address: offset added to base address in rs

- MIPS J-format

op | address
:--:|:--:
6 bits | 26 bits
1. op: Operation code(Opcode)
2. Address: jump to target address
* * *
### **Arithmetic and Logic instruction groups**

Operation| MIPS | Format 
:--:|:--:|:--:
Add| add/addu,addi/addiu| R,I
Minus| sub, subu| R
Set if less than| slt/sltu, slti/sltiu | R, I
Shift left | sll | R
Shift right | srl | R
Bitwise AND | and, andi | R,I
Bitwise OR | or, ori | R, I
Bitwise NOT| nor| R

**shamt**: How many positions to shift
- Shift left logical
	- Shift left and fill with 0 bits 
	- sll by i bits multiplies by $2^{i}$ 
- Shift right logical
	- Shift right and fill with 0 bits 
	- srl by i bits divides by $2^{i}$ 
- AND
	- 0 and 1 => 0
	- 0 and 0 => 0
	- 1 and 1 => 1
- OR
	- 0 or 1 => 1
	- 0 or 0 => 0
	- 1 or 1 => 1
- NOR
	- 0 nor 1: not (0 or 1) => not(1) => 0
	- 0 nor 0: not (0 or 0) => not(0) => 1
	- 1 nor 1: not (1 or 1) => not(1) => 0
Conditional branch instructions
![[Picture1.png]]![[Picture2.png]]

