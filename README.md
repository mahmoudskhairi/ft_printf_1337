# 42 ft_printf Project

## Overview

The **`ft_printf`** project is part of the 42 School curriculum and focuses on re-implementing the well-known `printf` function from the C Standard Library. This project is designed to deepen your understanding of variadic functions, string formatting, and output management in C, providing a flexible way to format text and output it to the standard output or other streams.

---

## Key Features

- Custom implementation of a subset of the C standard `printf` function.
- Supports formatted output conversion specifiers such as:
  - **`%c`**: Print a single character.
  - **`%s`**: Print a string of characters.
  - **`%p`**: Print a pointer address.
  - **`%d` or `%i`**: Print a signed decimal integer.
  - **`%u`**: Print an unsigned decimal integer.
  - **`%x` or `%X`**: Print a hexadecimal number (lowercase and uppercase).
  - **`%%`**: Print a literal `%` sign.
  
- Handles variable arguments using the `stdarg.h` library.
- Proper management of buffer and memory to ensure correct output, even with large input.

---

## Supported Conversion Specifiers

`ft_printf` mimics the functionality of the standard `printf` but is limited to the following specifiers:

| Specifier | Description                   | Example Input | Example Output |
|-----------|-------------------------------|---------------|----------------|
| `%c`      | Character                      | `ft_printf("%c", 'A');` | A |
| `%s`      | String                         | `ft_printf("%s", "Hello");` | Hello |
| `%p`      | Pointer                        | `ft_printf("%p", ptr);` | 0x7ffee32f0a |
| `%d`/`%i` | Signed integer (decimal)       | `ft_printf("%d", 42);` | 42 |
| `%u`      | Unsigned integer               | `ft_printf("%u", 42);` | 42 |
| `%x`      | Unsigned hexadecimal (lower)   | `ft_printf("%x", 255);` | ff |
| `%X`      | Unsigned hexadecimal (upper)   | `ft_printf("%X", 255);` | FF |
| `%%`      | Percent sign                   | `ft_printf("%%");` | % |

---

## Project Structure

Here is the structure of the `ft_printf` repository:

```bash
ft_printf/
├── srcs/              # Source files for the implementation
│   ├── ft_printf.c    # Main printf logic
│   ├── ft_utils.c     # Helper functions (itoa, etc.)
│   ├── ft_parser.c    # Handles parsing of format specifiers
│   └── ft_writer.c    # Handles writing formatted output
├── includes/          # Header files
│   └── ft_printf.h    # Prototypes and macro definitions
├── Makefile           # Script to compile the library
├── README.md          # This readme file
└── tests/             # Test files for different printf cases
