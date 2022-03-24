############################### Some c library for my 42 school projects ###############################

*Note: The code is written in C language and thus needs the gcc/clang compiler and some standard C libraries to run*

# libft.a

It Uses [libft project](https://github.com/sgkhusal/42-libft) functions plus another functions developed in other 42 school projects.

## Using the library

* clone this repo: ```git clone https://github.com/sgkhusal/42-libraries.git```
* ```cd 42-libraries/libft```
* run ```make ```
* Include the header libft.h in your C projects:
```
#include "<path>/libft/src/libft.h"
```
* For compilation add ```<path>/libft/libft.a```

## Functions in the library

### [Libft](https://github.com/sgkhusal/42-libft) Functions

* ```int ft_isalpha(int c)``` - returns 1 if c is an alphabetic character and 0 if no
* ```int ft_isalnum(int c)``` - returns 1 if c is a alphanumeric character and 0 if no
* ```int ft_isascii(int c)``` - returns 1 if c is an ascii character and 0 if no
* ```int ft_isdigit(int c)``` - returns 1 if c is a number character and 0 if no
* ```int ft_isprint(int c)``` - returns 1 if c is a printable character and 0 if no

* ```char	*ft_itoa(int n)``` - returns a string to a given int number
* ```int ft_atoi(const char *nptr)``` - transforms a string of number in an int and returns the int value
* ```int ft_toupper(int c)``` - if is an alphabetic character returns the upper case character, else return the character  
* ```int ft_tolower(int c)``` - if is an alphabetic character returns the lower case character, else return the character

* ```void	ft_bzero(void *s, size_t len)``` -
* ```void	*ft_calloc(size_t nmemb, size_t size)``` -
* ```void	*ft_memset(void *buffer, int c, size_t len)``` -
* ```void	*ft_memcpy(void *dest, const void *src, size_t n)``` -
* ```void	*ft_memccpy(void *dest, const void *src, int c, size_t n)``` -
* ```void	*ft_memmove(void *dest, const void *src, size_t n)``` -
* ```void	*ft_memchr(const void *s, int c, size_t n)``` -
* ```int  ft_memcmp(const void *s1, const void *s2, size_t n)``` -

* ```void	ft_putchar_fd(char c, int fd)``` - Outputs the character ’c’ to the given file descriptor.
* ```void	ft_putstr_fd(char *s, int fd)``` - Outputs the string ’s’ to the given file descriptor.
* ```void	ft_putendl_fd(char *s, int fd)``` - - Outputs the string ’s’ to the given file descriptor, followed by a newline.
* ```void	ft_putnbr_fd(int n, int fd)``` - Outputs the integer ’n’ to the given file descriptor.

* ```size_t	ft_strlen(const char *str)``` - return the string size
* ```size_t	ft_strlcpy(char *dest, const char *src, size_t size)``` -
* ```size_t	ft_strlcat (char *dst, const char *src, size_t size)``` -
* ```char	*ft_strchr(const char *s, int c)``` -
* ```char	*ft_strrchr(const char *s, int c)``` -
* ```char	*ft_strnstr(const char *big, const char *little, size_t len)``` -
* ```int  ft_strncmp(const char *s1, const char *s2, size_t n)``` -
* ```char	*ft_strdup(const char *s)``` - duplicates the string
* ```char	**ft_strjoin(char const *s1, char const *s2)``` - concatenates two strings
* ```char	*ft_substr(char const *s, unsigned int start, size_t len)``` - returns a substring from the initial string which starts at index 'start' and is of maximum size 'len' 
* ```char	*ft_strtrim(char const *s, char const *set)``` - returns the string 's' with the characters of 'set' removed from the beginning and the end or the string
* ```char	**ft_split(char const *s, char c)``` - returns an array of strings  from the split of 's' using 'c' as the delimeter
* ```char	*ft_strmapi(char const *s, char (*f)(unsigned int, char))``` - Applies the function ’f’ to each character of the string ’s’ to create a new string (for exemple, to use the ft_toupper function in a string)

* ```t_list *ft_lstnew(void *content)``` - returns a new t_list element
* * ```int  ft_lstsize(t_list *lst)``` - returns the list size
* ```t_list *ft_lstlast(t_list *lst)``` - returns the last element from a list
* ```void	ft_lstadd_back(t_list **lst, t_list *new)``` - adds in the last positon a new t_list element in a list
* ```void	ft_lstadd_front(t_list **lst, t_list *new)``` - adds in the first positon a new t_list element in a list
* ```void	ft_lstdelone(t_list *lst, void (*del)(void *))``` - deletes de element (frees the memory from the content element and \*lst) 
* ```void	ft_lstclear(t_list **lst, void (*del)(void *))``` - deletes de element and the subsequent elements

### [Get-Next-Line](https://github.com/sgkhusal/42-GNL) Function

```int		get_next_line(int fd, char **line)``` - read from a file descriptor and returns in pointer \*\*line a new line (\n)

**Returns values:**
* 1: a line has been read
* 0: reached EOF
* -1: an error happened

# libftprintf.a

[Ft_printf](https://github.com/sgkhusal/42-ft_printf) Function

## Using the library
**Requires libft.a library

* clone this repo: ```git clone https://github.com/sgkhusal/42-libraries.git```
* ```cd 42-libraries/ft_printf```
* run ```make```
* ```cd .. && cd libft```
* run ```make```
* Include the headers libft.h and ft_printf.h in your C projects:
```
#include "<path>/ft_printf/ft_printf.h"
```
* For compilation add ```<path>/ft_printf/libftprintf.a <path>/libft/libft.a```

## Functions in the library:

* ```int		ft_printf(const char *str, ...)``` - a function that mimic the real printf
* ```int		ft_printf_fd(int fd, const char *str, ...)``` - the same as ft_printf but you can specified the file descriptor where the output should be written.

### Return values:
- number of characters writing in the stdout for `ft_printf` function
- number of characters writing in the file descriptor fd for `ft_printf_fd` function
- 0 if error

_Note: The ft_printf function outputs are according with the printf outputs for MacOS system (in Linux some outputs are different).

## Specifiers supported:
- `%c`: char
- `%s`: string
- `%p`: pointer
- `%d`: decimal signed integer
- `%i`: signed integer
- `%u`: unsigned integer
- `%x`: hexadecimal unsigned integer (lowercase)
- `%X`: hexadecimal unsigned integer (uppercase)
- `%%`: % printing

* Manage any combination of the following flags: `'-0.'` and minimum field width with all conversions
* flags - `'# +'`

### Understanding the flags:
- `number` (width): minimum number of charcters to be printed. If the value to be printed is shorter than this number,
the result is padded with blank spaces. The value is not truncated even if the result is larger
- `'-'`: left-justifies within the given field width. Right justification is the default
- `'0'`: left-pads the number with zeroes instead of spaces
- `'+'`: forces to precede the result with a plus or minus sign, even for positive numbers
- `' ' (space)`: if no sign is going to be written, a blank space is inserted before the value
- `'#'`: used x or X specifiers - the value is preceded with 0x or 0X for values different than zero

#### Precision flag: `.number`
- When no precision is specified, the default is 1.
- If the period is specified without an explicit value for precision, 0 is assumed
- For integer specifiers d, i, o, u, x and X specifies the minimum number of digits to be written. If the value to be written is shorter than this number, the result is padded with leading zeros. The value is not truncated even if the result is longer.
- A precision of 0 means that no character is written for the value of 0
- For s is the maximum number of significant digits to be printed (By default all characters are printed until the ending null character is encountered)
- For c it is has no effect
