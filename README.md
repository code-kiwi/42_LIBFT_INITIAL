![C](https://img.shields.io/badge/c-%2300599C.svg?style=for-the-badge&logo=c&logoColor=white)
# LIBFT (42 initial project)

> **Note:** This is a project from **42 learning cursus**.<br>
> This the original libft project, I made [another repository](https://github.com/code-kiwi/42_LIBFT) in order to have a modified libft, evolving all along the 42 cursus.

## Description
The 42 cursus teaches us programming from scratch. Most of the time, we have to code our own tools instead of using existing ones.<br>
For C progamming, we are not allowed to use functions from libraries (there are a few exceptions like `malloc`, `free`, `read`, `write`, etc.) but we are invited to code the tools we need.<br>
The libft project aims to give us a basic library with a lot of useful functions. Thanks to this library, we all have common tools to start with good foundations.<br>
This project is also the first project of our cursus, giving us the opportunity to practice programming after the piscine, instead of starting off with something difficult.

## Library content
|FUNCTION          |C equivalent   |DESCRIPTION                                                                                                                                                                                                           |
|------------------|---------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|`ft_isalpha`      |`isalpha`      |See official man
|`ft_isdigit`      |`isdigit`      |See official man
|`ft_isalnum`      |`isalnum`      |See official man
|`ft_isascii`      |`isascii`      |See official man
|`ft_isprint`      |`isprint`      |See official man
|`ft_strlen`       |`strlen`       |See official man
|`ft_memset`       |`memset`       |See official man
|`ft_bzero`        |`bzero`        |See official man
|`ft_memcpy`       |`memcpy`       |See official man
|`ft_memmove`      |`memmove`      |See official man
|`ft_strlcpy`      |`strlcpy`      |See official man
|`ft_strlcat`      |`strlcat`      |See official man
|`ft_toupper`      |`toupper`      |See official man
|`ft_tolower`      |`tolower`      |See official man
|`ft_strchr`       |`strchr`       |See official man
|`ft_strrchr`      |`strrchr`      |See official man
|`ft_strncmp`      |`strncmp`      |See official man
|`ft_memchr`       |`memchr`       |See official man
|`ft_memcmp`       |`memcmp`       |See official man
|`ft_strnstr`      |`strnstr`      |See official man
|`ft_atoi`         |`atoi`         |See official man
|`ft_calloc`       |`calloc`       |The calloc() function shall allocate unused space for an array of nelem elements each of whose size in bytes is elsize.  The space shall be initialized to all bits 0.
|`ft_strdup`       |`strdup`       |The strdup() function returns a pointer to a new string which is a duplicate of the string s.  Memory for the new string is obtained with malloc(3), and can be freed with free(3).
|`ft_substr`       |None           |Allocates (with malloc(3)) and returns a substring from the string ’s’. The substring begins at index ’start’ and is of maximum size ’len’.
|`ft_strjoin`      |None           |Allocates (with malloc(3)) and returns a new string, which is the result of the concatenation of ’s1’ and ’s2’.
|`ft_strtrim`      |None           |Allocates (with malloc(3)) and returns a copy of ’s1’ with the characters specified in ’set’ removed from the beginning and the end of the string.
|`ft_split`        |None           |Allocates (with malloc(3)) and returns an array of strings obtained by splitting ’s’ using the character ’c’ as a delimiter. The array must end with a NULL pointer.
|`ft_itoa`         |None           |Allocates (with malloc(3)) and returns a string representing the integer received as an argument. Negative numbers must be handled.
|`ft_strmapi`      |None           |Applies the function ’f’ to each character of the string ’s’, and passing its index as first argument to create a new string (with malloc(3)) resulting from successive applications of ’f’.
|`ft_striteri`     |None           |Applies the function ’f’ on each character of the string passed as argument, passing its index as first argument. Each character is passed by address to ’f’ to be modified if necessary.
|`ft_putchar_fd`   |None           |Outputs the character ’c’ to the given file descriptor.
|`ft_putstr_fd`    |None           |Outputs the string ’s’ to the given file descriptor.
|`ft_putendl_fd`   |None           |Outputs the string ’s’ to the given file descriptor followed by a newline.
|`ft_putnbr_fd`    |None           |Outputs the integer ’n’ to the given file descriptor.
|`ft_lstnew`       |None           |Allocates (with malloc(3)) and returns a new node. The member variable ’content’ is initialized with the value of the parameter ’content’. The variable ’next’ is initialized to NULL.
|`ft_lstadd_front` |None           |Adds the node ’new’ at the beginning of the list.
|`ft_lstsize`      |None           |Counts the number of nodes in a list.
|`ft_lstlast`      |None           |Returns the last node of the list.
|`ft_lstadd_back`  |None           |Adds the node ’new’ at the end of the list.
|`ft_lstdelone`    |None           |Takes as a parameter a node and frees the memory of the node’s content using the function ’del’ given as a parameter and free the node. The memory of ’next’ must not be freed.
|`ft_lstclear`     |None           |Deletes and frees the given node and every successor of that node, using the function ’del’ and free(3). Finally, the pointer to the list must be set to NULL.
|`ft_lstiter`      |None           |Iterates the list ’lst’ and applies the function ’f’ on the content of each node.
|`ft_lstmap`       |None           |Iterates the list ’lst’ and applies the function ’f’ on the content of each node. Creates a new list resulting of the successive applications of the function ’f’. The ’del’ function is used to delete the content of a node if needed.|


## Setup instructions
1. Clone the repo: `https://github.com/code-kiwi/42_LIBFT_INITIAL`
2. Compile the project `make`
The libft archive `libft.a`is created and can be used from any project
> **Note:** Some functions are part of the bonus subject. In order to copile them, use `make bonus`.

## How to use the library ?
Just import the `libft.a` archive into a C project and use the flags `-L<PATH TO THE ARCHIVE> -lft` with your compiler command in order to use the library functions.

## Testing
I made a "naive" testing program. This was a first attempt to write unit tests.<br>
Just copy a libft folder into the TEST folder, calling it `libft/`<br>
Then, use `make` to create the testing program with the libft of your choice.<br>
Some functions are not tested yet (by the testing program I wrote.<br>
In order to check if the libft is working, there are cool testing tools online like [this one](https://github.com/Tripouille/libftTester) by [Tripouille](https://github.com/Tripouille).<br>
There are a lot of edge cases and online testers are really useful in order to validate the libft project.

## Grade
![LIBFT](https://github.com/ayogun/42-project-badges/blob/main/badges/libftm.png)<br><br>
`125/125`<br>

## Credits
The badge comes from [this repo](https://github.com/ayogun/42-project-badges/tree/main), by [@ayogun](https://github.com/ayogun) which proposes a lot of amazing badges for 42 projects.
