# C Programming – Day 2 Notes

Date: 18-06-2025
By: Samatha

---

## The `printf()` Function and Its Arguments

* We can provide input (called arguments) to `printf()` inside parentheses.
* These arguments are used to display output on the screen.
* `printf()` can accept a single or multiple arguments, separated by commas.

### Example:

```c
printf("Hello");
printf("World");
```

**Output:**

```
HelloWorld
```

**Explanation:**
Both strings are printed one after another in the same line since there is no newline character or space between them.

---

## Escape Sequence Characters

Escape sequences are non-printable characters that control the output format.
They start with a backslash `\` and are used inside `printf()`.

---

### 1. `\n` – New Line (Line Feed)

* Moves the cursor to the beginning of the next line
* ASCII value: 10
* Also called Line Feed (LF)

#### Example:

```c
printf("Hello\n");
printf("World");
```

**Output:**

```
Hello
World
```

**Explanation:**
After printing "Hello", `\n` moves the cursor to the next line. Then "World" is printed on that new line.

---

### 2. `\t` – Horizontal Tab

* Adds a horizontal tab space
* Moves the cursor forward by a fixed number of spaces
* ASCII value: 9
* Also called Horizontal Tab (HT)

#### Example:

```c
printf("Hello\tWorld");
```

**Output:**

```
Hello   World
```

**Explanation:**
There is a tab space between "Hello" and "World".

---

### 3. `\b` – Backspace

* Moves the cursor one position backward
* ASCII value: 8
* Also called Backspace (BS)

#### Example:

```c
printf("Helloo\bWorld");
```

**Output:**

```
HelloWorld
```

**Explanation:**
The `\b` removes the last character 'o' from "Helloo", and "World" gets printed right after that.

---

### 4. `\a` – Alert or Beep

* Produces a beep sound
* Called Audible Alert or Alarm
* ASCII value: 7
* No visible output, but system may beep

---

## Comments in C

* Comments are non-executable lines used to explain code
* They are ignored by the compiler

### Types of Comments:

1. Single-line comment

```c
// This is a comment
```

2. Multi-line comment

```c
/* This is
   a multi-line
   comment */
```

---

## When are Comments Removed?

* Comments are removed during the preprocessing stage of compilation
* They do not become part of the final executable file

---

## Compilation Stages in C

1. Preprocessing – Handles `#include`, macro expansion, and removes comments
2. Compilation – Converts code to assembly language
3. Assembly – Converts assembly to machine code
4. Linking – Links all code and libraries into a final executable

---

## Format Specifiers in `printf()`

* The first argument in `printf()` is called the control string
* It may contain format specifiers to print variables
* Examples:
  `%d` for integers
  `%f` for floats
  `%c` for characters
  `%s` for strings

(We will learn detailed usage of each format specifier later.)

---

## Identifiers in C

* Identifiers are names used for variables, arrays, functions, etc.
* They are user-defined names given to memory locations

### Rules for Identifiers:

1. Must begin with a letter (A–Z, a–z) or underscore `_`
2. Can include digits, letters, and underscores
3. No spaces or special characters allowed
4. Cannot use predefined keywords like `int`, `float`, etc.
5. C is case-sensitive – `Value` and `value` are treated differently

---

### Example:

```c
int val;
val = 25;
```

**Explanation:**

* `val` is an identifier
* It is a variable of type `int` (integer)
* `val = 25;` assigns the value 25 to the variable
* `int` takes 4 bytes of memory (system dependent)

---

## Summary

* `printf()` is used to display output and accepts one or more arguments
* Escape sequences like `\n`, `\t`, `\b`, and `\a` are used to control output formatting
* Comments help explain the code and are ignored during compilation
* The C compiler works in stages: Preprocessing, Compilation, Assembly, Linking
* Identifiers are names for memory locations and follow strict rules

---
