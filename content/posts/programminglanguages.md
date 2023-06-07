---
title: "Programming Languages"
date: 2023-06-05
showToc: true
TocOpen: false
draft: false
searchHidden: false
hidemeta: false
comments: false
disableHLJS: true # to disable highlightjs
disableShare: false
disableHLJS: true
hideSummary: true
ShowReadingTime: true
ShowBreadCrumbs: true
ShowWordCount: true
ShowRssButtonInSectionTermList: false
UseHugoToc: false
ShowPostNavLinks: false
---
A programming language is a system of notation for writing computer programs. 
{{< youtube pEfrdAtAmqk >}}

---

Languages can be viewed through two components.

- Semantics (function) - refers to the meaning behind the code, such as what a particular command or function does.

- Syntax (form) - refers to the rules and structure of a programming language, such as how code is written and formatted.

*Together, semantics and syntax define a language*

---

Additionally, languages can be defined by its specification or a implementation

-  Language specification - a formal description of its syntax and semantics.

-  Language implementation - the actual software that reads programs (compile or interprets) and executes it.

*Specification's are nice because they leave no ambiguity in the language's interpretation and the implementation is what brings the specification to life*


---


## Semantics 

The semantics of a programming language refers to the meaning of its elements - the "what happens" when the code is executed. 


**Data types and Structures**

- Every language has its own set of data types (such as integers, strings, or booleans) and structures (like arrays or objects). 
- What happens when you manipulate these components and how these components react with other components ultimately dictate the language's semantics. 


**Control Flow**

-  This is how the code execution is controlled (including loops, conditional statements, and functions)

- Defines the order of execution, what is executed, how to make decisions, and to handle subroutines

**Error Handling**

-  Defines how the language handles errors 
-  Throwing exceptions, logging errors, or halting execution.

**Memory Management**
-  How memory is used and allocated/deallocated
- Includes variable creation/destruction and garbage collection  

**Concurrency and Parallelism** 
- Depends if language supports it 
- Essentially defines how multiple tasks will be done simultaneously


*Semantics can vary significantly from one language to another.*




---
## Syntax 

Syntax refers to a set of rules that define how programs written in the language **must** be structured. Syntax is made of lexical elements and grammatical structure.
- Lexical elements and grammatical structure are what govern how statements and expressions are **correctly** formed. 


**Lexical Elements:**

 These are the basic components of a language. They include keywords (like `if`, `else`, `for`), identifiers (variable or function names), operators (`+`, `-`, `*`, `/`), literals (like `1`, `"hello"`), and punctuation symbols (`{}`, `()`, `,`).

**Grammatical Structure (Syntax):**

 This defines how the basic components can be combined to form valid statements or expressions in the language. For example, an `if` statement in Python is written as `if condition: statement`, where `condition` is an expression that evaluates to a boolean value and `statement` is the code that gets executed if the condition is true.

*Programming languages, such as C, C++, and Java, have syntax that is based on the C programming language which is very concise syntax. Other programming languages, such as Python, Ruby, and JavaScript, have very readable syntax.*

---

## Important 


**Low-level vs High-level Languages**

Programming languages are classified as low-level or high-level depending on abstraction from the hardware.

- Low-level languages (assembly languages or C) have little abstraction from the computer’s instruction set architecture. They offer high control over the hardware but require a lot knowledge about the computer's architecture and memory model.

- High-level languages (Python or Java) abstract the precise hardware details. They have features like garbage collection and bounds checking that make them easier to use but perhaps less performant for very specific tasks.

**Scripting vs System Languages**

- Scripting languages (Python,JavaScript) are typically used for short and simple tasks. They are **interpreted** rather than compiled, and they have features good for text processing or automating system tasks.

- System languages (C,Rust) are used for writing operating systems and other low-level applications. They give close control over system resources and are **compiled** to machine code 


**Interpreter vs Compiler**

- An Interpreter reads and executes the code **line by line**. If there is an error, it stops at that line and reports it - making it easier to debug. Every time the program is ran, an interpreter has to translate the source code into machine code.  

- A Compiler converts the **entire** source code into machine code before the program is run. If there is an error, it is reported during the compilation step and the program doesn't run until all errors are resolved - making it harder to debug. Once the program is compiled, it can be run multiple times without further translation

- The choice between an interpreted language and a compiled language  doesn't matter as much as it used to.
    - Java compiles into bytecode and then gets interpreted by the Java Virtual Machine (JVM)
    - Just-In-Time (JIT) compilers can compile before execution. 
  
**Static vs Dynamic Typing**

- In statically-typed languages (C++,Java) you must declare a variable's type ahead of time and it can't change

- In dynamically-typed languages (Python,Ruby) you do not have to declare a variable's type and it can be of any type.

- An easy and intuitive example is that in a statically-typed language, if you declare a variable as an integer, you cannot later assign a string to it where as in a dynamically-typed language you can assign any type of value to the variable without having to declare it.


**Type System**

A type system is a collection of rules that assign a property called a "type" to the programming constructs (variables, expressions, functions or modules) a computer program is composed of. A "type" is used to reduce the possibility for bugs in programs by defining the connections between different parts of a computer program, and then checking that they are connected in a consistent way.

- An easy and intuitive example is declaring a variable of type "integer" and assigning it a value of 5. The type system will give a type error because it ensures that the variable can only hold integer values

**Intended Use: System, General, Specific, Script**

- System languages are used for system programming, to develop the core functioning parts of an operating system

- General-purpose languages are used to write software that will be used for a wide variety of applications.

- Specific-purpose languages are for a specific domain, like SQL for databases or HTML for web pages.

- Scripting languages are used for small tasks like text processing or network scripting.



**Standard library and run-time system**
- Every language comes with a set of built-in functions, classes, and modules that form its standard library - providing utilities for tasks
- Runtime system refers to the software/hardware *environment* within which a program runs.

---

{{< youtube qQXXI5QFUfw >}}

