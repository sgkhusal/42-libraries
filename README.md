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

* ```int ft_atoi(const char *nptr)```: 
* ```int ft_isalpha(int c)```: returns 1 if c is an alphabetic character and 0 if no
* ```int ft_isdigit(int c)```: returns 1 if c is a number character and 0 if no
* ```int ft_isalnum(int c)```: returns 1 if c is a alphanumeric character and 0 if no
* ```int ft_isascii(int c)```: returns 1 if c is an ascii character and 0 if no
* ```int ft_isprint(int c)```: returns 1 if c is a printable character and 0 if no
* ```int ft_toupper(int c)```: if is an alphabetic character returns the upper case character, else return the character  
* ```int ft_tolower(int c)```: if is an alphabetic character returns the lower case character, else return the character
* ```void	ft_bzero(void *s, size_t len)```:
* ```void	*ft_memset(void *buffer, int c, size_t len)```:
* ```void	*ft_memcpy(void *dest, const void *src, size_t n)```:
* ```void	*ft_memccpy(void *dest, const void *src, int c, size_t n)```:
* ```void	*ft_memmove(void *dest, const void *src, size_t n)```:
* ```void	*ft_memchr(const void *s, int c, size_t n)```:
* ```int  ft_memcmp(const void *s1, const void *s2, size_t n)```:
* ```size_t	ft_strlen(const char *str)```: return the string size
* ```size_t	ft_strlcpy(char *dest, const char *src, size_t size)```:
* ```size_t	ft_strlcat (char *dst, const char *src, size_t size)```:
* ```char	*ft_strchr(const char *s, int c)```:
* ```char	*ft_strrchr(const char *s, int c)```:
* ```char	*ft_strnstr(const char *big, const char *little, size_t len)```:

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

