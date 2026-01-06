# Memory Game (C)

A terminal-based memory matching game written in pure C.  
The project focuses on mastering core C fundamentals such as pointers, dynamic memory allocation, structs, input validation, and modular program design.

This is a learning-driven project. Visual polish is intentionally deprioritized in favor of correctness and low-level control.

---

## Overview

The game presents a hidden 4×4 board containing 8 pairs of values.  
The player reveals two cells per move and attempts to find matching pairs. Matched cells remain visible. The game ends when all pairs are revealed.

---

## Key Features

- 4×4 dynamically allocated game board  
- Each value appears exactly twice  
- Randomized board using Fisher–Yates shuffle  
- Input validation for all user actions  
- Move counter  
- Clear win condition detection  
- Terminal-only interface (no external libraries)

---

## Technical Constraints

This project intentionally follows strict rules:

- No global variables  
- No fixed-size 2D arrays for the board  
- Dynamic memory allocation using `malloc` and `free`  
- Board cells represented using `struct`  
- Logic split into multiple functions  
- No `goto` statements  

These constraints exist to enforce proper C practices.

---

## Concepts Practiced

- Pointer and pointer-to-pointer usage (`Cell **board`)  
- Dynamic memory allocation and deallocation  
- Struct-based data modeling  
- Array shuffling algorithms  
- Defensive programming  
- Game loop design  
- Separation of concerns  

---

## Build Instructions

Compile using GCC:

```bash
gcc main.c -o memory_game
