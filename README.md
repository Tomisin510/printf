Printf
Summary
This is a simple implementation of printf function that formats and prints data
Representation
The _printf() function produces output according to a format which is described below. This function write its output to the the standard output stream, stdout. It returns the count of printed characters when the function is successful and 1 when the function fails.

The available conversion specifiers are:
%c: Prints a single character.

%d: Prints integers.

%b: Prints the binary representation of an unsigned decimal.

%x: Prints the hexadecial representation of an unsigned decimal in lowercase letters

%X:Prints the hexadecial representation of an unsigned decimal in uppercase letters

%R: Prints the Rot13 interpretation of a string

%s: Prints a string of characters.

Usage
All the files are to be compiled on Ubuntu 14.04 LTS

Include the "main.h" header file on the functions using the _printf()

Compile your code with $ gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c

Example
#include "main.h"
#include <stdio.h>
/**
* main - Entry point
*
* Return: Always 0
*/

int main(void)
{
  int a;
  int b;
  char *str;

  str = "school";
  a = _printf("%r\n", "Alx"); /*expected: xlA*/
  printf("--->%d\n", a); /*expected: 10*/

  b = _printf("%r\n", str); /*expected: loohcs*/
  printf("%d\n", b); /*expected: 7*/

  b = _printf("%r\n", str); /*expected: loohcs*/
  printf("%d\n", b); /*expected: 7*/
  return (0);
}
File Functions
_printf.c
Custom Printf Function That Performs Formatted Output Conversion And Print Data.

main.h
Header File Were All Prototypes Are Saved.

get_print_func.c
Pointer To A Function That Selects The Correct Function To Perform The Operation.

print_buf.c
Function That Prints The Buffer.

handl_buf.c
Function That Concatenates The Buffer Characters.

print_chr.c
Function That Writes The Character C To Stdout.

/* Identifier : %c */

print_str.c
Function That Writes The String To Stdout.

/* Identifier : %s */

print_int.c
Function That Prints An Integer.

/* Identifier : %i or %d */

print_bnr.c
Function That Prints Decimal In Binary.

/* Identifier : %b */

print_oct.c
Function That Prints Decimal In Octal.

/* Identifier : %o */

print_hex.c
Function That Prints Decimal In Hexadecimal.

/* Identifier : %x */

print_upx.c
Function That Prints Decimal In Uppercase Hexadecimal.

/* Identifier : %X */

print_usr.c
Function That Prints A String And Values Of Non-Printed Chars.

/* Identifier : %S */

print_unt.c
Function That Prints An Unsigned Integer.

/* Identifier : %u */

print_rev.c
Function That Writes The String To Stdout In Reverse.

/* Identifier : %r */

print_rot.c
Function That Writes The String To Stdout In Rot13.

/* Identifier : %R */

print_add.c
Function That Prints The Address Of An Input Variable.

/* Identifier : %p */

print_long_oct.c
Function That Prints Long Decimal Number In Octal.

/* Identifier : %lo */

print_long_hex.c
Function That Prints Long Decimal Number In Hexadecimal.

/* Identifier : %lx */

print_long_int.c
Function That Prints A Long Integer.

/* Identifier : %li */

print_long_upx.c
Function That Prints A Long Decimal In Uppercase Hexadecimal.

/* Identifier : %lX */

print_long_unt.c
Function That Prints A Long Unsigned Integer.

/* Identifier : %lu */

print_short_oct.c
Function That Prints Short Decimal Number In Octal.

/* Identifier : %ho */

print_short_hex.c
Function That Prints Short Decimal Number In Hexadecimal.

/* Identifier : %hx */

print_short_int.c
Function That Prints A Short Integer.

print_short_upx.c
Function That Prints A Short Decimal In Uppercase Hexadecimal.

/* Identifier : %hX */

print_short_unt.c
Function That Prints A Short Unsigned Integer.

/* Identifier : %hu */

print_num_hex.c
Function That Print A Number In Hexadecimal Begining With 0 And x.

/* Identifier : %#x */

print_num_oct.c
Function That Prints A Number In Octal Begining With 0 And o.

/* Identifier : %#o */

print_num_upx.c
Function That Prints A Number In Uppercase Hexadecimal.

/* Identifier : %#X */

print_plus_int.c
Function That Prints An Integer With Plus Symbol.

/* Identifier : %+i */

print_space_int.c
Function That Prints An Integer Begining With 0 And u.

/* Identifier : % i */

ev_print_func.c
Function That Returns The Amount Of Identifiers.

Authors
Tomisin Obijole
Wasilat Ibiyemi

End


the ALX task itself is below

0x11. C - printf
 By Julien Barbier, co-founder & CEO
 Weight: 5
 Project to be done in teams of 2 people (your team: Tomisin Obijole, Wasilat Ibiyemi
 Project over - took place from Apr 14, 2022 to Apr 20, 2022 - you're done with 150% of tasks.
 An auto review will be launched at the deadline
In a nutshell…
Contribution: 100.0%
Auto QA review: 65.65/101 mandatory & 484.9/1123 optional
Altogether:  93.07%
Mandatory: 65.0%
Optional: 43.18%
Contribution: 100.0%
Calculation:  100.0% * (65.0% + (65.0% * 43.18%) )  == 93.07%
Concepts
For this project, students are expected to look at these concepts:

Group Projects
Pair Programming - How To
Flowcharts
Technical Writing
Background Context
Write your own printf function.



^ In this picture, Kris, and Jul

Resources
Read or watch:

Secrets of printf
Group Projects concept page (Don’t forget to read this)
Flowcharts concept page
man or help:

printf (3)
Requirements
General
Allowed editors: vi, vim, emacs
All your files will be compiled on Ubuntu 20.04 LTS using gcc, using the options -Wall -Werror -Wextra -pedantic -std=gnu89
All your files should end with a new line
A README.md file, at the root of the folder of the project is mandatory
Your code should use the Betty style. It will be checked using betty-style.pl and betty-doc.pl
You are not allowed to use global variables
No more than 5 functions per file
In the following examples, the main.c files are shown as examples. You can use them to test your functions, but you don’t have to push them to your repo (if you do we won’t take them into account). We will use our own main.c files at compilation. Our main.c files might be different from the one shown in the examples
The prototypes of all your functions should be included in your header file called main.h
Don’t forget to push your header file
All your header files should be include guarded
Note that we will not provide the _putchar function for this project
GitHub
There should be one project repository per group. If you clone/fork/whatever a project repository with the same name before the second deadline, you risk a 0% score.

More Info
Authorized functions and macros
write (man 2 write)
malloc (man 3 malloc)
free (man 3 free)
va_start (man 3 va_start)
va_end (man 3 va_end)
va_copy (man 3 va_copy)
va_arg (man 3 va_arg)
Compilation
Your code will be compiled this way:
$ gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c
As a consequence, be careful not to push any c file containing a main function in the root directory of your project (you could have a test folder containing all your tests files including main functions)
Our main files will include your main header file (main.h): #include main.h
You might want to look at the gcc flag -Wno-format when testing with your _printf and the standard printf. Example of test file that you could use:
alex@ubuntu:~/c/printf$ cat main.c 
#include <limits.h>
#include <stdio.h>
#include "main.h"

/**
 * main - Entry point
 *
 * Return: Always 0
 */
int main(void)
{
    int len;
    int len2;
    unsigned int ui;
    void *addr;

    len = _printf("Let's try to printf a simple sentence.\n");
    len2 = printf("Let's try to printf a simple sentence.\n");
    ui = (unsigned int)INT_MAX + 1024;
    addr = (void *)0x7ffe637541f0;
    _printf("Length:[%d, %i]\n", len, len);
    printf("Length:[%d, %i]\n", len2, len2);
    _printf("Negative:[%d]\n", -762534);
    printf("Negative:[%d]\n", -762534);
    _printf("Unsigned:[%u]\n", ui);
    printf("Unsigned:[%u]\n", ui);
    _printf("Unsigned octal:[%o]\n", ui);
    printf("Unsigned octal:[%o]\n", ui);
    _printf("Unsigned hexadecimal:[%x, %X]\n", ui, ui);
    printf("Unsigned hexadecimal:[%x, %X]\n", ui, ui);
    _printf("Character:[%c]\n", 'H');
    printf("Character:[%c]\n", 'H');
    _printf("String:[%s]\n", "I am a string !");
    printf("String:[%s]\n", "I am a string !");
    _printf("Address:[%p]\n", addr);
    printf("Address:[%p]\n", addr);
    len = _printf("Percent:[%%]\n");
    len2 = printf("Percent:[%%]\n");
    _printf("Len:[%d]\n", len);
    printf("Len:[%d]\n", len2);
    _printf("Unknown:[%r]\n");
    printf("Unknown:[%r]\n");
    return (0);
}
alex@ubuntu:~/c/printf$ gcc -Wall -Wextra -Werror -pedantic -std=gnu89 -Wno-format *.c
alex@ubuntu:~/c/printf$ ./printf
Let's try to printf a simple sentence.
Let's try to printf a simple sentence.
Length:[39, 39]
Length:[39, 39]
Negative:[-762534]
Negative:[-762534]
Unsigned:[2147484671]
Unsigned:[2147484671]
Unsigned octal:[20000001777]
Unsigned octal:[20000001777]
Unsigned hexadecimal:[800003ff, 800003FF]
Unsigned hexadecimal:[800003ff, 800003FF]
Character:[H]
Character:[H]
String:[I am a string !]
String:[I am a string !]
Address:[0x7ffe637541f0]
Address:[0x7ffe637541f0]
Percent:[%]
Percent:[%]
Len:[12]
Len:[12]
Unknown:[%r]
Unknown:[%r]
alex@ubuntu:~/c/printf$
We strongly encourage you to work all together on a set of tests
If the task does not specify what to do with an edge case, do the same as printf
Tasks
0. I'm not going anywhere. You can print that wherever you want to. I'm here and I'm a Spur for life
mandatory
Score: 65.00% (Checks completed: 100.00%)
Write a function that produces output according to a format.

Prototype: int _printf(const char *format, ...);
Returns: the number of characters printed (excluding the null byte used to end output to strings)
write output to stdout, the standard output stream
format is a character string. The format string is composed of zero or more directives. See man 3 printf for more detail. You need to handle the following conversion specifiers:
c
s
%
You don’t have to reproduce the buffer handling of the C library printf function
You don’t have to handle the flag characters
You don’t have to handle field width
You don’t have to handle precision
You don’t have to handle the length modifiers
Repo:

GitHub repository: printf
    
1. Education is when you read the fine print. Experience is what you get if you don't
mandatory
Score: 65.00% (Checks completed: 100.00%)
Handle the following conversion specifiers:

d
i
You don’t have to handle the flag characters
You don’t have to handle field width
You don’t have to handle precision
You don’t have to handle the length modifiers
Repo:

GitHub repository: printf
    
2. With a face like mine, I do better in print
#advanced
Score: 65.00% (Checks completed: 100.00%)
Handle the following custom conversion specifiers:

b: the unsigned int argument is converted to binary
alex@ubuntu:~/c/printf$ cat main.c
#include "main.h"

/**
 * main - Entry point
 *
 * Return: Always 0
 */
int main(void)
{
    _printf("%b\n", 98);
    return (0);
}
alex@ubuntu:~/c/printf$ gcc -Wall -Wextra -Werror -pedantic -std=gnu89 main.c
alex@ubuntu:~/c/printf$ ./a.out
1100010
alex@ubuntu:~/c/printf$
Repo:

GitHub repository: printf
   
3. What one has not experienced, one will never understand in print
#advanced
Score: 65.00% (Checks completed: 100.00%)
Handle the following conversion specifiers:

u
o
x
X
You don’t have to handle the flag characters
You don’t have to handle field width
You don’t have to handle precision
You don’t have to handle the length modifiers
Repo:

GitHub repository: printf
    
4. Nothing in fine print is ever good news
#advanced
Score: 65.00% (Checks completed: 100.00%)
Use a local buffer of 1024 chars in order to call write as little as possible.

Repo:

GitHub repository: printf
    
5. My weakness is wearing too much leopard print
#advanced
Score: 65.00% (Checks completed: 100.00%)
Handle the following custom conversion specifier:

S : prints the string.
Non printable characters (0 < ASCII value < 32 or >= 127) are printed this way: \x, followed by the ASCII code value in hexadecimal (upper case - always 2 characters)
alex@ubuntu:~/c/printf$ cat main.c
#include "main.h"

/**
 * main - Entry point
 *
 * Return: Always 0
 */
int main(void)
{
    _printf("%S\n", "Best\nSchool");
    return (0);
}
alex@ubuntu:~/c/printf$ gcc -Wall -Wextra -Werror -pedantic -std=gnu89 main.c
alex@ubuntu:~/c/printf$ ./a.out
Best\x0ASchool
alex@ubuntu:~/c/printf$
Repo:

GitHub repository: printf
   
6. How is the world ruled and led to war? Diplomats lie to journalists and believe these lies when they see them in print
#advanced
Score: 65.00% (Checks completed: 100.00%)
Handle the following conversion specifier: p.

You don’t have to handle the flag characters
You don’t have to handle field width
You don’t have to handle precision
You don’t have to handle the length modifiers
Repo:

GitHub repository: printf
    
7. The big print gives and the small print takes away
#advanced
Score: 65.00% (Checks completed: 100.00%)
Handle the following flag characters for non-custom conversion specifiers:

+
space
#
Repo:

GitHub repository: printf
    
8. Sarcasm is lost in print
#advanced
Score: 65.00% (Checks completed: 100.00%)
Handle the following length modifiers for non-custom conversion specifiers:

l
h
Conversion specifiers to handle: d, i, u, o, x, X

Repo:

GitHub repository: printf
    
9. Print some money and give it to us for the rain forests
#advanced
Score: 0.00% (Checks completed: 0.00%)
Handle the field width for non-custom conversion specifiers.

Repo:

GitHub repository: printf
     
10. The negative is the equivalent of the composer's score, and the print the performance
#advanced
Score: 0.00% (Checks completed: 0.00%)
Handle the precision for non-custom conversion specifiers.

Repo:

GitHub repository: printf
     
11. It's depressing when you're still around and your albums are out of print
#advanced
Score: 0.00% (Checks completed: 0.00%)
Handle the 0 flag character for non-custom conversion specifiers.

Repo:

GitHub repository: printf
     
12. Every time that I wanted to give up, if I saw an interesting textile, print what ever, suddenly I would see a collection
#advanced
Score: 0.00% (Checks completed: 0.00%)
Handle the - flag character for non-custom conversion specifiers.

Repo:

GitHub repository: printf
     
13. Print is the sharpest and the strongest weapon of our party
#advanced
Score: 65.00% (Checks completed: 100.00%)
Handle the following custom conversion specifier:

r : prints the reversed string
Repo:

GitHub repository: printf
    
14. The flood of print has turned reading into a process of gulping rather than savoring
#advanced
Score: 65.00% (Checks completed: 100.00%)
Handle the following custom conversion specifier:

R: prints the rot13'ed string
Repo:

GitHub repository: printf
    
15. *
#advanced
Score: 31.73% (Checks completed: 48.81%)
All the above options work well together.

Repo:

GitHub repository: printf
     
Copyright © 2022 ALX, All rights reserved.
