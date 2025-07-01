```
C Programming – Day 6 Notes  
Date: 23-06-2025  
By: Samatha

______________________________________________________

Short Data Type (2 Bytes)  
____________________________

1. **Signed short**  
   Syntax:  
   short sval;  
   Range: -32,768 to +32,767  
   - Can store both negative and positive values  
   - Most Significant Bit (MSB) is treated as the **sign bit**

2. **Unsigned short**  
   Syntax:  
   unsigned short sval;  
   Range: 0 to 65,535  
   - Can store only positive values  
   - MSB is not treated as a sign bit

Explanation:  
- A short occupies **16 bits (2 bytes)** in memory  
- For signed:  
  - Bit 15 (MSB) is for sign (0 for +ve, 1 for -ve)  
  - Remaining 15 bits represent the magnitude  
- For unsigned:  
  - All 16 bits are used for value (no sign bit)

______________________________________________________

Wrap Around in short  
_______________________

- When the value **exceeds the maximum limit**, wrap around occurs.  
- This happens during addition or subtraction if the result goes beyond range.

Example with unsigned short:  
unsigned short sval = 65535;  
sval = sval + 1;   // Output: 0 (wrap around)

- Value after 65535 wraps to 0  
- If decremented below 0, it wraps around to 65535

Example:  
sval = 0;  
sval = sval - 1;   // Output: 65535 (wrap around)

______________________________________________________

Signed int (4 Bytes)  
_______________________

1. **Signed int**  
   Syntax:  
   int val;  
   Range: -2,147,483,648 to +2,147,483,647  
   - Can store both negative and positive values  
   - MSB (bit 31) is treated as sign bit  
   - 4 bytes = 32 bits

2. **Unsigned int**  
   Syntax:  
   unsigned int val;  
   Range: 0 to 4,294,967,295  
   - Can store only positive values  
   - All 32 bits used for value

Explanation:  
- For signed int:  
  - Bit 31 is sign bit  
  - Remaining 31 bits for magnitude  
  - Total values: 2^32  
  - Half for positive, half for negative

- For unsigned int:  
  - 32 bits give 2^32 values  
  - Range: 0 to 4,294,967,295

______________________________________________________

Note on Compilers  
______________________

- On **16-bit compilers** like Turbo C, `int` takes **2 bytes**  
- On **32-bit compilers**, `int` takes **4 bytes**  
- Always check your compiler's architecture for exact type sizes

______________________________________________________

Summary  
__________

- short (signed): 2 bytes, range -32,768 to +32,767  
- short (unsigned): range 0 to 65,535  
- int (signed): 4 bytes, range -2,147,483,648 to +2,147,483,647  
- int (unsigned): range 0 to 4,294,967,295  
- Wrap around occurs when value exceeds type range  
- Compiler bit-size affects the memory size of data types  
```
