# Vi and Linux commands

## About Vi
Vi (visual editor) is the default editor used with Linux. It has two main modes of operation:

1. Command mode: causes action to be taken on a file (takes user commands)
1. Insert mode: entered text is inserted into the file (edits text)

Vi is perfect for both creating scripts and editing files.

## cd
  This command is used to change the current working directory, which is the directory that the user is currently working in. Each time a user interacts with the command prompt, he or she is working within a directory; thus, cd is one of the most basic and frequently used Linux commands. When used without an argument, cd takes the user to the home directory. When used with an argument, such "Downloads," cd will change the directory to the one provided. Please see the example below:

## mkdir
  it allows the user to created directories in Linux. This command can also make multiple directiories. We use the command mkdir [directory name] to make directories , if multiple directories have to be made we have a space between the directory names mkdir [name1] [name2]
## cp
  cp stands for copy in linux. This command is used to copy files or a grouop or a directory.it requires two filenames in its arguments. If a command has 2 files names, then it copies the contents of first file into another. If it doesnt exist, it creates one and all the content is copied in that 
      *Various options*
      -**i(interactive)** In this options
 
 ## pwd 
 Pwd stands for print working directory. Starting from the root, it prints the full path of the current working directory. The command has two flags:

Pwd -L prints the symbolic path.
Pwd -P prints the actual path (avoiding symlinks).

## mv
The mv command is used to move files or directories from one place to another. The command supports moving single files and multiple files. For added convenience, it can prompt before overwriting and also has the option to only move files that are new to the destination. The mv command is also used to rename files. To use the command, pass the name of the file or directory followed by the destination.

## rm
rm, which stands for “remove here,” is used to remove objects from the file system. More specifically, it removes references to objects, such as files, directories, symbolic links, etc., from the file system (although by default it does not remove directories). This can be helpful when objects might have multiple references, such as a file with two different names. However, the command should be used with caution since you are not able to recover the contents of a file once deleted.

## History
The history command shows all of the last commands that have been recently used. By default, it shows the last five hundred commands entered. The up arrow and down arrow can be used to browse for a particular recent command.

## Home Directory and ~
A standard subdirectory of the root directory, the home directory serves as the repository for a user’s personal files, directories, and programs. It is the first directory a user is in after logging into the system. The tilde (~) represents the user’s home directory; thus, a user could return to the home directory by using the tilde as an argument to cd (cd ~).
