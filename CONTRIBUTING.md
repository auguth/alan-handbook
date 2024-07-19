# Contributing to Alan Handbook - Guidelines

There are three areas where you can contribute:

1. Specifications
2. Non-Specification Areas (Spell/Syntax/etc.)

## For Specification Contributors:

### 1. Create Abstract Introduction, and Mathematical Models
- Develop introductory sections, and mathematical models that outline the program logic.

### 2. Begin Program Logic
- Begin with an abstract mathematical model.
- Define individual function operations:
  - Each function shall only possess a single required operation.
  - Use PascalCase or UpperCamelCase for function names.
  - Construct a radix tree of cohesive, and loosely coupled functions.
  - Avoid nesting functions with logic; use cross calls instead.

### 3. Write Function Skeletons in LaTeX
- Follow the formatting guidelines from the book's backmatter.
- For each function:
  - Start with examples section in binary format, and testing sections in hexadecimal format which includes empty or zero value test cases.
  - Write pseudocode for the function starting from the bottom of the radix trie.
  - Maintain high cohesion with loose coupling:
    - Use vectors for runtime-created sequences with unknown length.
    - Prefer arrays for compile-time created sequences with known length.
  - Use tilde (~) to denote variables subject to garbage collection.
  - Describe function's variants in description if any for different input and output data types.
  - Inputs and outputs shall require data types available in Index of Data Types Section.
  - Match types of variables for consistency, and maintainability in algorithms instead of hard-coding types.
  - Use `true` or `false` for boolean types.

### 4. Comments on Algorithms
- Textual comments in algorithms are avoided in the ALAN Specification, unless a comment is required to explain non-deducible variable usage.
- All functions are highly cohesive, hence their descriptions in their respective sections are sufficient.
- If a call is made to another function, specify its section in a comment as a reference.

## For Non-Specification Writers:

- Write improvements in spelling, syntax, and other non-specification areas such as examples.