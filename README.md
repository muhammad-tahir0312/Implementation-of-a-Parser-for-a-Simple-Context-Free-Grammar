# Project: Simple Arithmetic Expression Parser

## Overview
This project implements a parser for a simple context-free grammar (CFG) that describes arithmetic expressions involving addition and multiplication, with support for parentheses for grouping.

## Grammar
The grammar rules are as follows:
- E → E + T | T
- T → T * F | F
- F → (E) | a

## Functionality
The parser reads an input string and checks if it conforms to the grammar rules defined above. If the input string is valid according to the grammar, it prints confirmation; otherwise, it indicates that the input structure is incorrect.

## Implementation Details
The implementation is done in Python using a hand-written recursive descent parser. Key components include:
- **E_func**: Handles expressions with addition (`+`) operations.
- **T_func**: Manages expressions with multiplication (`*`) operations.
- **F_func**: Deals with atomic expressions, including variables (`a`) and nested expressions within parentheses.

## Example Usage
### Valid Input
Input:
    (a + a) * a
Output:
  The Input Entered by The User is Valid!


### Invalid Input
Input:
    a * a *
Output:
  The Input Entered by The User is Invalid!


## Submission Instructions
- This parser was developed as part of a project and is capable of handling various arithmetic expressions as per the specified grammar.
- The parser can be further extended to include error handling or additional arithmetic operations if needed.

---

This project was developed to demonstrate parsing techniques for context-free grammars in computational theory applications.
