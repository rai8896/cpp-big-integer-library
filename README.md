# C++ Big Integer Library

A custom arbitrary-precision integer implementation in C++ that uses strings to represent and process large integers beyond the limits of built-in integer data types.

## Overview

The project implements an `Integer` class that performs arithmetic and comparison operations on large integer values. It uses digit-by-digit arithmetic algorithms and operator overloading to provide an interface similar to built-in integer types.

## Features

- **Arbitrary-Precision Representation:** Stores integer values as strings to support numbers larger than standard integer types.
- **Arithmetic Operations:** Supports addition (`+`), subtraction (`-`), multiplication (`*`), division (`/`), and modulo (`%`).
- **Comparison Operators:** Implements equality, inequality, and relational comparisons.
- **Compound Assignment:** Supports `+=`, `-=`, `*=`, `/=`, and `%=`.
- **Object-Oriented Design:** Encapsulates integer representation and operations inside a custom C++ class.
- **Interactive CLI:** Accepts arithmetic expressions through a command-line interface.

## Tech Stack

- C++
- Object-Oriented Programming (OOP)
- Operator Overloading
- String Manipulation
- Arithmetic Algorithms

## Getting Started

### Prerequisites

- A C++ compiler supporting C++11 or later
- A terminal or command prompt

### Compilation

Save the source code as `main.cpp` and compile it using:

```bash
g++ -std=c++11 main.cpp -o big_integer
```

### Execution

**Linux / macOS:**

```bash
./big_integer
```

**Windows:**

```bash
big_integer.exe
```

## Usage

Enter an operator followed by two integer values.

Example input:

```text
+ 12345678901234567890 98765432109876543210
* 123456789 987654321
== 12345 12345
end
```

Example output:

```text
111111111011111111100
121932631112635269
true
```

The `end` command terminates the program.

## Supported Operators

| Category | Operators |
|---|---|
| Arithmetic | `+`, `-`, `*`, `/`, `%` |
| Comparison | `==`, `!=`, `<`, `>`, `<=`, `>=` |
| Compound assignment | `+=`, `-=`, `*=`, `/=`, `%=` |

## Learning Objectives

- Understanding operator overloading in C++
- Implementing arithmetic algorithms using strings
- Working with custom numeric representations
- Applying object-oriented programming concepts
- Handling large integer values without relying on fixed-width integer arithmetic

## Future Improvements

- Fix and test edge cases involving negative numbers, zero, and leading zeros
- Add division-by-zero validation
- Make arithmetic operations avoid modifying their input objects unexpectedly
- Add automated unit tests and performance benchmarks
- Optimize multiplication using more efficient algorithms

## License

This project is available under the MIT License. Add a `LICENSE` file before distributing it under this license.