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
* ### ada |a|1-16| |1-16| (add a or register and register and deposite to a)
* ### sba |a|1-16| |1-16| (subtract a or register and register and deposite to a)
* ### add |1-16| |1-16| (add register and register and deposite to register)
* ### sub |1-16| |1-16| (subtract register and register and deposite to register)
* ### ror |1-16| |1-16| (rotate right and deposite to register)
* ### rol |1-16| |1-16| (rotate left and deposite to register)
## logic operations
* ### ora |a|1-16| |1-16| (or a or register and register and deposite to a)
* ### ana |a|1-16| |1-16| (and a or register and register and deposite to a)
* ### era |a|1-16| |1-16| (exclusive or a or register and register and deposite to a)
* ### naa |a|1-16| |1-16| (not and a or register and register and deposite to a)
* ### or |1-16| |1-16| (or register and register and deposite to register)
* ### and |1-16| |1-16| (and register and register and deposite to register)
* ### eor |1-16| |1-16| (exclusive or register and register and deposite to register)
* ### nan |1-16| |1-16| (not and register and register and deposite to register)
## memory instructions
* ### mva |a|1-16| |a|1-16| (move a or register to a or register)
* ### mov |mem|1-16| |mem|1-16| (move memory or register to memory or register)

## other operations
* ### cma |a|flags| |a|1-16| (compare a or flags and a or register and deposite to flags)
* ### cmp |1-16| |1-16| (compare register and register and deposite to register)
