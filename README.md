I created a customized printf function called _printf for the C programming language. The goal was to have a function that could handle various inputs and optional arguments, similar to the standard library function printf, but with optimization that utilizes a local buffer of 1024 bytes for printing, even though it can process larger data sets.

When _printf runs successfully, it returns the total number of characters that have been printed to the standard output stream (except for the null byte at the end of strings). In the event of an output error, the function returns -1.

The _printf function prototype is: int _printf(const char format, ...). The first argument is mandatory, and the following arguments can be none or many.

The format string is a character string enclosed in double quotes that may have zero or more directives, ordinary characters (not %), and conversion specifications. Each conversion specification starts with the % character and ends with a conversion specifier.

Between the % and conversion specifier, there can be zero or more flags, an optional field width, an optional precision modifier, and an optional length modifier. The flags include #, 0, -, ' ', and +. The field width can be a decimal digit string or a * character, and the precision can be specified with a period (.) and a decimal digit string or a * character.

The length modifiers are l and h, which are used for converting to a long int or unsigned long int and a short int or unsigned short int, respectively.

The conversion specifiers include d and i for signed decimal notation, o, u, x, and X for unsigned octal, decimal, and hexadecimal notation (with lowercase and uppercase letters), c for converting to an unsigned char, s for a string of characters, p for a void * pointer argument represented as a hexadecimal in lowercase, % for writing a % character, b for converting to a binary representation, and S for a string of characters with non-printable characters represented as \x followed by the corresponding hexadecimal value.

This _printf function can handle all of these format specifiers and modifiers and is a custom solution that does not rely on any standard library files. I submitted this project as part of my ALX software engineering course and received a grade for it.

Author:

Ebenezer Nyamkye
