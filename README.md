# SumForge

**A modular arithmetic utility written in C.**

SumForge is a lightweight C project that demonstrates integer addition through a modular program structure. It separates application logic, function declarations, and the entry point into individual files, making the code easier to understand, maintain, and extend.

## Overview

The project implements an addition function that accepts two integers and returns their sum. It also validates user input and includes assertion-based tests for verifying the function's behavior.

## Features

- **Modular architecture** — separates declarations, implementation, and application entry point.
- **Input validation** — checks whether both inputs are valid integers.
- **Reusable function** — implements addition as an independent function.
- **Assertion-based testing** — verifies expected results for different integer inputs.
- **Standard C libraries** — uses standard input/output and process exit-status facilities.

## Tech Stack

- **Language:** C
- **Standard Library:** `stdio.h`, `stdlib.h`, `assert.h`
- **Testing:** C assertions
- **Compiler:** GCC or Clang
- **Version Control:** Git and GitHub

## Project Structure

```text
sumforge/
├── Header/
│   └── Header.h
├── src/
│   ├── MainFunction.c
│   └── EntrypointFunction.c
├── Test/
│   └── AssertFunction.c
└── README.md
```

### File Responsibilities

| File | Responsibility |
|---|---|
| `Header/Header.h` | Declares the addition function and includes standard headers. |
| `src/MainFunction.c` | Handles user input, validation, and output. |
| `src/EntrypointFunction.c` | Implements the addition logic. |
| `Test/AssertFunction.c` | Tests addition results using assertions. |

## Getting Started

### Prerequisites

Install a C compiler, such as GCC or Clang, and ensure it is available from your terminal.



### Build

Compile the application from the repository root:

```bash
gcc -Wall -Wextra -std=c11 -IHeader \
    src/MainFunction.c \
    src/EntrypointFunction.c \
    -o myexe
```

### Run

On macOS or Linux:

```bash
./myexe
```

On Windows, run the generated executable using the appropriate command for your terminal.

## Usage

Enter two integers when prompted.

Example:

```text
Enter First Number :
10
Enter Second Number :
20
Addition is : 30
```

If an input is not a valid integer, the application reports an error and exits unsuccessfully.

## Testing

The project includes assertion-based tests to verify the addition function.

Compile the test program separately from the application entry point:

```bash
gcc -Wall -Wextra -std=c11 -IHeader \
    Test/AssertFunction.c \
    src/EntrypointFunction.c \
    -o myexe
```

Run the tests:

```bash
./myexe
```

**Note:** Ensure that every assertion contains the correct expected result. For example, `Addition(10, 11)` should equal `21`, not `22`.

## Learning Objectives

- Understand function declarations and definitions in C.
- Practice separating source files and header files.
- Implement basic input validation.
- Compile multi-file C applications.
- Write and execute assertion-based tests.
- Apply foundational software development practices.


## Author

**Vishakha Vinod Hiwrale**

GitHub: [Vishakhaa02](https://github.com/Vishakhaa02)


