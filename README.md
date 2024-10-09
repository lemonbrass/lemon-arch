## What is it?
A toolchain for building near native speed programs that can run on virtually any possible platform.

## Brief
This project includes: 
 -  a CPU with an unconventional Bitstream based instructions
 -  unix-like OS for the CPU
 -  a C backend (possibly a LLVM backend) for the CPU.

## Philosophy
The main idea behind lemon-arch is that platform shouldn't restrict you from programming, the main bottleneck should be skills instead of platform-dependent stuff.

## State
Currently, the CPU Instruction set is in development, the instruction set pdf will be pushed when it is completed

The programming for this project has not initiated as currently, I am working in its design.

## CPU 
It has a bitstream based ISA with the first byte as header byte containing conditions, type of instruction, size of remaining instruction, no. of operands, etc.

This makes encoding/decoding process simpler and efficient, so actual time by cpu is spent running the instructions instead of decoding them.

(this project is in its early stages and ISA is subject to changes)
