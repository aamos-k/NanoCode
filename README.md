# The ***NANO-CODE*** Instruction Set ##
## by aamos k ##
### loosely based on the [***RISC-V***](https://www2.eecs.berkeley.edu/Pubs/TechRpts/2016/EECS-2016-118.pdf) architecture

---
## Registers

### From RISC-V the instruction length encoding is simplified by simply not using it 
### and only having 1 byte used for the instruction it's self and up to 16 general-purpose 8 bit registers
### other registers include the accumulator (8 bits), stack pointer (4 bits) + flags (4 bits) and 
### program counter (16 bits)
### flags include negative, zero, carry,

## Instructions
## integer math 
* ### ada |a|1-16| |1-16| (add a or register and register)
* ### sba |a|1-16| |1-16| (subtract a or register and register)
## logic operations
* ### ora |a|1-16| |1-16| (or a or register and register)
* ### ana |a|1-16| |1-16| (and a or register and register)
* ### era |a|1-16| |1-16| (exclusive or a or register and register)
* ### naa |a|1-16| |1-16| (not and a or register and register)
## other operations
* ### cmp |a|flags| |a|1-16| (compare a or flags and a or register and deposite to flags)
