```
C Programming – Day 1 Notes  
Date: 147-06-2025  
By: Samatha

______________________________________________________

Basic Elements of C Language  
_____________________________

1. Character Set – Used to write a program  
2. Identifiers – Names given to memory locations  
3. Keywords – Predefined and reserved words  
4. Data Types – Used to define type of data  
5. Constants – Fixed values that don't change  
6. Variables – Used to store data  
7. Expressions – Combination of variables, constants, and operators  
8. Statements – Instructions written in C  

______________________________________________________

Character Set in C  
___________________

Character set is the set of valid characters that can be used in a C program. It is divided into 4 categories:

1. Alphabets  
_____________

- Uppercase: A to Z (65–90)  
- Lowercase: a to z (97–122)  
- Every character is associated with a unique integer value called ASCII value.

2. Numerics  
____________

- Digits: 0 to 9  
- These are also characters and have ASCII values.  
  For example:  
  '0' → 48  
  '1' → 49  
  '9' → 57

3. Special Symbols  
___________________

- Examples: @, #, %, (, ), {, }, etc.  
- These symbols also have unique ASCII values.  
- Even a space has an ASCII value, which is 32.

4. Backslash Characters (Escape Sequences)  
___________________________________________

- These are special characters starting with a backslash `\`  
- Mostly used in output functions like `printf()`  
- Examples include:  
  `\n` for new line  
  `\t` for tab space  
  `\\` for backslash  
  `\'` for single quote  
  `\"` for double quote

______________________________________________________

Printable and Non-Printable Characters  
_______________________________________

Printable Characters  
_____________________

- Characters that can be seen on the screen when printed.  
- These include alphabets, digits, special symbols, and space.  
- Examples: A to Z, a to z, 0 to 9, @, #, %, space, etc.

Non-Printable Characters  
_________________________

- Characters that are not directly visible on the screen.  
- These are used to control formatting or actions.  
- Examples: newline (`\n`), tab (`\t`), backspace, enter, etc.

______________________________________________________

ASCII Values – Some Examples  
_____________________________

'A' → 65  
'Z' → 90  
'a' → 97  
'z' → 122  
'0' → 48  
'9' → 57  
Space → 32  
Enter → 10 or 13  
DEL → 127  

- ASCII means American Standard Code for Information Interchange.

______________________________________________________

Important Points  
_________________

- C is a case-sensitive language. For example, `a` and `A` are treated as different characters.  
- Every character in C has a corresponding ASCII value.  
- Backslash characters (escape sequences) are used to perform special actions like line break, tab, etc.  
- Special symbols also have unique ASCII values.

______________________________________________________

The `printf()` Function  
________________________

- `printf()` is a standard library function in C.  
- It is used to display output on the screen.  
- Syntax example:  

Code:
printf("Hello, World!");
```
