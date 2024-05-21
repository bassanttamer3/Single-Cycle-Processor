

**Single-Cycle Processor Design in VHDL** 😎🚀

Our project focuses on designing a Single-Cycle Processor using VHDL. The processor supports both R-type and I-type instructions. Each instruction is executed in a single cycle, where all stages (instruction fetch, decode, execution, memory access, and write-back) occur simultaneously. Below is a summary of the supported instructions:

### R-type Instructions
- **Add**: Perform addition.
- **Sub**: Perform subtraction.
- **And**: Perform bitwise AND.
- **Or**: Perform bitwise OR.
- **Nand**: Perform bitwise NAND.
- **Slt**: Set on less than.

### I-type Instructions
- **Load word (lw)**: Load a word from memory.
- **Store word (sw)**: Store a word to memory.
- **Add immediate (addi)**: Add immediate value to a register.
- **Branch equal (beq)**: Branch if registers are equal.
- **Branch not equal (bne)**: Branch if registers are not equal.

### Instruction Execution Cycles
In a Single-Cycle Processor, all instructions are executed in one cycle, which encompasses the following stages:

1. **Instruction Fetch**: Retrieve the instruction from memory.
2. **Instruction Decode and Register Fetch**: Decode the instruction and read the necessary registers.
3. **Execution/Memory Address Computation/Branch Completion/Jump Completion**: 
    - Execute the operation for R-type instructions.
    - Compute the memory address for load/store instructions.
    - Complete the branch decision for branch instructions.
4. **Memory Access or R-type Instruction Completion**: 
    - Access memory for load/store instructions.
    - Complete the execution for R-type instructions.
5. **Memory Read Completion**: Complete the memory read for load instructions.


