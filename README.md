Our team created a custom printf function called _printf for the C programming language. It was designed to take various inputs and optional arguments, similar to the standard library function printf, and has been optimized to use a local buffer of 1024 bytes for printing, although it can handle larger data sets.

When _printf is executed successfully, it returns the total number of characters printed to the standard output stream (excluding the null byte at the end of strings). However, if an output error occurs, the function returns -1.

The _printf function prototype is: int _printf(const char format, ...). The first argument is mandatory, and the subsequent arguments can be none or many.

The format string is a character string enclosed by double quotes, consisting of zero or more directives, ordinary characters (not %), and conversion specifications. Each conversion specification begins with the % character and ends with a conversion specifier.

Between the % and conversion specifier, there can be zero or more flags, an optional field width, an optional precision modifier, and an optional length modifier. The flags include #, 0, -, ' ', and +. The field width can be a decimal digit string or a * character, and the precision can be specified with a period (.) and a decimal digit string or a * character.

The length modifiers are l and h, which are used for converting to a long int or unsigned long int and a short int or unsigned short int, respectively.

The conversion specifiers include d and i for signed decimal notation, o, u, x, and X for unsigned octal, decimal, and hexadecimal notation (with lowercase and uppercase letters), c for converting to an unsigned char, s for a string of characters, p for a void * pointer argument represented as a hexadecimal in lowercase, % for writing a % character, b for converting to a binary representation, and S for a string of characters with non-printable characters represented as \x followed by the corresponding hexadecimal value.

Our _printf function can handle all these format specifiers and modifiers and is a custom solution that does not rely on any standard library files. We submitted this project as part of our ALX software engineering course and received a grade for it.

Authors

Ebenezer Nyamekye 
Yonas Leykun
