# CSE 15L Lab Report 1
### by Charan Battula A17750911

---

This lab report will describe the use cases of three commands often used in the UNIX terminal.  These commands are `cd`, `ls`, and `cat` and are used to navigate and display the various files found in a file system. 

---
## `cd` command
> the `cd` command is used to navigate the various directories that can be found in a basic file system.  Below, three examples of cd will be displayed, alongside the output with a description of it below.

#### `cd` command without any arguments
```bash
[user@sahara ~/lecture1/messages]$ cd
[user@sahara ~]$
```
- When the command was run, the working directory was `~/lecture1/messages` and after the command was run, the working directory became`~/`
- When this command is run without any arguments, the command moves the working directory to the home directory.  There will be no arguments as there is always a home directory and this command will always reach it.
- The output is not an error as shown above, the command was able to take the working directory to the home directory.

#### `cd` command with the path to a directory
```bash
[user@sahara ~]$ cd lecture1/messages/
[user@sahara ~/lecture1/messages]$ 
```
- When the command was run, the working directory was `~/`, and after the command was run, the working directory became`~/lecture1/messages`
- When this command is run with the path to a directory, the command moves the working directory to the described directory.  This would only work if that directory is inside the working directory and having no errors means that it was able to reach the directory itself as it is in the working directory.
- The output is not an error as shown above, the command was able to take the working directory to the specified directory, meaning that the directory given is found within the working directory.

#### `cd` command with the path to a file
```bash
[user@sahara ~]$ cd lecture1/messages/en-us.txt 
bash: cd: lecture1/messages/en-us.txt: Not a directory
```
- When the command was run, the working directory was `~/`, and after the command was run, the working directory stayed as `~/` due to an error
- When this command is run with the path to a file, the terminal throws an error as the command `cd` can only navigate within directories.
- The output is an error as the terminal throughs the error `Not a directory`. `cd` is a command that navigates only within directories and cannot access files.

---








