# Vi and Linux commands

## About Vi
Vi (visual editor) is the default editor used with Linux. It has two main modes of operation:

1. Command mode: causes action to be taken on a file (takes user commands)
1. Insert mode: entered text is inserted into the file (edits text)

Vi is perfect for both creating scripts and editing files.

## cd
  This command is used to change the current working directory, which is the directory that the user is currently working in. Each time a user interacts with the command prompt, he or she is working within a directory; thus, cd is one of the most basic and frequently used Linux commands. When used without an argument, cd takes the user to the home directory. When used with an argument, such "Downloads," cd will change the directory to the one provided. 

<img src="https://media.geeksforgeeks.org/wp-content/uploads/Screenshot-from-2018-12-20-10-56-04-1.png" >

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

<img src ="https://media.geeksforgeeks.org/wp-content/uploads/built-inPwd-1.png">

## mv
The mv command is used to move files or directories from one place to another. The command supports moving single files and multiple files. For added convenience, it can prompt before overwriting and also has the option to only move files that are new to the destination. The mv command is also used to rename files. To use the command, pass the name of the file or directory followed by the destination.

## rm
rm, which stands for “remove here,” is used to remove objects from the file system. More specifically, it removes references to objects, such as files, directories, symbolic links, etc., from the file system (although by default it does not remove directories). This can be helpful when objects might have multiple references, such as a file with two different names. However, the command should be used with caution since you are not able to recover the contents of a file once deleted.

## History
The history command shows all of the last commands that have been recently used. By default, it shows the last five hundred commands entered. The up arrow and down arrow can be used to browse for a particular recent command.

<img src= "https://geek-university.com/wp-content/images/linux/history_command1.jpg?x67341" >

## Home Directory and ~
A standard subdirectory of the root directory, the home directory serves as the repository for a user’s personal files, directories, and programs. It is the first directory a user is in after logging into the system. The tilde (~) represents the user’s home directory; thus, a user could return to the home directory by using the tilde as an argument to cd (cd ~).

## File paths in linux
A file path is the human-readable representation of a file or folder’s location on a computer system.A path is a unique location to a file or a folder in a file system of an OS.A path to a file is a combination of / and alpha-numeric characters.

file paths are part of a useful framework for understanding how computers work, and learning to think of files in a path can be useful if you’re looking to become a developer (you need to understand the paths to support libraries), a web designer (file paths ensure you’re pointing your HTML to the appropriate CSS), a system administrator, or just a power user.
Start at the root directory ( / ) and work down.
Write a slash ( / ) after every directory name)
<img src= "https://www.tecmint.com/wp-content/uploads/2013/09/Linux-Directory-Structure.jpeg" alt= "important paths"> 

## Using the tab key to complete file paths
Tab completion is an extremely helpful feature in nearly any command-line environment, whether you’re using the Bash shell on Linux, Command Prompt or PowerShell on Windows, or a terminal window on Mac OS X.
This feature can dramatically help you speed up typing commands. Just hit Tab while typing a command, option, or file name and the shell environment will automatically complete what you’re typing or suggest options to you.

Tab completion is especially useful when typing file names, directories, and paths. Rather than trying to type a long file name that may involve spaces and special characters you’ll need to properly escape, you can just start typing the beginning of the name and press Tab.
Tab completion can even be used to automatically complete options for some commands. For example, when installing a package with the apt-get install command, you can use tab completion to automatically complete a package’s name. This also helps you search for related packages, and is very useful when you’re not sure exactly what a package is named.
How
Just click TAB

## Using up and down arrow for history 
e the up arrow key -- the previous command you entered shows up on the command line, and you can use the left arrow to move the cursor just after the capital C, hit Backspace, and type a lower case c. Note you can also position the cursor before the capital C and hit Delete to get rid of it.
Once you have changed the capital C to a lower case c you can hit Return to enter the command -- you do not have to move the cursor to the end of the line.
Now hit the up arrow key a few times, then hit the down arrow key and notice what happens. Play around with this until you get a good feel for what is happening.
Linux maintains a history of commands you have entered. Using the up and down arrow keys, you can recall previously-entered commands to the command line, edit them and re-issue them.
Makes the work easier
Click aaup and down arrow keys from your keyboard
