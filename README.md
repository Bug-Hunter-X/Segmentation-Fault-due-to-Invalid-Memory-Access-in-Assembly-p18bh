# Segmentation Fault in Assembly Code

This repository demonstrates a common error in assembly programming: accessing memory outside the program's allocated address space. This can lead to segmentation faults and program crashes.  The `bug.asm` file contains the erroneous code, while `bugSolution.asm` provides a corrected version.

## Bug Description

The problem lies in the memory access calculation.  The code attempts to dereference a pointer that points outside of the valid memory region, leading to unpredictable behavior. This is a classic example of a segmentation fault.

## How to Reproduce

1. Assemble the `bug.asm` code using your preferred assembler (e.g., NASM, MASM).
2. Run the resulting executable. You should observe a segmentation fault or a similar error.

## Solution

The `bugSolution.asm` file provides a corrected version of the code.  The solution involves carefully checking the calculated memory address before attempting to access it, either by adding boundary checks or by ensuring correct pointer arithmetic.