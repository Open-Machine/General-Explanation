<h1 align="center">Open Machine</h1>
<div align="center">

<img align="center" src="https://raw.githubusercontent.com/Open-Machine/README/master/Media/logo-horizontal.png" alt="open-machine"/>

<br/>
The goal is to to design and build a computer from scratch.
<br/>
I will only use logical gates to build the circuit and GoLang to build the compiler and assembler for your computer.
<br/>
I also want to understand how a computer works behind the curtains and maybe do some things my way.

</div>

## [WIP] Todo
**Circuit**
- [ ] Signed integer
- [ ] Float
  - [ ] Summation and Subtraction
  - [ ] Division circuit and command
- [ ] Clock
- [ ] Own RAM
- [ ] Own Register

**High-Level Language**
- [ ] High-Level Language Compiler

**Future**
- [ ] Built-in data structures in the High-Level Language Compiler
- [ ] Interpreted Language
- [ ] Compiler and Assembler inside my machine
- [ ] Print to Screen
- [ ] Read from Keyboard
- [ ] Basic Operating System
- [ ] Disk

---

## 🔖 Table of Contents
#### 1. [💡 The Idea](#the-idea)
#### 2. [💻 How does a computer work behind the curtains?](#how-does-a-computer-work-behind-the-curtains)
#### 3. [▶️ Steps to run the machine with your program](#steps-to-run-the-machine-with-your-program)
#### 4. [👨🏻‍💻 Code Examples](#code-examples)
#### 5. [📄 Contributing Guidelines](#contributing-guidelines)

---

# 💡 The Idea

The idea came from an [article](https://medium.com/@luca.assumpcao.dillenburg/programming-tips-from-a-not-yet-experienced-programmer-754623ce28ae) I wrote about some tips for developers:

> And a message for those (myself included) that still want to build apps entirely from scratch because "That's the only way it will feel my doing only":
> 
> There's nothing wrong with building it from scratch. On the contrary, you can learn so much more when doing so. However, don't fool yourself into thinking that you built it entirely yourself. No program is created by just one person. If you want to achieve this, go ahead and start picking up some stones to build your computer first, then you can create your programming language and only then, your program.

I was obviously not encouraging people in any way to do that, but a few weeks later I asked myself: "What if I do just that? Could I actually do it?".

[ ⚠️ **Disclaimer**: Of course, I am doing some research and using knowledge developed by many people over many years of study. So I'm still not building it entirely on my own. In fact, I don't think that's even an option anymore since everybody has some knowledge about computers today. ]

Anyway, with that out of the way, this is when the everything started: a small doubt in my head was fuel enough to face the challenge.

---

# 💻 How does a computer work behind the curtains?
Developers usually have a good understanding of how a computer works. However, for me at least understanding a computer so deeply that you would be able to actually build one yourself seemed like an impossible task. So, in this section I want to break to you the most important pieces of the computer puzzle that you need to know in order to build your own computer from scratch using only circuits.

### Circuits
Click [here]() to know more about how the circuits work and how they were built.

### Code
Since the machine only understands bits of information and it would be very hard to actually memorise all these numbers, in the not so early days of computers they invented computer languages that could be translated to the bits that a machine can actually understand which is called Machine Code. This process is called compiling or assembling depending on the language.

#### Assembly
Click [here]() to know more about how you can code in assembly and how it was developed.

#### High-Level Languages
There are other categories of high-level languages such as compiled languages and interpreted languages. 
For high-level languages the process of translating the code to the machine code is called compiling, because 

---

# ▶️ Steps to run the machine with your program


### I) Code to Executer
As we discussed earlier, in order to to run your program, you have to write the code then assemble or compile it depending on the language you used.

- **From the machine code**
	If you wrote your code using only numbersYou can jump to the next step. You already have executable code.

- **From the assembly code: Assemble**
	If you wrote your program in Machine Code, you only need to assemble it, because there's a very strong correspondence between the instructions in the language and the architecture's machine code instructions: every instruction in the language is a machine code instruction and vice-versa.

	In the **Machine-Code** repository, use the commands below to assemble your code:
	```sh
	./assembler assemble filename.asm
	```

- **From the High-Level Language: Compile**
	Since each instruction in a high-level language corresponds to many machine code instructions, the process of generating an executable from its code is called "compile".

	In the **High-Level-Language** repository, use the commands below to compile your code:
	```sh
	./compiler compile filename.lang
	```


### II) Run the machine and the program in it
1. In the **Circuits** repository, use the commands below to run the machine:
	```sh
	java -jar logisim-evolution.jar
	```
2. Import the circuit file by navigating the menu:
   *```File -> Open -> Select main.circ from the repository folder```*
3. Open Main file on the left side of Logisim
4. Paste the executable code into the RAM
   - If it was generated from the Assembly Code or written in Machine Code, you should paste the code in the beginning of the RAM. Also, you may want to change some values of the memory as if you were initializing variables.
   - If it was generated from the High-Level Language there's nothing else you have to do.
5. Run the Program by navigating the menu:
   *```Simulate -> Enable 'Ticks Enabled'```*
   - You can change the speed of the program by navigating the menu: 
	*```Simulate -> Tick Frequency -> To get the fastest execution, select the top item```*

---

# 👨🏻‍💻 Code Examples
You can find examples of code in the ```Examples``` folder.
#### Examples List
- [Basic-IO](Examples/basic-io)

---

# 📄 Contributing Guidelines
Check out the contributing guidelines [here](https://github.com/Open-Machine/Organization-README/blob/master/CONTRIBUTION.md).
