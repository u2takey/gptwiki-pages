# bitwise 
## chatgpt 
"Bitwise" is not a command, rather it is a term used in computer programming to refer to operations performed on individual bits of binary data. 

Bitwise operations typically involve bitwise logical operators AND, OR, XOR, NOT and bit shifts (left-shift and right-shift).

1. The bitwise AND operator returns a 1 in each bit position for which the corresponding bits of both operands are 1s.

Example:

a = 5 (binary 0101)
b = 6 (binary 0110)

a & b = 4 (binary 0100)

2. The bitwise OR operator returns a 1 in each bit position where either operand has a 1.

Example:

a = 5 (binary 0101)
b = 6 (binary 0110)

a | b = 7 (binary 0111)

3. The bitwise XOR operator returns a 1 in each bit position where only one of the bits is 1.

Example:

a = 5 (binary 0101)
b = 6 (binary 0110)

a ^ b = 3 (binary 0011)

4. The bitwise NOT operator flips all the bits of the operand.

Example:

a = 5 (binary 0101)

~a = -6 (binary 1010)

5. Bit shift operators move the bits of the operand to the left or right by a specified number of positions.

Example:

a = 5 (binary 0101)

a << 1 = 10 (binary 1010)

a >> 1 = 2 (binary 0010)

Overall, bitwise operations are useful for optimizing code and manipulating individual bits of binary data. 

## tldr 
 
> Multi base interactive calculator supporting dynamic base conversion and bit manipulation.
> More information: <https://github.com/mellowcandle/bitwise>.

- Run using interactive mode:

`bitwise`

- Convert from decimal:

`bitwise {{12345}}`

- Convert from hexadecimal:

`bitwise {{0x563d}}`

- Convert a C-style calculation:

`bitwise "{{0x123 + 0x20 - 30 / 50}}"`
