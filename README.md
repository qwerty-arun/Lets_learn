# 6/6/24
- Visualisation of amplitude modulation and frequency modulation waves on desmos graphing calculator.
- Think and Grow Rich book: Chapter 1. Desire for riches, having a success conscious mind, think broad, having nothing to lose attitude (buring all bridges behind one). DEFINITE DESIRE IS EVERYTHING. 
# 5/6/24
- HW: Create custom keymap for closing the buffer.
- HW: Debug the C program
- Introduction to SSH keys: creating one, linking with github. `ssh-keygen` creates a pair of ssh keys: one private and another public.
- Using SSH keys, it is possible to git push in local system but not with https links.
- Commands and shortcuts learnt today: `spacebargcb` , `g;` takes you to previous change that has been made , `di'` deletes contents within the single quotes , `Shift-d` deletes till end of line, `Shift-insert` is copy pasting , `vnew` for creating buffer, 'Crun' for finding out buffer number, `terminal` to open a new terminal, `Spacebar` opens up a dialogue of what all we can search , `tabnew` creates a buffer.
- Basics about Makefiles.
- Shift for tabs and Ctrl for windows.
- Actual meaning of `return 0` and its significance. `man error` for man pages for error, `man errno` to see values associated with different errors. '0' means you know there is no error. After writing a program, if you anticipate a particular error, then you return a value associated with that error. So that people reading your code understand what is going on.
# 4/6/24
- Makefiles
- C programming workspace setup.
- Bufnr
- Split window in neovim
# 2/6/24
- Neovim tutorial
- Mason command
- Everything which I learn in college, how do you code for every topic? This is a nice way of thinking.
- How to change colorschemes on neovim.
- `e $MYVIMRC` command in nvim.
- Document everything from now on.
- A broad idea about vimwiki, second brain and LaTex in github.
- https://linuxconfig.org/install-npm-on-linux for installing npm on linux
- https://github.com/nvim-lua/kickstart.nvim for nvim kickstart
- https://github.com/nvim-tree/nvim-tree.lua
- installed `curl` in linux
- https://www.nerdfonts.com/ for downloading different fonts
- https://github.com/nvm-sh/nvm?tab=readme-ov-file#install--update-script 
# 5/5/24
- Draw a graph for the sensor caliberation thing.
- Harmonics: compare a filtered square wave with a sine wave in one time period and see how deviation in present.
- Learn C programming from the start for the next 2 months.
- Review on bezier curve. 
# 7/4/24
- A review on the line following robot. What challenges did you face? </br>
- Problems in the circuit diagram. How to make it more optimised? Why was there a voltage issue. </br>
- Replace boards, drivers etc. with resistances to visualize series or parallel connection.</br>
- Why did I even use 2 batteries? One was way more than enough. </br>
- Don't use Arduino UNO as voltge supplier from now on. Make sure components get their own supply from external source. And from that external source, tap the voltage and step it down using voltage divider circuit. This is a better approach. </br>
- Read data sheet of IR sensor module. Note down the operating conditions. </br>
- Write down own code for sensor. Just use Arduino UNO and one sensor, read the sensor data. Vary the voltage supplied by the Arduino UNO using a potentiometer. With corresponding voltages, note the readings of the sensor. Plot a graph. </br>
- Read about optocouplers and how they are used to isolate ciruits. </br>
- Ideal measurements for the robot: 4 x 2 x 1 cm and not more than 25 grams. </br>
# 24/3/24
- A review on Harmonics project</br>
- What's the difference between plugins and app?</br>
- GNU systems.</br>
- How to write academic papers? What font to use? What color? etc.</br>
- Making your own circuit diagram for your project and its importance.</br>
- Don't make local files.Bring everything online.</br>
# 03/03/24
- About ISRO visit. </br>
- Comparing outputs of filters on Audacity and SoX.</br>
- What about cascading filters?</br>
- Neighbouring frequencies, why are they still present in output? Because of filter response and low roll-off rate.</br>
- How I assembled a CPU? How I could identify different components.</br>
- Check out Audacity open source software. Check if they use SoX library.</br>
- Try out Nyquist plot on Audacity.</br>
- What is kerning? Kerning is the spacing between individual letters or characters.</br>
- Some ideas on CNC machines, 3-D printing and so on.</br>
# 28/1/24
- How do you design a CNC machine using OnShape? A simple one which can cut wood, aluminium. What all components should be made of metal and other of which material?</br>
- Research about MPCNC.</br>
- Implement Arduino grbl in arduino microcontroller.</br>
- Use desmos to plot different graphs on the same sheet. Analyse different waveforms.</br>
- Handwriting font generator. yourfonts website.</br>
- Learn about ttf and otf formats.</br>
# 14/01/24
- Learn about applications of op-amp, every possible circuit, understand it deeply.</br>
- Learn basic electronics. Learn how to debug circuit connections. Don't be scared to try! What happens if we remove one component? How to measure accurate voltages in the circuit? How to read data sheets of every components? [Click here](https://www.youtube.com/@LearnElectronicsRepair) to watch videos based on these topics.</br>
- LIBSOX: `play --h`, `play --h | grep <effect_name>`, `play --help` are some commands with which we learn about various effects.</br>
- Create line numbers in the libsox programs to traverse better.</br>
- Every command can be converter into a program. Try that. For example, the effect `remix` can be converted to a program written by you.</br>
- In every libsox program, do a `NULL` pointer checking always before using it. </br>
- Keep in mind the time and space complexity of each and every program, it matters. </br>
- Research about no. of channels in an audio file.</br>
- Learn about spatial audio.</br>
- Try to visualize 3 files on `sonic visualizer` simultaneously and also try to run the waves in real time.</br>
# 10/12/23
- `sox --help` to find out more about libsox.</br>
- [Click here](https://fossies.org/dox/sox-14.4.2/index.html) to view source code of libsox functions. Using this as a reference, you can build your own tool.</br>
- [Click here](https://github.com/dmkrepo/libsox) to view some examples of tools which is built using basic functions.</br>
- Test each function to know about their details like, thier parameters, return value etc.</br>
# 7/12/23
- Introduction to libsox library.
- Dowloading libsox library in linux using the command: `sudo apt-get install -y libsox-dev`, `sudo apt install pkg-config`, `sudo apt-get install sox libsox-fmt-all bc`.</br>
- Creating first sinwave using the command: `sox -V -r 48000 -n -b 16 -c 2 sin1k.wav synth 30 sin 1000 vol 20dB`. We are creating a sine wave of amplitude: 30, frequency: 1000 and volume of 20dB which is stored in the file `sin1k.wav` of sample rate 48000Hz.</br>
- Generally, frequencies below 1kHz is considered as "noise" in noise-cancelling devices like earphones, headphones etc. So why not test our own earphones using multiple waves of different frequencies and find out what is the bandwidth of the earphones.</br>
- There are too many parameters like, frequency, volume, amplitude, bit rate, sample rate, channels etc. What happens if we even change one parameter. How to tabulate this?</br>
# 20/8/23
- A review of my team project on "E-nose (Electronic nose)", its challenges and how to overcome. Suggestions:- Try using ESP-8266 which has inbuilt wifi module for data tranmission. For integrating two or more sensors, you will need to use a multiplexing device. Gaussian data would be better for our data collection. 
- A discussion on configurations of robots. For example, a robot of cylindrical work volume is very useful parking lots to automate the process of parking in a cylindrical building.
- Bee-keeping tutorial.
- An overview on concepts like classes and objects. Object being an instance of a class. Think of 'class' being a cookie cutter which defines shape and size of a cookie, when you make a cookie, it is an object which we can eat which has the properties of the class. But, we can't eat the class(cookie cutter) itself. There class doesn't have physical existence but an object doesn't.
- Learn the following concepts:
  - MACRO v/s Inline
  - Struct and C++ class
  - Abstract class
  - Copy constructor
  - Move semantics
  - Assigning an object to another</br>
# 6/8/23
- Update the current stack prgm such that the topmost element in the stack now points to NULL.
- Downloading clang compiler.
- Debugging core files using lldb.
- How to backtrace? Use: `bt` command.
- Install virtual box with Ubuntu 22 LTS. </br>
# 30/7/23
- Why learning simulation softwares are important? It can help you analyse and design circuits before you actually try to build one in real life. This saves a lot of expenses.
- Try to build a constant current circuit in the simulation software.
- Optimize the stack program in the following way:
  - Imagine you don't know the no. of elements in the stack, how would you traverse and find out the middle element?
  - Without knowing the no. of elements, how would you insert and delete elements in the stack?</br>
# 16/7/23
- Find the middle element of the linked list and print it.
- Insert a node at a particular position.
- Delete a node at a particular position.
- Sorting the linked list.
- Print stack properly.
- Merge two linked lists.
- Forking repos in Github.
- `gd` stands for `go to definition` goes to a function definition, to come back to caller function, press `Ctrl+o`.
- Check out `libsox` library in C which is related to audio processing. Find resources, find the source code for it. Build the source code for it in linux environment.
# 2/7/23
- Debugging the stack program(linked lists).
- It's a bad practice to use global variables. To eliminate this problem, we can declare it in the `main` function and the pass the value(it can be a pointer or a structure) to a function that requires it for a purpose.
- `Ctrl + r` in vim is for reverse searching in the terminal.
- In Escape mode of vim, `Shift + 8` which is `*` jumps to next occurance of the word under which the cursor is. The cursor can be anywhere in the word.
- `%s/<old_word>/<new_word>/gc` inside vim is used to substitute every `old_word` with `new_word` and vim will ask whether to replace each word or not by jumping to the next word.</br>
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




