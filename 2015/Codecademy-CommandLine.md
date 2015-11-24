# Codecademy: Learn the Command Line

<img src="https://cdn-production.codecademy.com/assets/logo/logo--dark-blue-ac069c03cf75e3cb300995028104f92e.svg" width="100" height="25">  Learn how to use the command line to manipulate data and automate tasks

# Navigate the File System
A filesystem organizes a computer's files and directories into a tree structure. It starts with the root directory.

Each parent directory can contain more child directories and files. From the command line, you can navigate through files and folders on your computer, such as:

## Print Working Directory (pwd)
Print the current/active directory:  
`$ pwd`

## List files
List all files in the current/active directory:  
`$ ls`

## Change Directory
Change the current/active directory:  
`$ cd <directory-name>`

## Make a directory (folder)
Create a folder within the current/active directory:  
`$ mkdir <directory-name>`

## Create a new file
Create a new file within the current/active directory:  
`$ touch <file-name.ext>`

# Manipulation
Copy, move, and delete files and directories from the command line.

## Options  
The `ls` command lists all files and directories in the working directory.

The `-a` is called an option. Options modify the behavior of commands. Here we used `ls -a` to display the contents of the working directory in more detail.

In addition to using each option separately, like `ls -a `or `ls -l`, multiple options can be used together. For example, `ls -alt` lists all contents, including hidden files and directories, in long format, ordered by the date and time they were last modified.

## Common Options
### 1. List all contents (`-a`)
List all contents, including hidden files and directories.

The `-a` modifies the behavior of the `ls` command to *also list the files and directories starting with a dot `.`*. Files started with a dot are hidden, and don't appear when using `ls` alone.

### 2. List long form of contents (`-l`)
List of all contents (files and directories) of a directory in a long format, as a table with the following properties:
* **Access rights**: These are actions that are permitted on a file or directory.
* **Number of hard links**: This number counts the number of child directories and files. This number includes the parent directory link (..) and current directory link (.).
* **File owner username**: Here the username is cc.
* **Group that owns the file**: Here the group name is `eng`.
* **Size of the file** in bytes.
* **The last modified date & time** of the file.
* **The name of the file or directory**.

### 3. Order by modified date (`-t`)
Order files and directories by the time they were last modified.

## Copy
The `cp` command copies files.  

### 1. Single file
The `cp` command copies files or directories. Here, we copy the contents of frida.txt into lincoln.txt.

For example:  
`$ cp <existing-file-name.ext> <new-file-name.ext>`

### 2. Single file to a different directory
To copy a file into a directory, use cp with the source file as the first argument and the destination directory as the second argument. Here, we copy the file biopic/cleopatra.txt and place it in the historical/ directory.

For example:  
`$ cp biopic/ray.txt biopic/notorious.txt historical/`

### 3. Multiple Files
To copy multiple files into a directory, use cp with a list of source files as the first arguments, and the destination directory as the last argument. Here, we copy the files biopic/ray.txt and biopic/notorious.txt into the historical/ directory.

For example:  
`$ cp biopic/ray.txt biopic/notorious.txt historical/`

### 4. Using wildcards
In addition to using filenames as arguments, we can use special characters like `*` to select groups of files. These special characters are called wildcards. The `*` selects all files in the working directory, so here we use cp to copy all files into the satire/ directory.

For example:  
`$ cp * satire/`

### 5. Advanced wildcards
Here, `m*.txt` selects all files in the working directory starting with "m" and ending with ".txt", and copies them to scifi/.

For example:  
`cp m*.txt scifi/`

## Move
The `mv` command moves files. It's similar to `cp` in its usage.

### 1. Single file into a directory
To move a file into a directory, use `mv` with the source file as the first argument and the destination directory as the second argument. Here we move superman.txt into superhero/.

For example:  
`mv superman.txt superhero/`

### 2. Multiple files into a directory
To move multiple files into a directory, use `mv` with a list of source files as the first arguments, and the destination directory as the last argument. Here, we move wonderwoman.txt and batman.txt into superhero/.

For example:  
`mv wonderwoman.txt batman.txt superhero/`

## 3. Move and rename a file
To rename a file, use mv with the old file as the first argument and the new file as the second argument. By moving batman.txt into spiderman.txt, we rename the file as spiderman.txt.

For example:  
`mv batman.txt spiderman.txt`

## Remove
The `rm` command moves files. It's similar to `cp` in its usage. Be careful when you use `rm`! It **deletes files and directories permanently**. There isn't an undelete command, so once you delete a file or directory with rm, it's gone.

### 1. Remove a file
The `rm` command deletes files and directories. Here we remove the file waterboy.txt from the filesystem.

For example:  
`rm waterboy.txt`

### 2. Remove a directory
The `-r `is an option that modifies the behavior of the `rm` command. The `-r` stands for "recursive," and it's used to **delete a directory and all of its child directories.**

For example:  
`rm -r comedy`

# Redirection
Through redirection you can direct the input and output of a command to and from other files and programs, and chain commands together in a pipeline.  

Redirection re-routes standard input, standard output, and standard error to or from a different location.

## Standard input (`stdin`)
The information inputted into the terminal through the keyboard or input device.

The echo command accepts the string "Hello" as standard input, and echoes the string "Hello" back to the terminal as standard output. For example:  
`$ echo "Hello"
Hello`

## Standard output (`stdout`)
The information outputted after a process is run.

### 1. Copy content from the command line
The `>` command redirects the standard output to a file. Here, "Hello" is entered as the standard input. The standard output "Hello" is redirected by `>` to the file hello.txt. For example:  
`$ echo "Hello" > hello.txt`

### 2. Display contents
The `cat` command outputs the contents of a file to the terminal. When you type cat hello.txt, the contents of hello.txt are displayed. For example:  
`$ cat hello.txt`

### 3. Copy data from a file
`>` takes the standard output of the command on the left, and redirects it to the file on the right. Here the standard output of cat oceans.txt is redirected to continents.txt. Note that `>` overwrites all original content in continents.txt. When you view the output data by typing cat on continents.txt, you will see only the contents of oceans.txt. For example:  
`$ cat oceans.txt > continents.txt`

### 4. Append data
`>>` takes the standard output of the command on the left and appends (adds) it to the file on the right. You can view the output data of the file with cat and the filename.

Here, the the output data of rivers.txt will contain the original contents of rivers.txt with the content of glaciers.txt appended to it. For example:  
`$ cat glaciers.txt >> rivers.txt`

### 5. Input data into a program  
`<` takes the standard input from the file on the right and inputs it into the program on the left. Here, lakes.txt is the standard input for the cat command. The standard output appears in the terminal. For example:  
`$ cat < lakes.txt`  

### 6. Piping (`|`)
The `|` takes the standard output of the command on the left, and pipes it as standard input to the command on the right. You can think of this as "command to command" redirection.

Here the output of `cat` volcanoes.txt is the standard input of `wc`. In turn, the `wc` command outputs the number of lines, words, and characters in volcanoes.txt, respectively. For example:  
`$ cat volcanoes.txt | wc`

Multiple `|`s can be chained together. Here the standard output of cat volcanoes.txt is "piped" to the `wc` command. The standard output of w`c` is then "piped" to `cat`. Finally, the standard output of `cat` is redirected to islands.txt.

You can view the output data of this chain by typing cat islands.txt.
`$ cat volcanoes.txt | wc | cat > islands.txt`

### 7. Sorting (`sort`)
Take the standard input and orders it alphabetically for the standard output. Here, the lakes in sort lakes.txt are listed in alphabetical order. For example:  
`$ sort lakes.txt`  

Here, the command takes the standard output from cat lakes.txt and "pipes" it to sort. The standard output of sort is redirected to sorted-lakes.txt. For examples, you can view the output data by typing cat on the file sorted-lakes.txt:  
`$ cat lakes.txt | sort > sorted-lakes.txt`

### 8. Unique (`uniq`)
Filter out adjacent, duplicate lines in a file. Here `uniq` deserts.txt filters out duplicates of "Sahara Desert", because the duplicate of 'Sahara Desert' directly follows the previous instance. The "Kalahari Desert" duplicates are not adjacent, and thus remain:
`$ uniq deserts.txt`

A more effective way to call uniq is to call sort to alphabetize a file, and "pipe" the standard output to uniq. Here by piping sort deserts.txt to uniq, all duplicate lines are alphabetized (and thereby made adjacent) and filtered out:  
`$ sort deserts.txt | uniq`

Here we simply send filtered contents to uniq-deserts.txt, which you can view with the cat command:  
`sort deserts.txt | uniq > uniq-deserts.txt`

### 9. Global Regular Expression Print (`grep`)
Searches files for lines that match a pattern and returns the results. It is also case sensitive. Here, grep searches for "Mount" in mountains.txt:  
`$ grep Mount mountains.txt`  

`grep -i` enables the command to be *case insensitive*. Here, `grep` searches for capital or lowercase strings that match Mount in mountains.txt:  
`$ grep -i Mount mountains.txt`

The above commands are a great way to get started with grep. If you are familiar with regular expressions, you can use regular expressions to search for patterns in files.

`grep -R` searches all files in a directory and outputs filenames and lines containing matched results. `-R` stands for "recursive". Here `grep -R` searches the /home/ccuser/workspace/geography directory for the string "Arctic" and outputs filenames and lines with matched results:  
`$ grep -R Arctic /home/ccuser/workspace/geography`

`grep -Rl` searches all files in a directory and outputs only filenames with matched results. `-R` stands for "recursive" and `l` stands for "files with matches". Here grep `-Rl` searches the /home/ccuser/workspace/geography directory for the string "Arctic" and outputs filenames with matched results:  
`$ grep -Rl Arctic /home/ccuser/workspace/geography`  

### 10. Stream editor (`sed`)
Stream editor accepts standard input and modifies it based on an expression, before displaying it as output data. It is similar to "find and replace".

Let's look at the expression `'s/snow/rain/'` from `$ sed 's/snow/rain/' forests.txt`:

* `s`: stands for "substitution". it is always used when using sed for substitution.
* `snow:` the search string, the text to find.
* `rain:` the replacement string, the text to add in place.
In this case, sed searches forests.txt for the word "snow" and replaces it with "rain." Importantly, the above command will only replace the first instance of "snow" on a line.

### 11. Globals (`g`)
An expression, meaning "global". Here `sed` searches forests.txt for the word "snow" and replaces it with "rain", globally. All instances of "snow" on a line will be turned to "rain":  
`$ sed 's/snow/rain/g' forests.txt`

## Standard error (`stderr`)
An error message outputted by a failed process.

# Environment
Each time we launch the terminal application, it creates a new session. The session immediately loads settings and preferences that make up the command line environment.

We can configure the environment to support the commands and programs we create. This enables us to customize greetings and command aliases, and create variables to share across commands and programs.

## Nano Text Editor
A command line text editor. It works just like a desktop text editor like TextEdit or Notepad, except that it is accessible from the command line and only accepts keyboard input.

1. The command nano hello.txt opens a new text file named hello.txt in the nano text editor.
2. "Hello, I am nano" is a text string entered in nano through the cursor.
3. The menu of keyboard commands at the bottom of the window allow us to save changes to hello.txt and exit nano. The `^` stands for the `Ctrl` key.
4. `Ctrl` + `O` saves a file. 'O' stands for output.
5. `Ctrl` + `X` exits the nano program. 'X' stands for exit.
6. `Ctrl` + `G` opens a help menu.
7. Entering in the text `clear` clears the terminal window, moving the command prompt to the top of the screen.

## Creating a file
`$ nano ~/.bash_profile`, where `~/.bash_profile` is the name of file used to store environment settings. It is commonly called the "bash profile". When a session starts, it will load the contents of the bash profile before executing commands.

* The command nano `~/.bash_profile` opens up `~/.bash_profile` in nano.
* The text echo "Welcome, Jane Doe" creates a greeting in the bash profile, which is saved. It tells the command line to echo the string "Welcome, Jane Doe" when a terminal session begins.
* The command source `~/.bash_profile` activates the changes in `~/.bash_profile` for the current session. Instead of closing the terminal and needing to start a new session, source makes the changes available right away in the session we are in.

## Alias (`alias`)
The alias command allows you to create keyboard shortcuts, or aliases, for commonly used commands.

Here `alias pd="pwd"` creates the alias `pd` for the `pwd` command, which is then saved in the bash profile. Each time you enter `pd`, the output will be the same as the `pwd` command.
The command source `~/.bash_profile` makes the alias `pd` available in the current session.
Each time we open up the terminal, we can use the `pd` alias:  
`alias pd="pwd"`

### History (`hy`)
Set as an alias for the history command in the bash profile. The alias is then made available in the current session through source. By typing `hy`, the command line outputs a history of commands that were entered in the current session:  
`alias hy="history"`

### Directory Output (`ll`)  
ll is set as an alias for ls -la and made available in the current session through source. By typing ll, the command line now outputs all contents and directories in long format, including all hidden files:  
`alias ll="ls -la"`

## Environmental Variables
Variables that can be used across commands and programs and hold information about the environment.

The line `USER="Jane Doe"` sets the environment variable `USER` to a name `"Jane Doe"`. Usually the `USER` variable is set to the name of the computer's owner.

The line export makes the variable to be available to all child sessions initiated from the session you are in. This is a way to make the variable persist across programs. At the command line, the command echo `$USER` returns the value of the variable. Note that `$` is always used when returning a variable's value. Here, the command echo `$USER` returns the name set for the variable:  
`export USER="Jane Doe"`

## Prompt Variables (`PS1`)
Variables that define the makeup and style of the command prompt. `export PS1=">> "` sets the command prompt variable and exports the variable. Here we change the default command prompt from `$` to `>>`. After using the source command, the command line displays the new command prompt.

## Home Variable (`HOME`)
An environment variable that displays the path of the home directory. Here by typing echo $HOME, the terminal displays the path /home/ccuser as output. You can customize the `HOME` variable if needed, but in most cases this is not necessary.

## Path Variable (`PATH`)
An environment variable that stores a list of directories separated by a colon. Looking carefully, `echo $PATH` lists the following directories:

```
/home/ccuser/.gem/ruby/2.0.0/bin
/usr/local/sbin
/usr/local/bin
/usr/bin
/usr/sbin
/sbin
/bin
```

Each directory contains scripts for the command line to execute. The `PATH` variable simply lists which directories contain scripts.

For example, many commands we've learned are scripts stored in the /bin directory: `/bin/pwd`. This is the script that is executed when you type the pwd command: `/bin/ls`. This is the script that is executed when you type the ls command. In advanced cases, you can customize the `PATH` variable when adding scripts of your own.

## Environment (`env`)
Returns a list of the environment variables for the current user. Here, the `env` command returns a number of variables, including PATH, PWD, PS1, and HOME.

`env | grep PATH` is a command that displays the value of a single environment variable. Here the standard output of env is "piped" to the grep command. grep searches for the value of the variable PATH and outputs it to the terminal.
