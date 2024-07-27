# CS 2200 - Systems and Networks (Spring 2022)
I took CS 2200 @ Gatech in the Spring of 2022.

Lectured by Umakishore Ramachandran.

## About
[Official course listing page](https://oscar.gatech.edu/bprod/bwckctlg.p_disp_course_detail?cat_term_in=202008&subj_code_in=CS&crse_numb_in=2200).

The semester-long project LC-22 virtual circuit computer was built using Circuitsim.

This class was primarly taught with Assembly and C.

### Course Curriculum
Exposure to computer system structure and networking:
- Organization of the processor
- Memory hierarchy
- Storage devices
- Parallel processors
- Networking hardware
- Software abstractions in the operating systems for orchestrating their usage
- Networking protocols to connect the computer system to its environment

- (Competency Knowledge) Understand the difference between RISC and CISC architectures. Be able to identify the strengths and weaknesses of each paradigm.
- (Competency Knowledge) Understand and be able to explain runtime system concepts such as procedure calls and register saving. Be able to write recursive subroutines in assembly.
- (Competency Application) Understand how a processor is controlled. Given a datapath and an instruction set be able to write the finite state machine steps in a high-level meta language.
- (Competency Knowledge) Understand and be able to explain (at a high level) hardware modifications required to implement an interrupt system and to understand the basic concepts required to write an interrupt handler (in assembly language).
- (Competency Knowledge) Understand the basic principles of pipelining:
- Pipelining registers
- Potential performance improvements with pipelining
- Pipelining Hazards: Structural, Data, and Control
- (Competency Knowledge) Understand basic concepts of processor scheduling: Process vs program, PCB, scheduling algorithms (Round Robin, Shortest Job First, First Come First Served, Priority, Multilevel Queues), types of scheduler (short, medium, and long term), and -context switching.
- (Competency Comprehension)  Given a set of processes with appropriate parameters show scheduling behavior under different scheduling algorithms.
- (Competency Application) Be able to calculate the proper size required for pipeline register and speedups with pipelining.
- (Competency Application) Be able to solve basic word problems involving Amdahl's Law.
- (Competency Knowledge) Be able to identify and explain how to avoid or minimize the effect of the different types of pipelining hazards.
- (Competency Knowledge) Understand the drivers of memory cache designs: Temporal locality, spatial locality, and working set. Be able to match the design with the motivator.
- (Competency Knowledge) Understand the basic operation of virtual memory and typical components: Page table, virtual pages, physical frames, TLB, page/frame offset, page replacement algorithms (LRU, Random, FCFS, Optimum). Be able to describe the basic operation and -identify the necessary subsystems.
- (Competency Knowledge) Understand the basic design of typical caches including indexes, tags, dirty and valid bits as well as multi-word blocks, set-associative, and fully associative caches. Given selected design parameters (i.e. word size, memory available for data
- (Competency Knowledge) Understand basic concepts of parallel processing: UMA (SMP) vs NUMA configurations, multiprocessor cache coherency, network interconnection schemes, threads, mutex, condition variables.
- (Accomplishment Application) Be able to write multi-threaded programs using the pthreads package. An example would be a multithreaded producer-consumer application.
- (Competency Knowledge) Understand basic networking concepts: Ethernet (CSMA/CD), Token Ring, Payload vs. header and trailer, checksums, bandwidth, effective bandwidth, latency, MAC addresses, Network (IP) addresses, protocol stacks, TCP/IP, routing, hubs/repeaters, -bridges, VLANS, routers.
- (Competency Knowledge) Understand fundamentals of I/O devices such as polling versus interrupts, memory-mapped I/O, device registers (data, control, and status), disk memory concepts (sectors, tracks, platters, cylinders, seek time, rotational latency), disk scheduling algorithms (FCFS, SSTF, scan, c-scan, look, c-look)
- (Accomplishment Synthesis) Write and debug medium-sized C programs that simulate various of the above subsystems (interrupt enabled processor, virtual memory, multi-threaded operating system schedulers, reliable transport layer protocol which will be examples of operating-system-like coding.

### Projects

**Using Circuit Sim**

1. LC-22 Barebones

![LC-22 Datapath](https://github.com/d-lee-te/CS-2200/blob/92adf85fc2799c4a5dda1c2119a70e27e80f6079/LC-22%20Datapath.png)

Implemented datapath as shown above along with components shown above.

2. Interrupts - Added and implemented interrupts from input devices

3. Virtual memory system

![Frame](https://github.com/d-lee-te/CS-2200/blob/93e7df87fa0c6fe1289931e7262b902e734d3373/Frame.png)

- Simulator simulated a system w/ 20-bit byte-addressable physical memory
  - System had 24-bit virtual address sapce
  - Memory was divided into 16KB pages

**Implemented**
- Address splitting
- Frame table setup/initialization
- Process setup/initialization
- Context switch function for PTBR (page table base register)
- Memory access function
- Page fault function
- Free frame function
- Swap page function
- Process cleanup function
- Random replacement algorithm
- Clock Sweep Algorithm (page replacement algorithm)
- FIFO (First in first out) algorithm (page replacement algorithm)

4. Process scheduler
- CPU scheduling algorithms
  - FCFS (First come, first serve)
  - Round-Robin
  - PS (Preemptive Priority)
- CPU schedule process functions
- CPU scheduler invocation functions

5. Networking - Modify transport layer of simulated network for additional reliability

![Transport Layer](https://github.com/d-lee-te/CS-2200/blob/2357f63f98f49448b1bd673ab8acf03cfc58463f/RTP%20Protocol.png)

### Debrief
My favorite part of this class was probably working with the CPU scheduler and learning how to implement the algorithms. I didn't really find an extreme interest in any of the other material here, but it was good experience.

# Disclaimer
As most of the course content belongs to either the College or the Professors, I am transcribing my work and assignments to record the course.

As such, many assignments and files **may not include detailed descriptions or solutions**. This is done to avoid violations, avoid doxing myself and others, and any number of other reasons. If for any reason the full repo must be accessed, all assignments, descriptions, solutions, and class files are stored in a private version of the repo (so contact me. If you're a current student, don't bother since I won't give you access and it wouldn't help you anyway xp).

If possible, portions of the class will be linked to a separate readme explaining more about the linked assignment/solution/description/other.

If there exist any honorcode violations or any problems/solutions are *too* in-depth, please contact me. The intention of each public class repo is to record my experience and assignments of each class taken.

