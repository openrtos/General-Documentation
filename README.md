# General-Documentation
## What is RTOS - 
RTOS is an acronym for Real Time Operating System. There are such conditions where the correctness or requirement of the output not only depends upon the logic of the application but also time plays an important role for example deployment of airbags while a crash is detected in the vehicles , missile systems where a small error or small time delay may lead to massive destruction . So we need such type of OS to deal with these type of real time Applications 

## What is FreeRTOS?
FreeRTOS is a class of RTOS that is designed to be small enough to run on a microcontroller – although its use is not limited to microcontroller applications.

A microcontroller is a small and resource constrained processor that incorporates, on a single chip, the processor itself, read only memory (ROM or Flash) to hold the program to be executed, and the random access memory (RAM) needed by the programs it executes. Typically the program is executed directly from the read only memory.

Microcontrollers are used in deeply embedded applications (those applications where you never actually see the processors themselves, or the software they are running) that normally have a very specific and dedicated job to do. The size constraints, and dedicated end application nature, rarely warrant the use of a full RTOS implementation – or indeed make the use of a full RTOS implementation possible. FreeRTOS therefore provides the core real time scheduling functionality, inter-task communication, timing and synchronisation primitives only. This means it is more accurately described as a real time kernel, or real time executive. Additional functionality, such as a command console interface, or networking stacks, can then be included with add-on components.

