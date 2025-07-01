```
C Programming – Day 7 Notes (Part 2)  
Date: 25-06-2025  
By: Samatha

______________________________________________________

Executable File & Memory Segments  
______________________________________

- An **executable file** is generated after compiling a program.  
- This file is present on the **hard disk**.  
- During program execution, it is **loaded into RAM**.  
- The file is divided into several **memory segments** when loaded.  
- These segments are copied from disk to RAM.

Segments include:  
1. **Text Segment** – Contains instructions (Read-only)  
2. **Data Segment** – Initialized global and static variables (Read/Write)  
3. **BSS Segment** – Uninitialized global and static variables (Read/Write)  
4. **Stack** – Stores function call information and local variables  
5. **Heap** – Used for dynamic memory allocation

______________________________________________________

Stack and Heap  
__________________

- Stack and Heap are created when the program is loaded into RAM.  
- **Stack:**  
  - Grows **downward** (from higher to lower memory addresses)  
  - Stores function call data (stack frames)  
  - Used for automatic memory allocation  
  - Each function call creates a **stack frame**

- **Heap:**  
  - Grows **upward** (from lower to higher memory addresses)  
  - Used for **dynamic memory allocation**  
  - Memory is allocated using:  
    - `malloc()`  
    - `calloc()`  
    - `realloc()`  
    - Freed using `free()`  

______________________________________________________

Why Stack Grows?  
_____________________

- When functions are called, memory blocks called **stack frames** are added to the stack.  
- These frames store local variables, return addresses, etc.  
- In system programming, every new thread created also gets a new **stack area**.

______________________________________________________

What Is Stored Above Stack?  
_____________________________

- **Command-line arguments** are stored above the stack in memory.  
- When a program is loaded into RAM, it becomes a **process**.

______________________________________________________

What Is a Process?  
_____________________

- A **program in execution** is called a **process**.  
- The same executable file, when loaded and running, is treated as a process by the operating system.

______________________________________________________

Tools to View Executables  
____________________________

- `objdump` – Used to inspect the contents of an object or executable file  
- `readelf` – Used to read ELF (Executable and Linkable Format) files

______________________________________________________

Viewing Running Processes  
_____________________________

- Use `ps -ef` command (in Linux CLI) to list all running processes  
- Use `top` command to monitor processes in real time  
- Both show process ID, memory usage, CPU usage, etc.  
- GUI alternative: System Monitor

______________________________________________________

Summary  
__________

- Executable files are loaded from hard disk to RAM for execution  
- Segments in memory include Text, Data, BSS, Stack, and Heap  
- Stack handles function calls; Heap handles dynamic memory  
- A running program is called a process  
- Tools like `ps`, `top`, `objdump`, and `readelf` are used to inspect system and program behavior  
```
