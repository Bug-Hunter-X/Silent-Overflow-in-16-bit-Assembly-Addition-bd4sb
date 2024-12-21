# Silent Overflow in 16-bit Assembly Addition

This repository demonstrates a common error in assembly programming: silent overflow in 16-bit addition.  The `add` instruction, when used with 16-bit registers like `ax`, silently truncates any bits beyond the 16-bit limit if an overflow occurs. This can lead to subtle and hard-to-debug errors.

The `bug.asm` file contains the erroneous code. The `bugSolution.asm` file shows how to handle potential overflows using appropriate checks and/or larger registers (e.g. 32-bit).