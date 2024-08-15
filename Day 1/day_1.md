# 🖥️ Operating Systems Interview Questions

#### Day 1 - 16-08-2024

This document provides a list of 30 beginner-level operating systems questions along with easy-to-understand explanations. Use these for placement training and interview preparation.

---

## Table of Contents

1. [What is an Operating System?](#1-what-is-an-operating-system)
2. [What are the main functions of an Operating System?](#what-are-the-main-functions-of-an-operating-system)
3. [What is the difference between a process and a thread?](#what-is-the-difference-between-a-process-and-a-thread)
4. [What is process scheduling?](#what-is-process-scheduling)
5. [What is a deadlock?](#what-is-a-deadlock)
6. [What are the different types of operating systems?](#what-are-the-different-types-of-operating-systems)
7. [What is virtual memory?](#what-is-virtual-memory)
8. [What is a file system?](#what-is-a-file-system)
9. [What is paging in operating systems?](#what-is-paging-in-operating-systems)
10. [What is segmentation?](#what-is-segmentation)
11. [What is a kernel?](#what-is-a-kernel)
12. [What is the difference between user mode and kernel mode?](#what-is-the-difference-between-user-mode-and-kernel-mode)
13. [What is a semaphore?](#what-is-a-semaphore)
14. [What is a mutex?](#what-is-a-mutex)
15. [What is a context switch?](#what-is-a-context-switch)
16. [What is a system call?](#what-is-a-system-call)
17. [What is thrashing?](#what-is-thrashing)
18. [What is a process control block (PCB)?](#what-is-a-process-control-block-pcb)
19. [What is a fork system call?](#what-is-a-fork-system-call)
20. [What is a zombie process?](#what-is-a-zombie-process)
21. [What is the purpose of an interrupt?](#what-is-the-purpose-of-an-interrupt)
22. [What is a race condition?](#what-is-a-race-condition)
23. [What is memory management?](#what-is-memory-management)
24. [What is a priority inversion?](#what-is-a-priority-inversion)
25. [What is a critical section?](#what-is-a-critical-section)
26. [What is a page fault?](#what-is-a-page-fault)
27. [What is a daemon process?](#what-is-a-daemon-process)
28. [What is a bootloader?](#what-is-a-bootloader)
29. [What are device drivers?](#what-are-device-drivers)
30. [What is an inode?](#what-is-an-inode)

---

## Questions and Answers

### 1. What is an Operating System?

An Operating System (OS) is system software that manages hardware and software resources on a computer. It provides services for computer programs and acts as an intermediary between users and the computer hardware.

### 2. What are the main functions of an Operating System?

The main functions of an OS include:

- **Process Management**: Handles process creation, scheduling, and termination.
- **Memory Management**: Manages RAM and allocates memory to processes.
- **File System Management**: Manages files on the disk and directories.
- **Device Management**: Manages hardware devices and their communication.
- **User Interface**: Provides a user interface, either command-line or graphical.

### 3. What is the difference between a process and a thread?

- **Process**: A process is an independent program in execution that has its own memory space.
- **Thread**: A thread is a smaller unit of a process that shares the process's memory space and resources.

### 4. What is process scheduling?

Process scheduling is the method by which an OS decides which process or thread runs at any given time. It uses various scheduling algorithms like Round Robin, First-Come-First-Served, and Shortest Job First.

### 5. What is a deadlock?

A deadlock is a situation where two or more processes are unable to proceed because each is waiting for the other to release a resource. This results in a standstill where no process can continue.

### 6. What are the different types of operating systems?

- **Batch Operating Systems**: Executes batches of jobs without user interaction.
- **Time-Sharing Operating Systems**: Provides time-sharing among multiple users (e.g., Unix).
- **Distributed Operating Systems**: Manages a collection of separate computers to appear as a single system.
- **Embedded Operating Systems**: Used in embedded systems (e.g., RTOS).

### 7. What is virtual memory?

Virtual memory is a memory management technique that provides an "idealized" memory space for processes, allowing them to use more memory than physically available by using disk space.

### 8. What is a file system?

A file system is a method and data structure that an OS uses to manage and store files on a disk or storage device. Examples include FAT32, NTFS, and ext4.

### 9. What is paging in operating systems?

Paging is a memory management scheme that eliminates the need for contiguous allocation of physical memory and thus eliminates the problems of fitting varying sized memory chunks onto the backing store.

### 10. What is segmentation?

Segmentation is a memory management technique where memory is divided into different segments based on the logical division of the process, such as code, data, and stack.

### 11. What is a kernel?

The kernel is the core part of an operating system that manages system resources and communication between hardware and software. It operates in kernel mode with full access to hardware.

### 12. What is the difference between user mode and kernel mode?

- **User Mode**: A restricted mode where applications run with limited access to hardware and system resources.
- **Kernel Mode**: A privileged mode where the OS kernel has full access to hardware and can execute any CPU instruction.

### 13. What is a semaphore?

A semaphore is a synchronization tool used to manage access to shared resources by multiple processes or threads to avoid conflicts and ensure mutual exclusion.

### 14. What is a mutex?

A mutex (mutual exclusion) is a synchronization primitive used to ensure that only one thread or process can access a critical section of code or resource at a time.

### 15. What is a context switch?

A context switch is the process of saving the state of a currently running process or thread and restoring the state of the next process or thread to be executed.

### 16. What is a system call?

A system call is an interface provided by the OS that allows user-level applications to request services from the kernel, such as file operations and process management.

### 17. What is thrashing?

Thrashing occurs when the OS spends the majority of its time swapping data between memory and disk rather than executing processes, leading to poor performance.

### 18. What is a process control block (PCB)?

A PCB is a data structure used by the OS to store information about a process, including its state, program counter, register values, and memory management information.

### 19. What is a fork system call?

The fork system call is used to create a new process by duplicating the current process. The new process, called a child process, runs concurrently with the parent process.

### 20. What is a zombie process?

A zombie process is a process that has completed execution but still has an entry in the process table, usually because its parent has not yet read its exit status.

### 21. What is the purpose of an interrupt?

An interrupt is a signal sent to the processor indicating that an event needs immediate attention. It temporarily halts the current process and executes an interrupt handler to address the event.

### 22. What is a race condition?

A race condition occurs when two or more processes or threads access shared resources concurrently, and the final outcome depends on the non-deterministic ordering of their execution.

### 23. What is memory management?

Memory management is the process of handling the allocation and deallocation of memory space to different processes and ensuring efficient utilization of RAM.

### 24. What is a priority inversion?

Priority inversion happens when a lower-priority task holds a resource needed by a higher-priority task, causing the higher-priority task to be indirectly delayed.

### 25. What is a critical section?

A critical section is a part of the code that accesses shared resources and must be executed atomically to prevent race conditions.

### 26. What is a page fault?

A page fault occurs when a program accesses a page not currently in physical memory, triggering the OS to load the page from disk into RAM.

### 27. What is a daemon process?

A daemon process is a background process that runs continuously and performs system-related tasks such as managing hardware or performing scheduled tasks.

### 28. What is a bootloader?

A bootloader is a small program that initializes the hardware and loads the operating system into memory when the computer is started or rebooted.

### 29. What are device drivers?

Device drivers are specialized software that allows the operating system to communicate with and control hardware devices, such as printers, keyboards, and storage devices.

### 30. What is an inode?

An inode is a data structure on a filesystem that stores information about a file or directory, including its size, permissions, and location on disk.

#### **📚 Suggested Reading**

- [Operating System Interview Questions - Interview Bit](https://www.interviewbit.com/operating-system-interview-questions/)

- [Operating System Interview Questions - GeeksforGeeks](https://www.geeksforgeeks.org/operating-systems-interview-questions/)

---

Feel free to use this document for your training and interview preparation. Good luck!
