# General-Documentation
## What is RTOS - 
RTOS is an acronym for Real Time Operating System. There are such conditions where the correctness or requirement of the output not only depends upon the logic of the application but also time plays an important role for example deployment of airbags while a crash is detected in the vehicles , missile systems where a small error or small time delay may lead to massive destruction . So we need such type of OS to deal with these type of real time Applications 

## What is FreeRTOS?
FreeRTOS is a class of RTOS that is designed to be small enough to run on a microcontroller – although its use is not limited to microcontroller applications.

A microcontroller is a small and resource constrained processor that incorporates, on a single chip, the processor itself, read only memory (ROM or Flash) to hold the program to be executed, and the random access memory (RAM) needed by the programs it executes. Typically the program is executed directly from the read only memory.

Microcontrollers are used in deeply embedded applications (those applications where you never actually see the processors themselves, or the software they are running) that normally have a very specific and dedicated job to do. The size constraints, and dedicated end application nature, rarely warrant the use of a full RTOS implementation – or indeed make the use of a full RTOS implementation possible. FreeRTOS therefore provides the core real time scheduling functionality, inter-task communication, timing and synchronisation primitives only. This means it is more accurately described as a real time kernel, or real time executive. Additional functionality, such as a command console interface, or networking stacks, can then be included with add-on components.

## DIFFERENCE BETWEEN GPOS AND RTOS
General purpose operating systems cannot perform real time tasks whereas RTOS is suitable for real time applications.
There is deadline associated with real time kernel but GPOS does not follow timely mechanism.
The real time kernel follows preemptive scheduling policy whereas GPOS follow non preemptive scheduling technique.
Synchronization is a problem with GPOS whereas synchronization is achieved in real time kernel.
Inter task communication is done using real time OS where GPOS does not.
Latency is a problem with GPOS but it is overcome using real time OS.
Priority inversion cannot be done in GPOS, it is done with real time kernel.
Jitter i.e. timing error in task is not present in real time OS, present in GPOS.
The mathematical relation cannot be defined for GPOS, for a real time OS mathematical equation can be defined.
