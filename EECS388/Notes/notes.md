# Notes

---------------
# **Thursday January 18th**
---------------
### Overview of the topics

### Embedded Systems
* Computers are desigend for a specific purpose
* *Modern embedded systems contain a large number chips or integrated circuits (ICs)*


##### Types Digital, Analog, and Mixed Signals
* **Digital IC**
    * Microprocessor
* **Analog Ic**
    * Sensors
* **Analog-mixed -signal**
* Contains both digital and analog in a single chip/IC

##### Embedded vs. general computing systems: Number of Applications
* Embedded:
    * Not end-user programmable, On-time
    * Power, memory & compute limited: i.e. smartwathch, implantable device
* General computing:
    * End-user programmable, Faster is awlays better!
    * Greater resouce! i.e. servers

### Internet of Things (IoT)
* **Internet** connected embedded systems
* Interconnection to the internet of devices is important

### Cyber-Physical Systes (CPS)
* Cyber system (computer) + physical system (Plant)
* Embedded systems but integration emphasied

### Real-Time Systems
* The correctness not only logical and computation but produced at the correct time
* A CORRECT VALUE AT THE WRONG TIME IS A FAULT

### Trends in modern embeded systems
* Trending towards: cheaper, powerful, and more connected
* The ECU computing capactiy in BMW i8 is greater than the i3 ( developed in 2014 or earlier )
* Rasberry pi 2 had even greater speeds
    * @ 4,744 MIPS (Millions of instructions per second) 1.0 GHz
* Human like intelligence in modern vehicles
* **Super computer introduced on a car in tesla 2019**
    * Full Self Driving Chip
    * Whats inside
        * CPU
        * GPU (1Ghz, 600 GLOPS) ( GIGA FLOPS ) GIGA FLOPS that is some cool shit man!!!!!!
        * Neural processing units to handle floating points

### Performance
* Processing real time from sensors in cars has increased a lot
* Autombile changes described in three step process]
    * **Inform**
        * Drivers wanted a way to meld lifestyle and car
    * **Assist**
        * Assisting drivers
    * **Assume**
        * communicate collaborate and fufill all functions

### Efficiency
* Size weight, power, and cost constraints are all decreasing as time progresses

### Safety
    Examples below are examples of things that have outside influences and can have failure
* *Examples
    * Therac 25
        * Computer controlled radiation therapy
    * Arian 5
        * Rocket destroyed in 40 seconds

### Security and Privacy
    Confidentiality issues: Infromation could be stolen

* Attack can be done in many ways
    * **Side channel leakage** : Observing the power consumption of the chip to guess the passwords
    * **Hardware or software trojan** : hidden functionality in software or hardware that leaks information to outsider
    * **Physical Attack** : Some dude touches your stuff and does some nasty stuff to it
###### .
    Integrity issues: An attacmed can start a failure inside a system

* Attack can be done in many ways
    * **Fault Inejection** : Change voltage to corrupt output
    * **Hardware or software trojan** : hidden functionality in software or hardware that leaks information to outsider
    * **Physical Attack** : Tampering mode or chip on your own hardware (i.e. your xbox series x version x installing xtynine)

### My Garbage Summary
* Limited Function computers in real world
* Requirements: perfromance, efficiency, safety, secrutiy, and privacy

---------------
# **TUESDAY JANUARY 23RD 2023**
---------------

---------------
# **EMBEDDED SOFTWARE DEVELOPMENT**
---------------

* **Software Abstraction**
    * Application programs, os, compiler

* **Hardware**
    * Primary Component: microprocessor or microcontroller
    * Abstractions: microacrchitecture and instruction set architecture
    * ![ISA: Instruction Set Architecture](ISA.png)

* **Example Abstraction**
    * *Application Software*
        * Word processor, internet, browser, games
    * *System software*
        * *OS* : manages resources to run applications
        * *Compiler* : translates programs to machine readable binary
    * *Hardware*
        * Processor, memory, IO
### Instructure Set Architecture
* (ISA)
* Acts as interface between hardware and software
* abstraction of hardware that can be controlled by assemby
* considred a manual for assembly
* specifis;
    * memory org
    * register set
    * instruction set (multiply, add, etc.)
* ARM, x86, MIPS, SPARC, and PowerPC

* *Analogy*
    * ISA of a car describes what the driver needs to do to get the carry out the drivers wishes

### Microarchitecture
* Design describes interconnections of microarch elelments
* Implementation of the ISA
* x86-64 : AMD, Intel

### Embed Sys Dev Platform
* exe runs on devices with the same arch

### Compiler tool chain
* .c/.h -> .i -> .s -> .o -> .exe
* prprocessor :
    * compiler : gcc
        * assembler  : as
            * linker : ld, turns machine code into executable code

### Cross Compilation
* compile on one system run on another
* hex holds 4x binary

### Problems
* Building can be complex
* building manually takes time and effot
* *SO WE USE MAKEFILESSS*

### Makefiles
* Make is a tool which controls the generation of executables and other non-source files of a program
* make file automates commands
