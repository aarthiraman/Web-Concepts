# JS Core Concepts

### Syntax Parser 
 A program that would read your code and validate if the syntax is alright

### Lexical Environment
Refers to the environment or a location where the code would sit and 
what it woould have access to.

### Execution Context
It again refers to a wrapper that holds your code and other data that it 
would have access to from the outer environment

1. An execution context gets created when your code starts to execute.
2. It creates a global object /  window object and the window object is referenced to this keyword
3. It has 2 phases - Creation phase and an execution phase

#### Creation Phase :
 - At the time of the creation phase, it sets up the global object and this
 - Setups memory spaces for variables and functions
 - A scope chain is created for each function or variable to understand 
what data and methods the code has access to

#### Execution Phase
 -  Code is executed line by line
 - When execution happens for each variable / function the engine would look for references 
 - The references are searched based on the scope chain from the innermost code 
    block in which the code is placed till it reaches the global context
