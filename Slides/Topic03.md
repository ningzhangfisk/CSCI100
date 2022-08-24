# CSCI110
# Dr. Ning Zhang
# Topic 3: Progamming Languages and Applications
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
  if a<0
      print(a, "is negtive.")
  else
      print(a, "is NOT negtive.")
  ~~~~
  - Iteration code
  ~~~~
  for i in [1,2,3,4]
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
+ Current trend is towards dynamic languages.
+ It’s attractive to save some programmer time at the expense of some CPU memory use.
+ CPU cheap, programmer relatively rare/ expensive.

# 3.2 Applications

![apps](https://blog.axway.com/wp-content/uploads/2014/05/blog-header-apps.png)

+ An app is a type of software in the computer that allows you to perform specific tasks.
+ Types of Applications

![Types of Applications](https://1.bp.blogspot.com/-Zm4rlx5r6hI/YUuNV998UbI/AAAAAAAACII/mKTeIGwKbGof_lYaD5oiNQ_YF2pJxoTyQCLcBGAsYHQ/s16000/Types%2Bof%2BApplication%2BSoftware.png)

## 3.2.1 Desktop Apps
+ Applications for desktop or laptop computers are sometimes called **desktop applications**.

![desktop app](https://i0.wp.com/ehayashi.com/wp-content/uploads/2020/07/tutorial_web-app.png)

## 3.2.2 Mobile Apps
+ And those for mobile devices are called **mobile apps**.

![mobile app](https://res.cloudinary.com/jerrick/image/upload/v1610287171/5ffb0843da62b9001cd087e8.jpg)

![mobile app time spent](https://www.statista.com/graphic/1/1272800/worldwide-mobile-apps-time-spent-daily.jpg)

### 3.2.3 Web Application
+ A web application (or web app) is application software that runs in a web browser, unlike software programs that run locally and natively on the operating system (OS) of the device.
+ Web applications are delivered on the `World Wide Web` to users with an active network connection.
+ Web applications are usually coded in browser-supported language such as JavaScript and HTML as these languages rely on the browser to render the program executable.
+ Some applications are dynamic, requiring server-side processing. Others are completely static with no processing required at the server.
+ The web application requires a web server to manage requests from the client, an application server to perform the tasks requested, and, sometimes, a database to store the information.
#### 3.2.3.1 A typical web application flow
+ 1. User triggers a request to the web server over the internet, either through a web browser or the application’s user interface
+ 2. Web server forwards this request to the appropriate web application server
+ 3. Web application server performs the requested task – such as querying the database or processing the data – then generates the results of the requested data
+ 4. Web application server sends results to the web server with the requested information or processed data
+ 5. Web server responds back to the client with the requested information that then appears on the user’s display
#### 3.2.3.2 Example of a web application
+ Web applications include online forms, shopping carts, word processors, spreadsheets, video and photo editing, file conversion, file scanning, and email programs such as Gmail, Yahoo and AOL. Popular applications include Google Apps and Microsoft 365.
+ Google Apps for Work has Gmail, Google Docs, Google Sheets, Google Slides, online storage and more. Other functionalities include online sharing of documents and calendars. This lets all team members access the same version of a document simultaneously.

#### 3.2.4 Cloud Apps
+ Cloud applications are software that users access primarily through the internet, meaning at least some of it is managed by a server and not users' local machines.
+ If designed well, cloud applications can offer a user experience like a program installed entirely on a local machine, but with reduced resource needs, more convenient updating, and the ability to access functionality across different devices.
+ Learn more about cloud applications [here](https://blog.servermania.com/what-is-a-cloud-application/).

![Cloud Apps](https://managedmethods.com/wp-content/uploads/what-is-cloud-application-security-blog-featured.jpg)


# References
+ [Assembly - Introduction](https://www.tutorialspoint.com/assembly_programming/assembly_introduction.htm)
+ [Higher level and lower level languages](https://computersciencewiki.org/index.php/Higher_level_and_lower_level_languages)
+ [Interpreter](https://en.wikipedia.org/wiki/Interpreter_(computing))
+ [Web Application](https://en.wikipedia.org/wiki/Web_application)
