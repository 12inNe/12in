# Book Review

This blog I am going to review and introduced the book that I have read and tried to  learned about C language.

The book is **Advanced Turbo C Programming (1988)** which is really old book and I have some checklist for the book which is for learning C programming and use for comparing which the topic this book which don't and which that this book have but I don't.

 [Clik here if you want to read Advanced Turbo C Programming (1988) ](https://www.sciencedirect.com/book/9780127426891/advanced-turbo-c-programming)
# Table of contents


  - [Topics to learn C](#topics-to-learn-c)
  - [What Advanced Turbo C Programming (1988) Does Not Have.](#what-advanced-turbo-c-programming-1988-does-not-have)
  - [The Topic that This Book Have](#the-topic-that-this-book-have)
  - [Topic I want to put in the checklist after rerading the book.](#topic-i-want-to-put-in-the-checklist-after-rerading-the-book)
  - [Conclusion](#conclusion)

## Topics to learn C
- **Getting started with C Language**
  - ***The history of C.***
  - ***The evolution of the C programming standards.***
  - The relationship of C to C++.
  - ***Some recommended / free books for learning C.***
  - Source Code Compilation, Cross-Compilation Process.
  - ***C/C++ Toolchains and Open Source IDEs.***

- **Code Comments**
  - ***Single-line comments: // ....***
  - ***Multple-line comments: /* ... */***
  
- *Keywords or reseverd words in C (Not in the book)*
  
- **Data Types**
  - Basic data types
    - ***'int' represents integers (whole numbers) with varying sizes depending on the platform.***
    - ***'char' represents single characters.***
    - ***'float' represents single-precision floating-point numbers.***
    - ***'double' represents double-precision floating-point numbers.***
    - 'bool' (via #include <stdbool.h>) represents boolean values ('true' or 'false').
    - '_Bool' (C99's boolean type)
  - ***Derived Data Types***
    - Arrays, structures, unions
  - ***Enumerated data types (the 'enum' keyword)***
  - ***'void' data type***
    - a special data type that indicates the absence of a specific type.
    - used to represent a lack of value or to indicate that a function does not return any value.
- *Type Modifiers for Numbers(Not in the book)*
  - integers: such as 'signed', 'unsigned', 'short', 'long', 'long long'
  - floating-points: 'long' (for 'float' and 'double')
- **Type Conversions**
  - ***Implicit: short to int to long, float to double.***
  - ***Explicit: (<type>)(expression) for type-casting.***
- **Literals (constant values of specific data types)**
  - Primitive vs. Compound Literals
  - ***Integer Literal: 42, -100, 0, 123456***
  - ***Octal Literal: 0644***
  - ***Hexadecimal Literal: 0x1A, 0xFF, 0xABC***
  - ***Floating-Point Literal: 3.14, -0.005, 1.0e-5***
  - ***Character Literal: 'A', '5', '!', '\n'***
  - Boolean Literal (C99 and later): true, false
  - ***String Literal: "Hello, world!", "" (an empty string)***
- **Identifiers and Variables**
  - Identifier Naming
  - ***Variable Definition and Initialization***
  - ***Variable Scope***
  - ***Constants (with the const keyword)***
  - Declaration vs. Definition
    - A declaration introduces an identifier to the compiler and informs it about the data type and name of the identifier.
    - A definition creates the actual instance of an identifier in memory. It allocates memory for variables and provides the implementation for functions.
- **Operators**
  - ***Arithmetic Operators: +, -, *, /, %, ++, --***
  - ***Relational Operators: ==, !=, >, <, >=, <=***
  - ***Logical Operators: &&, ||, !***
  - ***Bitwise Operators: &, |, ^, ~, <<, >>***
  - ***Assignment Operators: =, +=, -=, *=, /=, %=, &=, =, ^=, >>=, <<=***
  - ***Conditional Operator: () ? () : ()***
  - ***Miscellaneous Operators:***
    - , (comma), & (address-of operator)
    - sizeof(...) used to determine the size in bytes of a data type or variable.
    - . (dot or memory-access operator)
    - -> (memory-access operator),
    - [...] (square bracket or array indexing operator)
  - ***Side Effects of the ++ and -- Operators for Value Modification***
    - Pre-increment and Pre-decrement
    - Post-increment and Post-decrement
    - Order of Evaluation
  - ***Short-circuit logical operators***
    - The && (logical AND) operator: (expr1 && expr2)
    - The || (logical OR) operator: (expr1 || expr2)
    - These short-circuit operators halt evaluation once the final outcome is determined by the preceding sub-expressions.

- **Strings**
  - ***A string is a sequence of characters stored in an array that represents text.**
  - ***terminated by a null character ('\0').***
  - ***accessible by a (char *) pointer.***
- **Array: 1D and 2D**
  - ***a collection of elements of the same data type, stored in contiguous memory locations.***
- **Structs (short for structures)**
  - ***a composite data type that allows you to group together variables of different data types under a single name.***
- **Union**
  - ***a user-defined data type that all members of a union share the same memory location.***
- **Bit-field**
  - ***a bit field is used to specify the number of bits to be used to store a particular data member within a struct.***
- **Enumeration (enum)**
  - ***a user-defined data type that consists of a set of named integer constants.***
- **Typedef for user-defined types**
  - ***used to create an alias or a new name for an existing data type.***
  - ***provides a way to define custom names for data types.***
- **Statements such as**
  - ***Iteration Statements/Loops: for, while, do-while***
  - ***Selection Statements: if, if-else, switch-case***
  - ***Assignment Statements***
- **Functions**
  - ***Variable arguments of a function***
- **Pointers**
  - ***Pointer Arithmetics***
  - ***Function Pointers and Parameters***
- **C Preprocessor Directives and Macros**
  - ***#include <...>: include header files.***
  - ***#define***
  - ***#if, #else, #ifdef, #ifndef, #endif, #undef***
  - ***#error***
- **Command-line arguments to the main() function**
  - ***provided by the user when they run the program and can be used to pass information or parameters to the program.***
  - ***int main(int argc, char *argv[]) { ... }***
- **The C Standard I/O library**
  - ***printf() and scanf() functions.***
  - ***fprintf() functions and the output streams ('stdout' and 'stderr').***
  - ***Formatted strings for Input/Output***
- **Files and I/O streams**
  - ***<stdio.h> (Standard I/O Library) provides functions for basic input and output operations.***
  - ***Examples of functions in this library:***
    - fopen(), fclose()
    - fprintf(), fscanf()
    - fputc(), fgetc(), fgets(), fputs()
    - fwrite(), fread(), feof(), fseek(), rewind()
  - ***Other standard C libraries:***
    - <stdlib.h> provides functions for various file operations.
    - <unistd.h> (Unix Standard Library) provides functions for low-level file operations.
    - <sys/types.h> and <sys/stat.h> provide data types and functions for working with file status and attributes.
    - <fcntl.h> provides functions for managing file descriptors and controlling file attributes.
- *Pseudo-Random Number Generation(Not inthe book)*
  - srand(): used to seed the random number generator.
  - rand(): returns an integer between 0 and RAND_MAX.
  - Both functions are declared in <stdlib.h>
- *The C Standard Math library(not in the book)*
  - The <math.h> header file must be included in source code in order to use the C Standard Math library.
  - The -lm flag must be specified for program linking (when using GCC C compiler).
- *POSIX Threads and Multithreading(Not in the book)*
  - often referred to as pthreads.
  - a standardized threading library for creating and managing threads in a multi-threaded program.
  - used to create multiple threads within a single process, enabling concurrent execution of tasks.

- **Interprocess Communication (IPC)**
  - provides the mechanisms and techniques used for communication and data sharing
  between different threads or processes.
  - common IPC mechanisms:
    - ***Pipes and Named Pipes (FIFOs)***
    - Sockets
    - Signals
    - Message Queues
    - Semaphores, Mutexes, and Condition Variables
    - Shared Memory
    - Message Passing
- *Assertion(Not in the book)*
  - used to ensure that certain conditions hold true during program execution.
  - The assert() macro can be used to perform assertions, defined in the <assert.h> header file.
- **Memory management (Heap Usage)**
  - ***Memory management in C involves allocating and deallocating memory on the heap.***
  - ***Heap is a region of memory used for dynamically allocated data.***
  - ***Primary functions for memory management on the heap:***
    - malloc() used to allocate a block of memory on the heap.
    - calloc() used to allocate memory for an array of elements, initializing them to zero.
    - realloc() used to resize an existing allocated memory block.
    - free() used to release memory that was previously allocated.
- **Common C programming idioms and developer practices**
  - Use Meaningful Variable and Function Names.
  - Use consistent indentation and formatting.
  - Write Code with Comments and Documentation.
  - Avoid Global Variables.
  - Minimize the use of global variables.
  - Properly allocate and release memory.
  - Use Constants and Enumerations for improved code readability.
  - Avoid using hard-coded values directly in the code. Instead, use named constants or macros.
  - Break large functions into smaller, more manageable functions to improve readability.
  - Write code that is portable across different platforms and compilers.
  - ...
- **Common Pitfalls**
  - Memory Leakage
  - Buffer Overflows
  - Integer Overflow and Underflow
  - Null Pointer Dereference
  - Improper Type Conversion and Casting
  - Use of Uninitialized Variables
  - ...
- **GUI-based Application Development (with C/C++)**
  - GTK3 or GTK4 framework (for Linux)
  - Qt5 framework (Cross-platform)
  
## What Advanced Turbo C Programming (1988) Does Not Have.
  As you can see from the there are many of basic stuff that you need to learned if you new to c language but this book doesn't have a lot of them its also state that ***"This book assumes that you're familiar with the basics of C programming. It does not explain C programming fundamentals at the level you'll need if you're a new hand at C programming."*** So if you new or just started learning C ,I'm not recommend this book for you.

## The Topic that This Book Have

**Getting started with C Language**

  In this book its have some of brief history of C and none of C++ cause of the year it was publish and also how new the language is. Also this book show the change of C standards and book about it which is classic text of Kernighan and Ritchie called "The C Programming Language".

**Code Comments**

  In this part it doesn't hve it but there are example of using them in the book on many parts

  **Data Types**

  About the data types it have showned on Chapter 3 about Data Structure which contain of 'int','char','float,'double' but none boolean type. Also it showned how to use many structure like arrays enumerated union and void type was include too.

  **Type Conversions**

  Showned some usage but doesn't explain how to use.
  
  **Literals (constant values of specific data types)**

  Used and explain about how to use the data but doesnt have compairation and does't have boolean.

  **Identifiers and Variables**

  Its have showned about how to defined waht type and constant and volatile usage in the book but doesn't have compairison of declare and define also none of topic of how to naming varible.

  **Operators**

  On this book it use all of the operators but doesn't have explaination and how to use them.

  **Strings**

  A lot of info about this part using string is like the main concept of the book the using of pointer and NULL all included.
  
  **Array: 1D and 2D**

  Its using Array in many kind like for some datta structured and to store value have showned how to use it on the first Chapter.
  
  **Structs (short for structures)**
  
  On chapter 3 it showned many of data structure like Linkedlist(singly and doubly),Stack,Binary tree and how to make it useful.

  **Union**
  
  Its showned how to create and usage of Union

  **Bit-field**

  Have showned some uses in the book.

  **Enumeration (enum)**
 
  Included on the First Chapter on how to stuct enum.

  **Typedef for user-defined types**

  Explained how to usage typedef and how we can redefine variable.
  
  **Statements such as**

  Have all of statement we're normally use such as for,while,switch case, if-else and a lot of usage.
  
  **Functions**

  Shows how to declare how the argument work and type of it , void function and how to used them.
  
  **Pointers**
  
  How to use them and many way to make them useful. It like the fundamental part of learning C.

  **C Preprocessor Directives and Macros**

  This book have the table for all Macros and Preprocesser which also explained how them work and when to use.
  

  **Command-line arguments to the main() function**

  Show about argv argc and how to used command-line for running the program.

  **The C Standard I/O library**

  Contains all of standard I/O function and explain the library used.
  
  **Files and I/O streams**

  All about Files and I/O streams are included in this book which i think it realy usedful if your gonna work with this part of programmig and also uit have the routine for practice yourself too.



  **Interprocess Communication (IPC)**

  Only pipes introduce in this book.


  **Memory management (Heap Usage)**

  Heap is use in this book and the function for memory allocate the too and there function too like 'malloc()','colloc()', 'realloc", 'free()'

  **Common C programming idioms and developer practices**

  In the book it says you have 2 main concepts of writing code ther are to be reable and portable. And it show how the code properly writing to be reable.
  
  **Common Pitfalls**

  Not really state on one topic but seperatly talk about when we in the topic and some of how to hadling with them.
  
 **GUI-based Application Development (with C/C++)**
  
  In this book the last 2 Chapters are about Video and creating UI which easily for user to use.

## Topic I want to put in the checklist after rerading the book.

After finished the book I know that this book have special pointer which I thing I would like to add them beacuse of pointer in uniqe for C programming. Next thing is the routine of programming which it state how you should write and work with them if you want to mastered and a topic about Console I/O and low-level I/O.And the last one is about graphic coding and functing of them.

## Conclusion

In conclusion this book is not bad but it out of date some of the feauture it state are popular on this day. And the styles of the book is boring a lot of plain text and code but the content of it isn't bad like the data structure , I/O and UI part is really nice to read if you want to use it. So over all I would say if you wanna learned and tried these topic the book is great for you.
