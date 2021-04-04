# 0x16. C - Simple Shell Project

Write a simple UNIX command interpreter.

[Holberton Group Project](https://intranet.hbtn.io/projects/235#task-1054)

![GitHub Logo](https://raw.githubusercontent.com/kaustubhhiware/Cshell/master/images/Cshell_about.png)


## Motivation

A Unix shell or command-line interpreter provides a command line user interface for Unix-like operating systems.
The shell is both an interactive command language and a scripting language, and is used by the operating system
to control the execution of the system using shell scripts. Read more about the Shell, [here](https://en.wikipedia.org/wiki/Unix_shell).

## Compilation

All code will be compiled this way:

```bash
gcc -Wall -Werror -Wextra -pedantic *.c -o hsh
```
## List of allowed functions and system calls

* access (man 2 access)
* chdir (man 2 chdir)
* close (man 2 close)
* closedir (man 3 closedir)
* execve (man 2 execve)
* exit (man 3 exit)
* _exit (man 2 _exit)
* fflush (man 3 fflush)
* fork (man 2 fork)
* free (man 3 free)
* getcwd (man 3 getcwd)
* getline (man 3 getline)
* isatty (man 3 isatty)
* kill (man 2 kill)
* malloc (man 3 malloc)
* open (man 2 open)
* opendir (man 3 opendir)
* perror (man 3 perror)
* read (man 2 read)
* readdir (man 3 readdir)
* signal (man 2 signal)
* stat (__xstat) (man 2 stat)
* lstat (__lxstat) (man 2 lstat)
* fstat (__fxstat) (man 2 fstat)
* strtok (man 3 strtok)
* wait (man 2 wait)
* waitpid (man 2 waitpid)
* wait3 (man 2 wait3)
* wait4 (man 2 wait4)
* write (man 2 write)

## Code Style

Our Shell will follow Betty guidelines. Betty is a Holberton Style C code checker written in Perl.
You can find the documentation [here](https://github.com/holbertonschool/Betty).

## Mandatory Tasks

0. Write a README, a man page for your shell, and AUTHORS file at the root of your repository.
1. Write a beautiful code that passes the Betty checks.
2. Write a UNIX command line interpreter.
3. Handle command lines with arguments.
4. Handle the PATH.
5. Implement the exit built-in, that exits the shell, you dont have to handle any argument to the built-in exit.
6. Implement the env built-in, that prints the current environment.
7. Write a blog post describing step by step what happens when you type ls -l and hit Enter in a shell. Try to explain every step you know of, going in as much details as you can, give examples and draw diagrams when needed. You should merge your previous knowledge of the shell with the specifics of how it works under the hoods (including syscalls). Blog post will be hosted on Medium, under user @2372!

## Testing

Our Shell can be tested in two modes. Either interactive or non-interactive mode.

### Interactive:

```
$ ./hsh
($) /bin/ls
hsh main.c shell.c
($)
($) exit
$
```
### Non-Interactive:

```
$ echo "/bin/ls" | ./hsh
hsh main.c shell.c test_ls_2
$
$ cat test_ls_2
/bin/ls
/bin/ls
$
$ cat test_ls_2 | ./hsh
hsh main.c shell.c test_ls_2
hsh main.c shell.c test_ls_2
$
```

## Troubleshooting

For help using our Shell or to report any bugs, you may contact:
1. **Lauren Dobratz** - 2316@holbertonschool.com
2. **Bree Browder** - 2372@holbertonschool.com

## Contributors
Lauren Dobratz and Bree Browder
