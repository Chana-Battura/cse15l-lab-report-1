# CSE 15L Lab Report 1
### by Charan Battula A17750911

---

This lab report will describe the use cases of three commands often used in the UNIX terminal.  These commands are `cd`, `ls`, and `cat` and are used to navigate and display the various files found in a file system. 

---
## `cd` command
> the `cd` command is used to navigate the various directories that can be found in a basic file system.  Below, three examples of `cd` will be displayed, alongside the output with a description of it below.

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

## `ls` command
> the `ls` command lists out the directories and files in the working directory.  Below, three examples of `cd` will be displayed, alongside the output with a description of it below.

#### `ls` command without any arguments
```
[user@sahara ~/lecture1]$ ls
Hello.class  Hello.java messages README
```
- When the command was run, the working directory was `~/lecture1` and after the command was run, the working directory stayed `~/lecture1` but lists out the directories and files in the directory.
- When this command is run without any arguments, the command lists out all of the directories and files in the directory itself.  The directories found in the working directory are listed as bold while the files are listed regularly 
- The output is not an error as shown above, the command was able to list all the files and directories found in the working directory.
- *It is important to note that **`messages`** was bold in the terminal and for formatting reasons couldn't be bold in the code block above.*

#### `ls` command with the path to a directory
```bash
[user@sahara ~]$ ls lecture1/
Hello.class  Hello.java  messages  README
```
- When the command was run, the working directory was `~/` and after the command was run, the working directory stayed `~/` but listed out the directories and files in the directory specified.
- When this command is run with the path to a directory, the command lists all the files and directories in the specified directory.  The directories found in the working directory are listed as bold while the files are listed regularly
- The output is not an error as shown above, the command was able to list all the files and directories found in `lecture1\`.
- *It is important to note that **`messages`** was bold in the terminal and for formatting reasons couldn't be bold in the code block above.*

#### `ls` command with the path to a file
```bash
[user@sahara ~]$ ls lecture1/messages/en-us.txt 
lecture1/messages/en-us.txt
```
- When the command was run, the working directory was `~/`, and after the command was run, the working directory stayed as `~/` and instead listed the path to the file itself.
- When this command is run with the path to a file, the command `ls`, does not have a directory to list out files and directories simply lists out the path of the file specified.
- The output is not an error as shown above, the command was able to list the path of the file itself

---









