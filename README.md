# Libft

## Overview
Libft is a personal C library containing a collection of custom-implemented functions similar to those found in standard C libraries. This project is part of the 42 School curriculum and serves as a foundation for future C programming projects.

## Description
This library is designed to recreate various standard C library functions along with additional useful functions that will be used in future 42 projects. By building this library, developers gain a deeper understanding of memory management, string manipulation, list operations, and more.

## Functions

### Libc Functions
The following functions are reimplementations of standard C library functions:

| Function | Description |
| --- | --- |
| `ft_atoi` | Converts a string to an integer |
| `ft_bzero` | Writes zeros to a byte string |
| `ft_calloc` | Allocates memory and sets it to zero |
| `ft_isalnum` | Checks if character is alphanumeric |
| `ft_isalpha` | Checks if character is alphabetic |
| `ft_isascii` | Checks if character is ASCII |
| `ft_isdigit` | Checks if character is a digit |
| `ft_isprint` | Checks if character is printable |
| `ft_memchr` | Locates byte in byte string |
| `ft_memcmp` | Compares byte string |
| `ft_memcpy` | Copies memory area |
| `ft_memmove` | Copies byte string, even if they overlap |
| `ft_memset` | Fills memory with a constant byte |
| `ft_strchr` | Locates character in string |
| `ft_strdup` | Duplicates a string |
| `ft_strlcat` | Concatenates strings with size limitation |
| `ft_strlcpy` | Copies string with size limitation |
| `ft_strlen` | Calculates the length of a string |
| `ft_strncmp` | Compares two strings |
| `ft_strnstr` | Locates a substring in a string |
| `ft_strrchr` | Locates character in string from the end |
| `ft_tolower` | Converts character to lowercase |
| `ft_toupper` | Converts character to uppercase |

### Additional Functions
These functions are not in the standard C library but are useful utilities:

| Function | Description |
| --- | --- |
| `ft_itoa` | Converts an integer to a string |
| `ft_putchar_fd` | Outputs a character to the given file descriptor |
| `ft_putendl_fd` | Outputs a string followed by a newline to the given file descriptor |
| `ft_putnbr_fd` | Outputs an integer to the given file descriptor |
| `ft_putstr_fd` | Outputs a string to the given file descriptor |
| `ft_split` | Splits a string using a delimiter character |
| `ft_strjoin` | Concatenates two strings |
| `ft_strmapi` | Applies a function to each character of a string |
| `ft_strtrim` | Trims specified characters from the beginning and end of a string |
| `ft_substr` | Returns a substring from a string |
| `ft_striteri` | Applies a function to each character of a string with its index |

### Bonus Functions (Linked List Operations)
These functions provide linked list manipulation capabilities:

| Function | Description |
| --- | --- |
| `ft_lstadd_back` | Adds a new element to the end of a list |
| `ft_lstadd_front` | Adds a new element to the beginning of a list |
| `ft_lstclear` | Deletes and frees a list |
| `ft_lstdelone` | Deletes and frees one element |
| `ft_lstiter` | Applies a function to each element of a list |
| `ft_lstlast` | Returns the last element of a list |
| `ft_lstmap` | Applies a function to each element and creates a new list |
| `ft_lstnew` | Creates a new list element |
| `ft_lstsize` | Counts the number of elements in a list |

## Usage

### Compilation
```bash
make              # Compile the library without bonus functions
make bonus        # Compile the library with bonus functions
make clean        # Remove object files
make fclean       # Remove object files and the library
make re           # Recompile the library
```

### Integration into Your Projects
To use this library in your projects:

1. Compile the library using the Makefile
2. Include the header file in your source code:
   ```c
   #include "libft.h"
   ```
3. Link the library when compiling your project:
   ```bash
   gcc your_program.c -L. -lft
   ```

## Notes
- All functions handle error cases and edge scenarios
- Memory is properly managed to avoid leaks
- The code follows the 42 Norm coding standards
