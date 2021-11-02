# A repository for our simple_shell group project due 4_11_2021

* Elisa Hezikiah Dimiti
* Eyene Samuel Baker


**A simple Unix command line interpreter**
![shell](/shell.png)

****
## Table of contents
 - **What is the shell?**
 - **About this project**
 - **Essential Functionalities of the Simple Shell**
 - **File description**
 - **List of allowed functions and system calls for this project**
 - **USAGE**
 - **Example of Usage**
 - **Bugs**
 - **TEAM**
 ****

## What is the shell?
The shell is a program that takes commands from the keyboard via the terminal, and gives them to the operating system to perform.\
**To better understand how the shell actually works, you can read our [Article].**

## About this project
This project is a simple version of the linux shell made for [ALX-SE Programme] taking part of the "Low-level programming & Algorithm - Linux and Unix system programming" projects.\
It is created using the **C programming Language** and it can do many functionalities that a real shell does.

## Essential Functionalities of the Simple Shell:
> Displays a prompt "#cisfun$ " and waits for user input.\
> Runs all commands of type "executable program" (ls and /bin/ls).\
> Runs the following build_in commands: **exit**, **env**, **setenv** and **unsetenv**.\
> Handles commands with arguments.\
> Handles the PATH global variable.\
> Handles The EOF (End Of File) condition.\
> Handles the Ctrl + C signal -> It doesn't exit the shell
## Files description
 - **AUTHORS** -> List of contributors to this repository
 - **man_1_simple_shell** -> Manual page for the simple_shell
 - **shell.h** -> Header file
 - **shell.c** -> main function
        - **sig_handler** -> handles the Ctrl + C signal
        - **_EOF** -> handles the End Of File condition
 - **string.c**
        - **_putchar** -> prints a character
        - **_puts** -> prints a string
        - **_strlen** -> gives the length of a string
        - **_strdup** -> copies a string in a newly allocated memory
        - **concat_all** -> concatenates 3 strings in a newly allocated memory
 - **line_exec.c**
        - **splitstring** -> splits a string into an array of words
        - **execute** -> executes a command using execve
        - **realloc** -> reallocates a memory block
        - **freearv** -> frees a 2 dimensional array
 - **linkpath.c**
        - **_getenv** -> returns the value of a global variable
        - **add_node_end** -> adds a node in a singly linked list
        - **linkpath** -> creates a singly linked list for PATH directories
        - **_which** -> finds the pathname of a command
        - **free_list** -> frees the linked list of PATH value
 - **checkbuild.c**
        - **checkbuild** -> checks if a command is a build-in command
 - **buildin.c**
        - **exitt** -> handles the exit buildin command
        - **_atoi** -> converts a string into an integer
        - **env** -> prints the current environment
        - **_setenv** -> Initialize a new global variable, or modify an existing one
        - **_unsetenv** -> remove a global variable


