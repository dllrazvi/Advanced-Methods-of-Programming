# Toy Language Interpreter
This project is a custom interpreter for a "toy" programming language, built using Java and a JavaFX graphical interface. It simulates the inner workings of programming languages, combining both backend logic (parsing and execution) and a simple graphical user interface.

## Core Concepts & Architecture
- Layered architecture with clear separation of concerns

- Model-View-Controller (MVC) pattern for GUI interaction

- Encapsulation, interfaces, and Java streams

- JavaFX for a user-friendly graphical interface

- Multi-threading with forking for parallel program states

## Language Features
### Supported Instructions:
- Arithmetic, relational, and logical expressions

- Variable declaration and assignment

- Conditional execution (if), loops (while)

- File handling (open, read, close)

- Dynamic memory management (heap allocation, read, write)

- Forking (multi-threaded execution with new program states)

- Printing output to a shared output table

## Variable Types:
Int, Bool, String, Reference

## Internal Mechanics
- Programs are interpreted step-by-step using an execution stack

- Symbol tables manage local variables per program state

- File table stores file descriptors (BufferedReader) for file I/O

- A shared heap allows reference manipulation and garbage collection

- Output list stores print outputs visible in the GUI

- Program states are uniquely identified, each with its own stack and symbol table

- Forking creates a new program state with its own execution stack, but shared heap and file table

## GUI Features (JavaFX)
- List and select available programs

- Visualize program state step by step

- See live updates of execution stack, symbol table, heap, file table, and output

- Support for running programs in parallel (forking)
