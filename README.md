# libft
A c library for my 42 school projects

# ***********Still in construction ******************

It Uses [libft project](https://github.com/sgkhusal/42-libft) functions plus another functions developed in other 42 school projects.

## Using the library

* clone this repo
* run ```make ```
* Include the library libft.h in your C projects:
```
#include "libft.h"
```
* During compilation use ```path-libft/libft.a```

## Functions in the library

### [Libft](https://github.com/sgkhusal/42-libft) Functions

* ```int ft_atoi(const char *nptr)```: transforms a string of number in an int and returns the int value
* ```char	*ft_itoa(int n)```: returns a string to a given int number
* ```int ft_isalpha(int c)```: returns 1 if c is an alphabetic character and 0 if no
* ```int ft_isdigit(int c)```: returns 1 if c is a number character and 0 if no
* ```int ft_isalnum(int c)```: returns 1 if c is a alphanumeric character and 0 if no
* ```int ft_isascii(int c)```: returns 1 if c is an ascii character and 0 if no
* ```int ft_isprint(int c)```: returns 1 if c is a printable character and 0 if no
* ```int ft_toupper(int c)```: if is an alphabetic character returns the upper case character, else return the character  
* ```int ft_tolower(int c)```: if is an alphabetic character returns the lower case character, else return the character
* ```void	ft_bzero(void *s, size_t len)```:
* ```void	*ft_calloc(size_t nmemb, size_t size)```:
* ```void	*ft_memset(void *buffer, int c, size_t len)```:
* ```void	*ft_memcpy(void *dest, const void *src, size_t n)```:
* ```void	*ft_memccpy(void *dest, const void *src, int c, size_t n)```:
* ```void	*ft_memmove(void *dest, const void *src, size_t n)```:
* ```void	*ft_memchr(const void *s, int c, size_t n)```:
* ```int  ft_memcmp(const void *s1, const void *s2, size_t n)```:
* ```void	ft_putchar_fd(char c, int fd)```: Outputs the character ’c’ to the given file descriptor.
* ```void	ft_putstr_fd(char *s, int fd)```: Outputs the string ’s’ to the given file descriptor.
* ```void	ft_putendl_fd(char *s, int fd)```: Outputs the string ’s’ to the given file
descriptor, followed by a newline.
* ```void	ft_putnbr_fd(int n, int fd)```: Outputs the integer ’n’ to the given file
descriptor.
* ```size_t	ft_strlen(const char *str)```: return the string size
* ```size_t	ft_strlcpy(char *dest, const char *src, size_t size)```:
* ```size_t	ft_strlcat (char *dst, const char *src, size_t size)```:
* ```char	*ft_strchr(const char *s, int c)```:
* ```char	*ft_strrchr(const char *s, int c)```:
* ```char	*ft_strnstr(const char *big, const char *little, size_t len)```:
* ```int  ft_strncmp(const char *s1, const char *s2, size_t n)```:
* ```char	*ft_strdup(const char *s)```: duplicates the string
* ```char	**ft_strjoin(char const *s1, char const *s2)```: concatenates two strings
* ```char	*ft_substr(char const *s, unsigned int start, size_t len)```: returns a substring from the initial string which starts at index 'start' and is of maximum size 'len' 
* ```char	*ft_strtrim(char const *s, char const *set)```: returns the string 's' with the characters of 'set' removed from the beginning and the end or the string
* ```char	**ft_split(char const *s, char c)```: returns an array of strings  from the split of 's' using 'c' as the delimeter
* ```char	*ft_strmapi(char const *s, char (*f)(unsigned int, char))```: Applies the function ’f’ to each character of the string ’s’ to create a new string (for exemple, to use the ft_toupper function in a string)

#### Bonus functions:

* ```t_list *ft_lstnew(void *content)```: returns a new t_list element
* * ```int  ft_lstsize(t_list *lst)```: returns the list size
* ```t_list *ft_lstlast(t_list *lst)```: returns the last element from a list
* ```void	ft_lstadd_back(t_list **lst, t_list *new)```: adds in the last positon a new t_list element in a list
* ```void	ft_lstadd_front(t_list **lst, t_list *new)```: adds in the first positon a new t_list element in a list
* ```void	ft_lstdelone(t_list *lst, void (*del)(void *))```: deletes de element (frees the memory from the content element and \*lst) 
* ```void	ft_lstclear(t_list **lst, void (*del)(void *))```: deletes de element and the subsequent elements

### [Get-Next-Line](https://github.com/sgkhusal/42-GNL) Function


### [Ft_printf](https://github.com/sgkhusal/42-ft_printf) Function

