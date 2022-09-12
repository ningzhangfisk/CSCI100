# 3.1 Programming Languages
## 3.1.2 Computer Languages
### 3.1.2.1 Machine Language
+ **Machine language** is a set of instructions executed directly by CPU.
+ **Machine language** is the elemental language of computers, comprising a long sequence binary digital zeros and ones.
+ CPU implements machine language instructions.
+ CPU understands a low level machine language.
+ Each machine language instruction is extremely simple.
  - add 2 numbers
  - compare 2 numbers
  - get input from keyboard
  - display information on screen

![machine language example](https://miro.medium.com/max/1400/1*GYRRMXSnCnEosJX6-8uOAQ.jpeg)

### 3.1.2.2 Assembly(lower-level) Language
+ A processor understands only machine language instructions, which are strings of 1's and 0's.
+ However, machine language is too obscure and complex for using in software development.
+ So, the low-level assembly language is designed for a specific family of processors that represents various instructions in symbolic code and a more understandable form.
+ Advantages of Assembly Language
  - Having an understanding of assembly language makes one aware of 
    + How programs interface with OS, processor, and BIOS;
    + How data is represented in memory and other external devices;
    + How the processor accesses and executes instruction;
    + How instructions access and process data;
    + How a program accesses external devices.
  - Other advantages of using assembly language are 
    + It requires less memory and execution time;
    + It allows hardware-specific complex jobs in an easier way;
    + It is suitable for time-critical jobs;
    + It is most suitable for writing interrupt service routines and other memory resident programs.
+ Assembly code is converted into executable machine code by a utility program referred to as an **assembler**.

![assembly language](https://i.ytimg.com/vi/wA2oMRmbrfo/maxresdefault.jpg)

### 3.1.2.3 High-level Language
+ The term `high-level language` (HLL) refers to the computer programming languages that not only allow the use of symbolic operators to signify operations and of symbolic names to represent data and data structures, but are also structured with syntax and semantics to describe the computing algorithm.
+ A high-level language enables a programmer to write programs that are more or less independent of a particular type of computer. 
+ Such languages are considered high-level because they are closer to human languages and further from machine languages.
+ A high-level programming language is a programming language with strong abstraction from the details of the computer. 
+ In contrast to low-level programming languages, it may use natural language elements, be easier to use, or may automate (or even hide entirely) significant areas of computing systems (e.g. memory management), making the process of developing a program simpler and more understandable than when using a lower-level language.
+ List of some popular higher-level languages:
  - **Python**(we'll learn Python in this class.)
  - Java
  - JavaScript
  - C++
  - C#
  - Ruby
  - Perl
  - PHP
  - GO
  - Rust

![machine vs assembly vs high-level](https://www.cise.ufl.edu/~mssz/CompOrg/Figure2.1-CompLang.gif)

### 3.1.3 Source Code
+ Programmer writes source code of a program in a high-level language, say, Python.
+ The high level language program is called the source code.
+ High level computer languages
  - Sequential code
  ~~~~
  a = 1
  b = 2
  c = a + b
  ~~~~
  - Selection code
  ~~~~
  a = 1
  if a<0:
      print(a, "is negtive.")
  else:
      print(a, "is NOT negtive.")
  ~~~~
  - Iteration code
  ~~~~
  for i in [1,2,3,4]:
      print(i)
  ~~~~
### 3.1.4 Complier and Interpreter
#### 3.1.4.1 Complier
+ **Compiler** translates the source code into a large number of machine code instructions.
+ A compiler is a language processor that translates an **entire** high-level language program into its machine language equivalent before the program is executed.
+ The compiler produces an executable file from the source code (e.g., .exe from C++), and it is finished.
+ Every high-level language requires its own compiler.
+ The high level language program is called the source code.
+ The machine language translation is called the object code.

![complier](http://www.sitesbay.com/cprogramming/images/c-compiling.png)

#### 3.1.4.2 Interpreter
+ Some dynamic languages(e.g., Java, Javascript, Python) can be implemented by an interpreter.
+ In computer science, an interpreter is a computer program that directly executes instructions written in a programming or scripting language, without requiring them previously to have been compiled into a machine language program.
+ Interpreter does not create an object code.
+ Interpreter is a program which runs other code.
+ Interpreter looks at one line at a time, then does that action, in the moment.
+ Then the interpreter proceeds to the next line.
#### 3.1.4.3 Compilers versus interpreters
|Interpreter|Complier|
|----|----|
|Interpreter translates just one statement of the program at a time into machine code.|Compiler scans the entire program and translates the whole of it into machine code at once.|
|An interpreter takes very less time to analyze the source code. However, the overall time to execute the process is much slower.|A compiler takes a lot of time to analyze the source code. However, the overall time taken to execute the process is much faster.|
|An interpreter does not generate an intermediary code. Hence, an interpreter is highly efficient in terms of its memory.|A compiler always generates an intermediary object code. It will need further linking. Hence more memory is needed.|
|Keeps translating the program continuously till the first error is confronted. If any error is spotted, it stops working and hence debugging becomes easy.|A compiler generates the error message only after it scans the complete program and hence debugging is relatively harder while working with a compiler.|
|Interpreters are used by programming languages like Ruby and Python for example.|Compliers are used by programming languages like C and C++ for example.|
#### 3.1.4.4 Current trend
+ Current trend is towards [dynamic languages](https://en.wikipedia.org/wiki/Dynamic_programming_language).
+ It’s attractive to save some programmer time at the expense of some CPU memory use.
+ CPU cheap, programmer relatively rare/ expensive.
