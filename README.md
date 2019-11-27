# Holberton School - Holberton Shell(hsh)

Low-level programming & Algorithm  Linux and Unix system programming
Code a simple shell for [Holberton School](https://www.holbertonschool.com/). This task integrates all the topics covered so far and forms the conclusion of the part of the course dedicated exclusively to learning C programming.

## Prerequisites

Only use this List of allowed functions and system calls :

 -   `access` (man 2 access)
 -   `chdir` (man 2 chdir)
 -   `close` (man 2 close)
 -   `closedir` (man 3 closedir)
 -   `execve` (man 2 execve)
 -   `exit` (man 3 exit)
 -   `_exit` (man 2 _exit)
 -   `fflush` (man 3 fflush)
 -   `fork` (man 2 fork)
 -   `free` (man 3 free)
 -   `getcwd` (man 3 getcwd)
 -   `getline` (man 3 getline)
 -   `isatty` (man 3 isatty)
 -   `kill` (man 2 kill)
 -   `malloc` (man 3 malloc)
 -   `open` (man 2 open)
 -   `opendir` (man 3 opendir)
 -   `perror` (man 3 perror)
 -   `read` (man 2 read)
 -   `readdir` (man 3 readdir)
 -   `signal` (man 2 signal)
 -   `stat` (__xstat) (man 2 stat)
 -   `lstat` (__lxstat) (man 2 lstat)
 -   `fstat` (__fxstat) (man 2 fstat)
 -   `strtok` (man 3 strtok)
 -   `wait` (man 2 wait)
 -   `waitpid` (man 2 waitpid)
 -   `wait3` (man 2 wait3)
 -   `wait4` (man 2 wait4)
 -   `write` (man 2 write)



### Installing

	Your shell will be compiled this way:


	gcc -Wall -Wextra -Werror -pedantic -g *.c -o hsh


	-   Where the gcc is the compiler used to compile the program.
	-   The `-g` and `--debug` flag is for show all the descriptions in debug format.
	-   The flags `-Wall -Werror -Wextra -pedantic` show all warnings treat as an error.
	-   The "`*.c`" means that all the files with .c extention will be compiled.
	-   The `-o` flag is used for the output file direction.

----------

### How to use

	-   You need to include the shell.h local library or header file.
	-   After the compilation process use the excecutable command: `./hsh` and click on enter "`\n`".
	-   If you want to verify the free() process in the shell I recommend to use valgrind and the executable

	------

## Description of File Structure
	In the present shell is posible to use common commands like:

	| command | Meaning |
	|--|--|
	|**`ls`**  | List the file in PATH (It's possible to use the flags) |
	|**`pwd`**  | Print the current directory |
	| **`env`** | Print the environment |
	| **`echo`** | Print the next argument after write the echo command |
	| **`exit`** | Close the shell in a correct end process |


## TODO

### Mandatory

	-   `EOF` / end-of-file?
	-  handle arguments for the built-in `exit`` -- Currently, if the first 4 characters of the string are `exit`, the shell will exit. 
	- Handle command lines with arguments
	-   Handle the `PATH`
	-   Implement the `env` **built-in**

### Advanced

	-   `exit` handles arguments to exit -- What is `exit status`?

	-   Catch `^C` (CTRL + C) -- Find the signal and change its behavior.
	-   Handle `;`
	-   Handle `&&`, and `||`
	-   Handle `#` Comments

#### Recreate standard library functions

	-   getline
	-   strtok
	-   setenv
	-   unsetenv

#### Shell Builtins

	-   register builtins before executing commands
	-   cd
	-   alias
	-   help
	-   history
	-   Deal with variables
	-   File as input


## Authors

	-   **Lafine Sami** [LinkedIn](https://www.linkedin.com/in/sami-lafine-374b2320/) || [Twitter](https://twitter.com/AfineSami)
	-  **Mohamed Mehdi Bouchoucha** [LinkedIn](https://www.linkedin.com) || [Twitter](https://twitter.com/MMBouchoucha)
