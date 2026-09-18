# C-Basics.md

## 1. Data Types

| Data Type | Description |
|-----------|-------------|
| `int`     | Stores whole numbers (integers), typically 4 bytes. |
| `float`   | Stores single-precision floating-point (decimal) numbers, typically 4 bytes. |
| `double`  | Stores double-precision floating-point numbers, typically 8 bytes, more accurate than `float`. |
| `char`    | Stores a single character, 1 byte. |
| `bool`    | Stores a boolean value (`true`/`false`), from `<stdbool.h>`. |
| `void`    | Represents "no type" — used for functions that return nothing or generic pointers. |

## 2. Format Specifiers

| Specifier | Meaning |
|-----------|---------|
| `%d`  | Signed decimal integer |
| `%u`  | Unsigned decimal integer |
| `%o`  | Unsigned octal integer |
| `%x`  | Unsigned hexadecimal integer (lowercase) |
| `%X`  | Unsigned hexadecimal integer (uppercase) |
| `%f`  | Floating-point number (decimal notation) |
| `%e`  | Floating-point number (scientific/exponential notation) |
| `%c`  | Single character |
| `%s`  | String of characters |
| `%ld` | Long signed decimal integer |

## 3. Input/Output Functions

- **`scanf()`** — Reads formatted input from the keyboard based on a format
  string (e.g., `scanf("%d", &num)`), matching each specifier to a variable.
- **`printf()`** — Writes formatted output to the screen based on a format
  string, substituting values for specifiers.
- **`getchar()`** — Reads a single character from standard input and returns
  it as an `int`.
- **`putchar()`** — Writes a single character to standard output.
- **`fgets()`** — Reads a line of text (including spaces) into a character
  array, safely limiting the number of characters read to avoid buffer
  overflow.
- **`puts()`** — Writes a string to standard output followed by a newline.

## 4. Escape Sequences

| Sequence | Meaning |
|----------|---------|
| `\n` | Newline — moves the cursor to the next line |
| `\t` | Horizontal tab |
| `\\` | Backslash character |
| `\"` | Double-quote character |
| `\'` | Single-quote character |

Example:
```
printf("Name:\tAli\nCity:\tLahore\n");
```

## 5. Precision

Precision for floating-point output is specified by placing a period and a
number between the `%` and the conversion character, e.g. `%.2f` prints two
digits after the decimal point, `%.4f` prints four digits, and so on. Without
an explicit precision, `%f` defaults to six digits after the decimal point.

Example:
```
printf("%.2f\n", 3.14159);   // prints 3.14
printf("%.4f\n", 3.14159);   // prints 3.1416
```
