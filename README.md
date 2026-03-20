# Buffer Overflow Principles Lab
This lab explores the fundamentals of buffer overflow vulnerabilities and how they affect program execution, using a vulnerable C program (``stack1.c``), to analyze stack behavior, memory layout, and the impact of protections like Address Space Layout Randomization (ASLR).

**Goals:**
- Understand stack layout and function call mechanics
- Observe how buffers are stored in memory
- Learn how buffer overflows corrupt adjacent memory
- Analyze crashes caused by overwritten return addresses
- Examine the role of ASLR in preventing exploitation

## Setup
- Extract the provided files: ``unrar x lab1-code.rar``
- Compile the program: ``gcc -g stack1.c -o stack1``
- Run: ``./stack1``

## Main takeaways
- Buffer Overflow: Writing beyond buffer limits corrupts adjacent memory
- Stack Frame: Stores local variables, saved base pointer, and return address
- Return Address Corruption: Leads to control flow hijacking or crashes
- ASLR: Randomizes memory addresses to make exploitation harder
