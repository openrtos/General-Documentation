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

## TYPES OF REAL TIME OPERATING SYSTEM
Depending upon the nature of application real time OS are designed and they are classified into 3 types:

SOFT REAL TIME OPERATING SYSTEM
Soft real time OS is a type of OS where certain deadlines may be missed, they will respond at a time t=0+.

Soft real time systems are not constrained to extreme rules. The critical time of the soft real time may be delayed to some extent. The expected latency between the tasks and time constraints may be deviated.

The preemption period for a soft real time task is about few milliseconds.

EXAMPLES
Digital camera, mobile phones, online data base etc.

HARD REAL TIME OPERATING SYSTEM
Hard real time OS is a type of OS we can predict the deadline, they will respond at a time t=0. Hard real time systems are constrained to predicted time constraints, deadlines and latency.

EXAMPLES:
Air bag control in cars, anti-lock brake, engine control system etc.

The preemption period for hard real time system is almost less than few microseconds.

FIRM REAL TIME OPERATING SYSTEM
This type of RTOS has certain time constraints which are not strict and it may cause undesired effect.

Example for firm RTOS is automated visual inspection in industrial automation. This system examines and detects the defected parts of assembly line. This type is also called event response system.

In short RTOS based system is a time critical system where most of the tasks are completed in time so that most of the deadly events are reduced.

## Why use an RTOS?
There are well-established techniques for writing good embedded software without the use of an RTOS. In some cases, these techniques may provide the most appropriate solution; however as the solution becomes more complex, the benefits of an RTOS become more apparent. These include:

Priority Based Scheduling: The ability to separate critical processing from non-critical is a powerful tool.

Abstracting Timing Information: The RTOS is responsible for timing and provides API functions. This allows for cleaner (and smaller) application code.

Maintainability/Extensibility: Abstracting timing dependencies and task based design results in fewer interdependencies between modules. This makes for easier maintenance.

Modularity: The task based API naturally encourages modular development as a task will typically have a clearly defined role.

Promotes Team Development: The task-based system allows separate designers/teams to work independently on their parts of the project.

Easier Testing: Modular task based development allows for modular task based testing.

Code Reuse: Another benefit of modularity is that similar applications on similar platforms will inevitably lead to the development of a library of standard tasks.

Improved Efficiency: An RTOS can be entirely event driven; no processing time is wasted polling for events that have not occurred.

Idle Processing: Background or idle processing is performed in the idle task. This ensures that things such as CPU load measurement, background CRC checking etc will not affect the main processing.

