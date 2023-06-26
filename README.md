# 25/6/23
- Realizing the importance of CAD drawing and its implementation in 3D printing.
- `while(1)` in C will create an infinite loop where 1 denotes "TRUE".
- Killing the program(Ctrl+C) v/s Exiting gracefully using return. By killing the program, you don't erase the values that variables hold, after some time, kernel goes and cleans up memory. This creates a vulnerability(security issue) for a short period of time. When you exit a program gracefully(return 0), the compiler will erase the memory right after exiting.
Assignment :
- Write a program using realloc function.
- Learn about linked lists. What is linked list? What is the most simplest form. Try implementing stack using this.</br>
# 18/6/23
- How is malloc different from calloc? Allocating memory to array of structures using calloc in one go whereas if we use malloc, we need to use a loop.
- How to dereference a double pointer of type structure?
- `cp <file1> <file2>` command copies content of file1(source) to file2 which is the destination.
- What is a packed struct?
- `ulimit -a` is a command used to print details of cpu and memory allocation to all programs which we write.
Assignment : 
- Write a program which uses the realloc() function.
- Write a program on Stack. Use heap memory allocation, do operations on stack like `push,pop,top` with proper testing conditions.</br>

# 4/6/23
- Concept of Variable Shadowing and how does a compiler know which variables to use? The compiler goes from innermost to the outermost(from innermost braces, say,a `for` loop or an `if` statement, then the compiler checks the entire function for the local variables, then it checks for global variables).
- How do you restrict a user from changing a value of a variable. By using 'const', you are making the variable a "read only" object, that is, you can just use the value stored but cannot manipulate it. Suppose you are building an open source API, these constant variables are very important so that other users don't change the value stored in them.
- `struct student *ptr` ,how do you read this? What does it mean? It means `ptr` is a pointer to student type struct. `int *p` means `p` is a pointer to an integer. When you come across pointers and its initialisation and you are not sure what it means, always read from right to left, it will make more sense than reading from left to right. For example, `int const *p` , here `p` is a pointer to a constant of type 'int'. `const int *p` means 'p' is a pointer to an integer which is a constant. Both are same thing. 
- `int const **p` means p is a pointer to a pointer which is a constant of type int. Now, try `const int **p`.
# 28/5/23 & 29/5/23
- reading man pages for each and every function(in-built) in C. For example, man strcmp.
- structures and concept of "Stack Canary Operation".
- Security Vulnerability: Unless we reset the values in stack, it retains the values even after pop operation.
- What are tracefiles? 
- What are core files? How do you backtrace core files? 
- What is Stack smashing? It's a defence mechanism against buffer overflows.


# 21/5/23
## Pointers
- Brief introduction to pointers.
- Advantages and Disadvantages of pointers.
- Security issues.
- Passing pointers to functions. 

# 30/4/23
## Discussion on topics like:- 
- How to build an emulator for old microcontrollers using C programming?
- Can one build a compiler for a programming language in the programming language for which he is building the compiler for? For example, building a compiler for C programs in C programming language. YES, but it is extremely difficult.
- While building an application or website, you need to use multiple programming languages. How do they run simultaneously? How do they work? How do they communicate with themselves?
- A simple introduction to SWIFT programming language. What compiler does it use and so on.


# 12/3/23
## When you are building a product, ask yourself these questions:-
1) Who are you selling this product to and what are their expectations? If you don't know, you are the one who is supposed to ask them.
2) Does this project make any sense and will it be of any use?
3) Do I have the datasheets of all the components which we are using in this project?
4) How much do I have to invest for building one such product?(it should be as minimal as possible). </br>
5) How much information is fine to be known to customers?
- Scope of a function (public, private).
- Advantages of using a private function. </br>
# 5/3/23
- A brief introduction to Time complexity, Space Complexity and Big-O-Notation.</br>
 Time complexity: Total amount of time take to run an algorithm as a function of length of the input. It represents the number of times a statement is executed. However, time complexity of an algorithm is NOT the actual time required to a execute a particular code, since that depends on other factors like programming language, operating software, disc usage, specialised hardware(Graphic card etc.) . </br>

![](https://adrianmejia.com/images/time-complexity-examples.png)

 Space complexity: Total amount of memory space needed to store the algorithm, run it and complete the task. It included a fixed part and a variable part. Fixed part:- Includes space for the code given, space for variables used, fixed size component variables, space for some other variables if needed etc. Variable part:- Includes the space needed by component variable whose size depends on a particular problem and the space required for other procedures like methods, recursion, object etc.

- Initialising all variables in your code is very important because when you don't, they will posses garbage values and compiler will assume something else.

# 19/2/23
- [Click here](https://graphics.stanford.edu/~seander/bithacks.html) to solve challenging programs in C.
- Try writing all sorting programs like Bubble Sort, Quick Sort etc.
- Learn more about Memory Management and Storage Classes.
- A Brief Introduction on how to Debug a program in Ubuntu(Linux) using `gdb`. 
- `gdb` is a very powerful, very vast but not so user friendly tool. 
- command `gdb <binaryfile>` will debug the binary file. 
- There are two modes of execution:- </br>1)Debug mode where additional information required for debugging is added by including `-g` in the command.`gcc -g main.c`.</br> 2) Release mode is just normal execution and the binary file doesn't contain any additional information about debugging.`gcc main.c`.  
- type `ls -lrth` after each mode of execution and see the difference in sizes of two binary files created. 
- Certain commands in gdb:- `run` to run the program, `break` or `b` are used to add a breakpoint, `quit` to exit gdb, `layout` to view program in different layout. For example: `layout src` will display the source code, `layout asm` will display assembly code, `layout regs` to display different registers used. 
- Shortcuts in gdb and their meaning: 'n' for next-> Goes to the next instruction in the program, 'r' for restart-> Runs the program the beginning, 'p' for printing value that a variable has stored-> 'p sum' will print the value of sum.  
- `layout regs` will not display registers used if you are working on a Linux distribution like ubuntu in Windows environment. Only in a perfect linux environment, it works.
- See types of registers used in loops like 'for' and also recursion. Also see assembly code.

# 05/2/23
- The problem with global declaration of variables.
-  ```# include <stdio.h>``` and ```# include "pascals_triangle.h"```. What's the difference? Well ```<>``` are used for system header files. For example:- ```stdio.h```. By using ```<>``` you are telling the compiler to go look for a header file in the current directory you are working in. ```""``` are used for user-defined header files.
- Introduction to storage classes. Difference between stack and heap.
- Introduction to MATLAB.

# 29/1/23
- Testing a program and finding a point where the program fails. Display proper message when input is wrong and terminating the execution. 
- Makefile Tutorial and some of its syntaxes.
- Changing a.out file name to something else. A source code can have multiple executable binary files and they are all the same.
- Breaking a program into seperate files(called modules) each containing a function of the original combined program.
- How to compile these so called 'modules'. Example:- `gcc main.c bin.c` will combine both these files and then it will execute the entire program. 

# 22/1/23
- Definition of fibonacci series.
- Importance of giving functions and variables proper names in C.
- time command in linux.
- hashmap and hashtables
- Write a program in C to find nth term of fibonacci series using i) functions ii) for loop iii) hashmap
- vim plugins for auto-indentation and text color 
- Pascal's triangle
- makefiles




