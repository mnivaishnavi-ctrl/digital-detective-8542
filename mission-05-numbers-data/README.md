# Mission 5 — Numbers and Data

## Task 5.1 — Convert numbers by hand

### Decimal 13 to binary

13 ÷ 2 = 6 remainder 1  
6 ÷ 2 = 3 remainder 0  
3 ÷ 2 = 1 remainder 1  
1 ÷ 2 = 0 remainder 1  
Reading the remainders from bottom to top: **1101₂**

### Decimal 25 to binary

25 ÷ 2 = 12 remainder 1  
12 ÷ 2 = 6 remainder 0  
6 ÷ 2 = 3 remainder 0  
3 ÷ 2 = 1 remainder 1  
1 ÷ 2 = 0 remainder 1  
Reading the remainders from bottom to top: **11001₂**

### Binary 1010 to decimal

1 × 2³ + 0 × 2² + 1 × 2¹ + 0 × 2⁰  
= 8 + 0 + 2 + 0  
= **10₁₀**

### Binary 1101 to decimal

1 × 2³ + 1 × 2² + 0 × 2¹ + 1 × 2⁰  
= 8 + 4 + 0 + 1  
= **13₁₀**

### Hexadecimal A to decimal

A₁₆ = 10₁₀

### Hexadecimal 1F to decimal

1 × 16¹ + 15 × 16⁰  
= 16 + 15  
= **31₁₀**

### Binary 1111 to hexadecimal

1111₂ = 8 + 4 + 2 + 1 = 15₁₀  
15₁₀ = **F₁₆**


## Task 5.2 — Verify using Python

| Python expression | Result | Matches Task 5.1? |
|---|---|---|
| `bin(13)` | `0b1101` | Yes, 1101₂ |
| `bin(25)` | `0b11001` | Yes, 11001₂ |
| `int("1010", 2)` | `10` | Yes, 10₁₀ |
| `int("1101", 2)` | `13` | Yes, 13₁₀ |
| `hex(15)` | `0xf` | Yes, F₁₆ |
| `int("A", 16)` | `10` | Yes, 10₁₀ |
| `int("1F", 16)` | `31` | Yes, 31₁₀ |


## Task 5.3 — Number converter

| Input | Binary output | Hexadecimal output |
|---|---|---|
| 5 | `0b101` | `0x5` |
| 13 | `0b1101` | `0xd` |
| 15 | `0b1111` | `0xf` |

`input()` gets the number, `int()` makes it an integer, and `bin()` and `hex()` convert it.


## Task 5.4 - How is text stored ?

- Uppercase A = 65
Lowercase a = 97

- A computer needs an encoding standard to represent characters in the form of numbers so that it can store and process text. It also ensures that text is displayed correctly across different devices and systems.

- The Euro symbol (€) or an emoji (😊).