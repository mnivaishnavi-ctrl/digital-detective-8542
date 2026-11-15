# Mission 4 — How Programs Run

## Task/objective

Write and run a short Python program, then learn the difference between compilers and interpreters.

## Work completed

- Created and ran `hello.py`, which prints `Hello from Python`.
- Compared compilers and interpreters in the table below.

| Topic | Compiler | Interpreter |
|---|---|---|
| When code is translated/run | Translates the program before it runs. | Translates and runs instructions as the program runs. |
| Typical output | Often creates machine code or an executable file. | Usually produces program results without a separate executable. |
| Example | GCC compiling C code. | CPython running Python code. |
| One advantage | Compiled programs can run quickly. | Programs can be tried and debugged without a separate compile step. |

## Commands/tools used

- `/usr/local/bin/python3.14 mission-04-programs/hello.py` — ran the program with Python 3.
- Git — checked, staged, committed, and pushed the Mission 4 files.

## My understanding

A compiler usually translates a whole program before it runs and often creates machine code or an executable. An interpreter runs code by translating instructions as the program runs, which can make it easier to try changes. Some language implementations combine both approaches: for example, CPython compiles Python source to bytecode and then runs that bytecode in its virtual machine. Both approaches help a computer run instructions written by people.

## Difficulties faced

No significant difficulties.

## How I resolved them

I ran the program with Python 3 and checked that its output matched the required message.

## Evidence/files

- [hello.py](./hello.py) — the one-line Python program.
- This README — comparison and learning notes.

## Commit details

- Commit message: `Compare compilers and interpreters`
- Branch: `main`
- The Mission 4 files and root README update are committed together.