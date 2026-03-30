# pipex

## Description

pipex is a project that recreates the behavior of UNIX pipes in C.

The program simulates the shell command:
`< file1 cmd1 | cmd2 > file2`

It takes an input file, executes two commands where the output of the first command is passed as input to the second through a pipe, and writes the final result to an output file.

This project focuses on process creation and communication using system calls such as `fork`, `pipe`, `dup2`, and `execve`, as well as proper file descriptor management and error handling.
