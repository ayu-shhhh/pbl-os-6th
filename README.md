# Nand2Tetris: From NAND Gates to Tetris

This repository contains my solutions for the projects from the book **"The Elements of Computing Systems"** by Noam Nisan and Shimon Schocken, also known as the Nand2Tetris course. This project walks through the construction of a modern computer, from the most basic logic gates to a fully-fledged operating system and a high-level programming language.

## About The Project

The Nand2Tetris project is a comprehensive journey into the world of computer architecture and software engineering. It's broken down into 12 projects, each building upon the last. The goal is to build a complete, general-purpose computer system capable of running a game (like Tetris), created entirely from scratch.

This repository serves as a portfolio of my work, demonstrating my understanding of:
* Boolean logic and digital circuit design (HDL).
* Computer architecture, including CPU and memory design.
* Machine language and assembly programming.
* Virtual machine architecture and implementation.
* Compiler construction for a high-level, object-oriented language.
* Operating system design and development.

## Project Structure

The repository is organized into directories, one for each project. Each directory contains the necessary source files (`.hdl`, `.asm`, `.jack`, etc.) I wrote to complete the assignment.

* **/projects/01: Boolean Logic**
    * Implementation of elementary logic gates (Not, And, Or, Xor) and multiplexers/demultiplexers from NAND gates.

* **/projects/02: Boolean Arithmetic**
    * Building an Arithmetic Logic Unit (ALU) capable of performing addition, subtraction, and logical operations.

* **/projects/03: Memory**
    * Constructing sequential logic circuits: flip-flops, registers, and a Random Access Memory (RAM) unit.

* **/projects/04: Machine Language**
    * Writing low-level programs in the Hack machine language.

* **/projects/05: Computer Architecture**
    * Integrating the CPU, Memory, and I/O to form the complete "Hack" computer hardware platform.

* **/projects/06: Assembler**
    * Building an assembler that translates programs written in Hack assembly language into Hack machine code.
    * *My assembler was written in Java.*

* **/projects/07: VM Translator - Stack Arithmetic**
    * The first stage of the VM translator, handling stack arithmetic and memory access commands.

* **/projects/08: VM Translator - Program Control**
    * The second stage of the VM translator, implementing branching and function call commands.

* **/projects/tbd: High-Level Language**
    * Writing a simple program in "Jack," the high-level language used in the course.

* **/projects/10: Compiler - Syntax Analysis**
    * Building a syntax analyzer (tokenizer and parser) for the Jack language.

* **/projects/11: Compiler - Code Generation**
    * Completing the compiler by adding code generation, which outputs VM code from the parsed Jack source.

* **/projects/12: Operating System**
    * Implementing a small, library-based operating system that includes mathematical functions, memory management, and I/O handling.

## Tools & Technologies

* **Hardware Description Language (HDL):** Used for all hardware construction in Projects 1-3 & 5.
* **Hack Assembly & Machine Language:** The low-level languages for the Hack computer.
* **Jack:** The high-level, object-oriented language for which the compiler and OS are built.
* **Java:** Used to implement the Assembler, VM Translator, and Compiler.
* **Nand2Tetris Software Suite:** The provided suite of tools (Hardware Simulator, CPU Emulator, VM Emulator, etc.) used for testing and development.

## Getting Started

To test and run the projects in this repository, you will need the official Nand2Tetris Software Suite.

### Prerequisites

1.  Download the **Nand2Tetris Software Suite** from the official website: [www.nand2tetris.org](https://www.nand2tetris.org/software)
2.  Clone this repository:
    ```sh
    git clone https://github.com/ayu-shhhh/pbl-os-6th
    ```

### Usage Examples

1.  **To test a hardware chip (e.g., `And.hdl`):**
    * Open the `HardwareSimulator`.
    * Click `File > Load Chip` and navigate to `/projects/01/And.hdl`.
    * Click `File > Load Script` and select the provided `And.tst` to run the test.

2.  **To run an assembled program (e.g., `Pong.hack`):**
    * Open the `CPU Emulator`.
    * Click `File > Load Program` and navigate to the `.hack` file you want to run (e.g., from `/projects/04/`).

3.  **To run a compiled Jack application:**
    * Open the `VM Emulator`.
    * Click `File > Load Program` and load the **directory** containing the compiled `.vm` files (e.g., the `Pong` directory from the course materials, after compiling it with my compiler).

## Acknowledgements

* **Noam Nisan and Shimon Schocken** for creating this incredible course and book.
* The entire **Nand2Tetris community** for providing a platform for learning and discussion.
