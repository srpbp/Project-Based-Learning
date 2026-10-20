# Project-Based Learning — C

Coursework from a university **C programming** module. The repo currently
contains one project: a terminal-based **vending machine simulator**.

## First Project — Vending Machine

A single-file C program that simulates a drinks vending machine. Covers the
basics the course was aiming at: `printf` / `scanf`, control flow with `if`
and nested `switch`, globals and constants, functions, user input validation
loops, and `exit()`.

### Features

- ASCII-art splash screen
- Insert cash with lower / upper balance limits (1,000 – 1,000,000 LAK)
- Buy from 5 items — Coke, Pepsi, Sprite, Monster, 7UP — each with its own
  price and insufficient-balance guard
- Check current balance
- Top up balance mid-session
- Cash out (with Y/N confirmation)
- Exit

### Build & run

The source file is `First Project` (no extension). Compile with any C
compiler:

```bash
gcc "First Project" -o vending
./vending
```

Or with clang:

```bash
clang "First Project" -o vending && ./vending
```

### Example session

```
===============================
        Vending Machine
===============================
        _______________
        |---------|   |
        |---------|===|
        ...
===============================
Insert your money: 20000

Welcome!

[1] Buy an item
[2] Check your balance
[3] Insert balance
[4] Cash out
[5] Exit
Please select: 1

Choose your item

[1] Coke 10,000 LAK
[2] Pepsi 10,000 LAK
[3] Sprite 8,000 LAK
[4] Monster 15,000 LAK
[5] 7UP 7,000 LAK
Please select: 1
Purchased Coke!
Remaining balance: 10000
```

## Repo layout

```
First Project       The C source (compile with gcc / clang).
.gitattributes      Forces GitHub to detect the file as C.
README.md           This file.
```
