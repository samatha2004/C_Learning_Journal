```
C Programming – Day 4 Notes 
Characters in c
Date: 19-06-2025  
By: Samatha

______________________________________________________

Range of Values – Character Variables  
______________________________________

- A character must be enclosed within **single quotes** when assigned to a variable.

Example:  
char ch = 'A';

Explanation:  
- Characters are not stored directly as symbols.  
- They are stored using their **ASCII values**.  
- For example, 'A' is stored as 65 (ASCII value) in memory.  
- 1 byte is used for character storage.

We can also assign a character using its ASCII value directly:  
char ch = 65;   // equivalent to 'A'

______________________________________________________

What is a Format Specifier?  
_____________________________

- A format specifier is a combination of `%` and a conversion character.  
- It tells the compiler **how to interpret and display** the data using `printf()` or `scanf()`.

Examples:  
%c   → for character  
%d   → for integer  
%f   → for float  
%ld  → for long integer  

______________________________________________________

Purpose of Format Specifiers in printf() and scanf()  
______________________________________________________

- Format specifiers specify the **type of data** and how to convert binary data to human-readable form (ASCII characters).  
- Even though characters are stored as numbers in memory (binary), we can use format specifiers to print them correctly.

Example:  
Code:  
char ch = 'a';  
printf("%c", ch);     // Output: a  
printf("%d", ch);     // Output: 97 (ASCII value of 'a')

Another example:  
char ch = 65;  
printf("%c", ch);     // Output: A  
printf("%d", ch);     // Output: 65

______________________________________________________

Important Notes on Character Values  
_____________________________________

- Characters can store integer values only within a specific range (usually -128 to 127 for signed char).  
- Non-printable characters are those with ASCII values 0–31.  
- They do not produce visible output on the screen.  
- You can assign both characters and ASCII values directly to `char` type variables.

Example:  
char ch = '8';        // ASCII value: 56  
char ch = 8;          // Backspace (non-printable)

char d = '0';         // ASCII value: 48  
char ch = 10;         // Newline (non-printable)

______________________________________________________

Summary  
_________

- Characters are stored as ASCII values in memory.  
- Use single quotes for character literals.  
- Format specifiers like %c and %d are used to print characters or their ASCII values.  
- ASCII values help to understand how characters are handled internally.  
```
