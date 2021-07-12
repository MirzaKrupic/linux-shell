# linux-shell

Linux shell written in C programming language which has to execute all Linux shell commands

## Description

The shell should operate in this basic way: when you type in a command (in response to its prompt), the shell creates a child process that executes the command you entered and then prompts for more user input when it has finished.
Your shell can be run in two ways: interactive and batch. In interactive mode, you will display a prompt (any string of your choosing) and the user of the shell will type in a command at the prompt. In batch mode, your shell is started by specifying a batch file on its command line; the batch file contains the list of commands that should be executed. In batch mode, shell does not display a prompt. In batch mode shell echoes each line you read from the batch file back to the user before executing it; this will help you when you debug your shells (and us when we test your programs). In both interactive and batch mode, your shell stops accepting new commands when it sees the quit command on a line or reaches the end of the input stream (i.e., the end of the batch file or the user types 'Ctrl-D'). The shell should then exit after all running processes have terminated.

Each line (of the batch file or typed at the prompt) may contain multiple commands separated with the ; character. Each of the commands separated by a ; should be run simultaneously, or concurrently.

The shell should not print the next prompt or take more input until all of these commands have finished executing (the wait() and/or waitpid() system calls may be useful here).

### Executing program

* Open linux terminal
* Navigate to the folder where your script is located
* Run the gcc command on the projectShellGroup5.c in terminal: gcc -W -o shell projectShellGroup5.c -pthread
* Then run the file in the folder: ./shell
* If you want to run shell in batch mode, run ./shell <name of file including extension>
