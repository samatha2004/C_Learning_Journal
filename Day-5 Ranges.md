```
C Programming – Day 5 Notes  
Date: 20-06-2025  
By: Samatha

______________________________________________________

String in C  
______________

- A string is a **sequence of characters** enclosed within **double quotes**.  
- Example: "Linux"  
- Internally, a **null character** `\0` is added at the end of every string automatically.  
- So, "Linux" occupies 6 bytes in memory: L, i, n, u, x, \0  
- The null character is used to indicate the end of the string.

______________________________________________________

ASCII Values Recap  
____________________

- Characters are stored using their ASCII values.  
- Example:  
  '0' → 48  
  'A' → 65  
  'a' → 97  

______________________________________________________

Range of Values for char  
__________________________

The range depends on whether the `char` is signed or unsigned.

1. Signed char (default in most systems)  
   - Can store both **positive and negative** values  
   - Range: -128 to +127  
   - The Most Significant Bit (MSB) is treated as the **sign bit**

2. Unsigned char  
   - Can store only **positive** values  
   - Range: 0 to 255  
   - MSB is not treated as a sign bit

Memory:  
- A `char` variable takes 1 byte (8 bits)  
- In signed char:
  - MSB = 1 → negative number  
  - MSB = 0 → positive number  
- 7 bits used for value, 1 bit for sign  
- Example range: -128 to 127

______________________________________________________

Wrap Around Behavior in Signed char  
_____________________________________

Example:  
char ch = 127;  
printf("%d", ch + 1);    // Output: -128 (wraps around)

Explanation:  
- When a signed char exceeds 127, it wraps around to the minimum value -128  
- Continuing to increment:  
  127 + 1 → -128  
  127 + 2 → -127  
  127 + 3 → -126  
  and so on...

Another example:  
char ch = 0;  
printf("%d", ch - 1);    // Output: -1  
If decremented below -128, wrap around occurs again.

______________________________________________________

Wrap Around Behavior in Unsigned char  
_______________________________________

Example:  
unsigned char ch = 255;  
printf("%d", ch + 1);    // Output: 0 (wraps around)

Explanation:  
- Unsigned char range is 0 to 255  
- If it exceeds 255, it wraps around to 0  
- Continuing to increment:  
  255 + 1 → 0  
  255 + 2 → 1  
  and so on...

______________________________________________________

Summary  
_________

- Strings are character arrays ending with a null character `\0`  
- `char` can be signed or unsigned  
- Signed char: range is -128 to 127  
- Unsigned char: range is 0 to 255  
- Wrap around occurs when value exceeds the range of char  
- ASCII values help understand how characters are stored and printed  
```
