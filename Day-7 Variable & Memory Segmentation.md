```
C Programming – Day 7 Notes  
Date: 24-06-2025  
By: Samatha

______________________________________________________

Variables in C  
__________________

- Variables are names given to memory locations.  
- These are used to store data that can change during program execution.  
- Variables must be declared before they are used.  
- Each variable is associated with a **data type**, which defines what type of data it can hold.

Example:  
int val;  
val = 25;    // Valid  

Invalid Example:  
25 = val;    // Compilation error – Constants cannot be on the left-hand side of assignment

______________________________________________________

Expressions in C  
_____________________

- An **expression** is a combination of variables, constants, and operators that evaluates to a value.  
- Example:  
  x = a + b;     // The result of a + b is assigned to x  
- The left side of the assignment must always be a variable.

Invalid Example:  
a + b = x;    // Error – Expression cannot be on the left side

______________________________________________________

Function Return Values in Assignment  
_______________________________________

- We can assign the return value of a function to a variable.  
Example:  
int x;  
x = printf("Linux");  

Explanation:  
- `printf()` returns the number of characters printed.  
- In this case, x will store that return value.

More Examples:  
printf("%d", printf("Hello\n"));  
Output:  
Hello  
6  
(Backslash elements like `\n` are also counted as one character)

______________________________________________________

Memory Segments in C Programs  
_________________________________

When a program is compiled and executed, it is divided into several memory segments:

1. **Text Segment**:  
   - Contains compiled code (machine instructions)

2. **Data Segment**:  
   - For global and static variables that are **initialized**

3. **BSS Segment** (Block Started by Symbol):  
   - For global and static variables that are **uninitialized**

4. **Heap**:  
   - Used for dynamic memory allocation (e.g., malloc)

5. **Stack**:  
   - Used for function calls, local variables, etc.

______________________________________________________

Global Variables  
______________________

- Global variables are declared **outside all functions**  
- If a global variable is **not initialized**, it goes into the **BSS Segment**  
- If initialized, it goes into the **Data Segment**

Example:  
int x = 25;       // Goes to Data Segment  
int y;            // Goes to BSS Segment

______________________________________________________

Executable Files  
_____________________

- After compiling a `.c` file, an **executable file** is created  
- This file is in binary format and cannot be read directly  
- Special tools are used to inspect them

Common Tools:  
- `objdump` – displays information from object files  
- `readelf` – displays contents of ELF (Executable and Linkable Format) files

Executable file types may differ:  
- CLI (Command Line Interface)  
- GUI (Graphical User Interface)  
- Embedded devices: microcontrollers, smartphones, smart TVs

______________________________________________________

Summary  
__________

- Variables store data and must be declared before use  
- Expressions combine variables and constants to compute values  
- The left side of an assignment must be a variable, not an expression  
- Memory is divided into segments like Text, Data, BSS, Heap, and Stack  
- Tools like objdump and readelf help analyze executable files  
```
