# libft42

```
 _  _  _       __  _     __ _    ___
| |(_)| |__   / _|| |_  / _| |_ |__ \
| || || '_ \ |  _||  _||  _||  _| /_/
|_||_||_.__/ |_|   \__||_|   \__||_|
```

> *The foundation of everything. 35 functions. Zero dependencies. Pure C.*

[![42 School](https://img.shields.io/badge/42-School-000000?style=flat-square&logo=42&logoColor=white)](https://42.fr)
![C](https://img.shields.io/badge/C-99-blue?style=flat-square&logo=c&logoColor=white)
![Functions](https://img.shields.io/badge/functions-35-orange?style=flat-square)

---

## About

The very first project at 42 School. **libft42** is a from-scratch reimplementation of 35 essential libc functions in C. No shortcuts, no external libraries â just you, a compiler, and the man pages.

Every 42 student's journey begins here. This library becomes the backbone of every project that follows.

## Functions

```
 CHAR CHECK       MEMORY             STRINGS            OUTPUT
 ââââââââââââ    ââââââââââââââââ    ââââââââââââââââ    âââââââââââââââ
 ft_isalpha      ft_memset          ft_strlen           ft_putchar_fd
 ft_isdigit      ft_bzero           ft_strchr           ft_putstr_fd
 ft_isalnum      ft_memcpy          ft_strrchr          ft_putendl_fd
 ft_isascii      ft_memmove         ft_strncmp          ft_putnbr_fd
 ft_isprint      ft_memchr          ft_strlcpy
                 ft_memcmp          ft_strlcat
 CONVERSION      ft_calloc          ft_strdup            ADDITIONAL
 ââââââââââââ                       ft_strnstr           âââââââââââââââ
 ft_atoi                            ft_substr            ft_split
 ft_itoa                            ft_strjoin           ft_strmapi
 ft_toupper                         ft_strtrim           ft_striteri
 ft_tolower
```

## Build

```bash
make        # Build libft.a
make clean  # Clean object files
make fclean # Full clean
make re     # Rebuild
```

## Usage

```c
#include "libft.h"

int main(void)
{
    char **words = ft_split("Hello 42 World", ' ');
    int i = 0;
    while (words[i])
        ft_putendl_fd(words[i++], 1);
    return (0);
}
```

```bash
cc main.c -L. -lft -o program
./program
```

---

*The first brick in the wall. â 42 School*
