# MyShell

MyShell is a simple interactive shell program written in C. It provides both interactive and non-interactive modes for executing commands.

## Features

- **Interactive Mode**: Run the shell without any command-line arguments to enter interactive mode. In this mode, MyShell displays a prompt ('$') and waits for the user to enter commands. It supports built-in commands such as `cd` to change directories and `exit` to quit the shell.

- **Non-Interactive Mode**: Run the shell with a command-line argument to execute a single command in non-interactive mode. This mode is useful for scripting or batch processing.

## Usage

### Interactive Mode

```bash
$ ./myshell
($) ls
file1.txt file2.txt
($) cd ..
($) exit
```
## Non Interactive Mode
$ ./myshell "ls -l"
total 8
-rw-r--r-- 1 user group 42 Jan 1 10:00 file1.txt
-rw-r--r-- 1 user group 64 Jan 1 10:01 file2.txt

## Instalation
### 1. Clone the repository
git clone https://github.com/LDtheGHOST/holbertonschool-simple_shell.git

### 2. Navigate to the project directory:
cd holbertonschool-simple_shell
### 3. Compile the program 
gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh

## Author
Wail Abou Zid, Bryan Kotro, Cuevas Luisdavid.



