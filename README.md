# omar-cpu

An 8-bit single-cycle CPU built from scratch: custom instruction set, 
hand-designed datapath and control unit in Logisim Evolution, and a 
Python assembler to write programs for it.

![demo](docs/demo.gif)

## Features
- 8-bit data path, 16-bit instructions, 8 general-purpose registers
- Harvard architecture (separate program and data memory)
- Zero / Negative / Carry flags with conditional branching
- Python assembler with labels and comments
- Demo programs: Fibonacci, multiplication, counter loop

## Quick start
1. Install [Logisim Evolution](https://github.com/logisim-evolution/logisim-evolution)
2. Write a program in `programs/fib.asm`
3. Run `python assembler/assembler.py programs/fib.asm -o fib.hex`
4. Load `fib.hex` into the program memory in `cpu.circ` and start the clock
