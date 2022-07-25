## Introduction to Assembly - bin0x01

All these fascinating computers run only on the basis of 0's and 1's.
But, Have you ever wondered how a computer is able to recognize 'xyz' lines of codes programmers write in any programming languages?
This is a simple to say yet very complex to do process which we are going to look into in this article.

#### **How does a CPU run a program written in English or human readable form?**

<img style="padding:5px;" align="right" width="150" height="400" src="https://raw.githubusercontent.com/bipin0x01/portfolio/main/assets/img/posts/Introduction-to-assembly/flowchart.jpeg">

&ensp;&ensp;Computers(say Digital Computers) can only understand 0s and 1s or simply binary which we, as humans find difficult to do manually for large computations. So, We cannot just communicate to each other.
Have you even seen a human talking like '0100100001100101011011000110110001101111
0010000001010011011001010111100001111001'.
Of Course Not!

&ensp;&ensp;Similarly, Lets assume humans are French and computers the Chinese. Both of them don't know each others mother tongue. So, they cannot communicate. The only way of communication is through translation, A person or language 'x' comes in the middle who knows both the languages. It takes the data from one person, translates and provides to the another whom we call real world language translators/interpreters.

&ensp;&ensp;So, Programs written in a programming language is actually converted into something the computer can understand 'machine code' by the use of translators.

&ensp;&ensp;To be specific, The code you write in human readable language([High Level language](https://en.wikipedia.org/wiki/High-level_programming_language)) like php, python, etc is first converted into a low level language code or assembly code with the help of translators like compiler of interpreter. Again the assembler converts the assembly code into a object file which contains the source code of the program.

&ensp;&ensp;Now, Linker links the object file with the library file present in the system and generates a machine code which is sent to the CPU.

#### **Wait, wait, what the hell is [Linker](<https://en.wikipedia.org/wiki/Linker_(computing)>) and a library file? Don't worry, I've got your back.**

&ensp;&ensp;If you are a programmer, you might be familiar with [libraries](<https://en.wikipedia.org/wiki/Library_(computing)>) If not you will eventually know it. It's the same term and is basically pieces of pre-written code to do some tasks. For Example: TensorFlow is a well known python library for Machine Learning. So, If you write a program that uses the 'Tensorflow' library in your python program. The [Linker](<https://en.wikipedia.org/wiki/Linker_(computing)>) links or binds all the assembled object files together with that library.
Moreover, Linker also links the object code to all the other important files like [makefiles](<https://en.wikipedia.org/wiki/Make_(software)>), etc.(**which we'll not talk about**). Then the final linked file we get, is as executable binary also known as bin.

<img style="padding:10px;" height="250px" width="350px" align="left" src="https://raw.githubusercontent.com/bipin0x01/portfolio/main/assets/img/posts/Introduction-to-assembly/linker-process.webp">

&ensp;&ensp;When the executables/bins are run, the CPU processes the given machine code and performs the instruction by using the registers in the processor which are made up of flip flops(made of logic gates which is the base of digital electronics).

#### **Why Assembly?**

&ensp;&ensp;As of now, you have the basic understanding of how long the process is. In every steps the program takes some time. So, higher the program starts from, the longer it will take for the program to execute.

&ensp;&ensp;So, Yeah! Talking directly to the computers through machine code might be the fastest way but not the easiest. This is also the reason why programming language like python is slower than C, because even inside the high level programming languages, there is a queue of higher highs and the rule remains same, higher it goes, slower it becomes.

Lets compare it to a real life example, Suppose there are 5 people standing next to each other namely A, B, C and D respectively.

&ensp;&ensp;Here, person 'A' knows the language of 'B', 'B' knows the language of 'C', 'C' knows the language of 'D' and vice versa. So , In order for A to talk to 'D', the information gets passed through 'B' and 'C' then to 'D' which again sends the reply through the same path taking some time. This is how it works in simple manner.

&ensp;&ensp; If 'A' wants to talk with D in short amount of time, A should know the language of D to get in the place of C. Similarly, We can use Assembly to make the programs talk to the computer a lot faster.

&ensp;&ensp; But, That's not everything. There is more to go! Just Keep Scrolling.

#### **Reasons to learn Assembly?**

&ensp;&ensp; It is the most human readable language which is closest to the computers after machine language, which is a lot harder to memorize. Assembly uses pneumonics instructions for performing task and making it easier to understand.

&ensp;&ensp; What every language you write a program with, It eventually gets passed through assembly language relevant to the architecture of the system/CPU used(Each system of difference architecture has its own syntax or way or writing assembly codes). So, If you know programming in assembly language you can edit, debug or examine the functionality of any program whether it is written in java, C++, Python, etc . This is where the concept of reverse engineering comes to play which we will be discussing in future articles.

Some other uses of Assembly:
&ensp;&ensp;It is used in embedded Programming and device driver which requires hardware specific instructions, Real time systems where program execution latency plays crucial role.

&ensp;&ensp; In an academic perspective, Assembly is used for better understanding of how the processor processes 'makes things happen' by use of memory addresses and registers.

&ensp;&ensp; In short, It is a bridge between the program and hardware interface. Use of assembly helps us to talk directly to the system.

#### **Extras**

You may skip the parts below if you feel it going over the head.

&ensp;Low level Language are hardware specific i.e code written for one type of architecture or just say one model of processor wont work with others.
For Example, low level code written for intel 8051 won't work with intel x86 processors. This can be taken as in disadvantage because one has to learn many low level languages based on the architecture of processor used. The same python program is completely different machines with two 'x' and 'y' versions or architecture of processors.

&ensp;
Note: **In this article term 'Assembly' is used to define low level language and doesnot refer to single programming language but is a group of similar languages which are architecture dependent in terms of syntax**
Instead of program conversion from high level language to the assembly, in real scenerio the executables or binaries are disassembled into the assembly language for reverse engineering which we will further discuss in the next part of blog series.

**Disclaimer: I, the writer of this article do not claim to be any kind of expert but a keen learner. So, Feedbacks, corrections and addups are highly appreciated. Everything that is explained above is oversimplified and is meant for beginners with at least some knowledge of computers and programming.**
