0x16. C - Simple Shell

We are assigned to come up with a simple shell that mimics the bash shell.

our shell would be called hsh

Usage: simple_shell

This project was done using C language

hsh is a simple UNIX command language that reads commands from a file or standard input and executes them.

how hsh works

it prints a prompt and waits for a command from the user
it creates a child process in which the command is checked
checks for built-ins, aliases in the PATH, and local executable programs
the child process is replaced by the command, which accepts arguments
when the command is done, the program returns to the parent process and prints the prompt
the program is ready to receive a new command

To exit: press Ctrl-D or enter "exit" (with or without a status)
it Works also in non interactive mode

compilation of files is done by

gcc -Wall -Werror -Wextra -pedantic -std=gnu89 \*.c -o hsh
