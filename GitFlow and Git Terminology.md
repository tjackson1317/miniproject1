# GitFlow and Git Terminology

## About GitFlow 

## Repository

## Clone

## Fork

## Branch

## Commit
This command records or snapshots the file permanently in the version history.
git commit -m “[ Type in the commit message]”  
git commit -a  
This command commits any files you’ve added with the git add command and also commits any files you’ve changed since then
## Merge
git merge [branch name]  
This command merges the specified branch’s history into the current branch.
## Checkout
Usage: git checkout [branch name]  
This command is used to switch from one branch to another.
git checkout -b [branch name]  
This command creates a new branch and also switches to it.
## Push
Usage: git push [variable name] master  
This command sends the committed changes of master branch to your remote repository.
Usage: git push [variable name] [branch]  
This command sends the branch commits to your remote repository.
Usage: git push –all [variable name]  
This command pushes all branches to your remote repository.
Usage: git push [variable name] :[branch name]  
This command deletes a branch on your remote repository.
## Pull
Usage: git pull [Repository Link]  
This command fetches and merges changes on the remote server to your working directory.
## Remote Add/Remove/Show
The "remote" command helps you to manage connections to remote repositories.
It allows you to show which remotes are currently connected, but also to add new connections or remove existing ones.
Git remote add <shortname> <url>
Creates a new connection to a remote repository. The "shortname" you provide can later be used instead of the URL when referencing the remote. A typical default shortname is "origin": this is used for the remote which your local repository was cloned from.
Git remote remove <name>
Disconnects the remote from the local repository. Note that this will have no effect on the actual remote repository (i.e. the repository itself is not removed / deleted / etc.).
Git remote show<remote- name>
To see more information about a particular remote, we use this command. It lists the URL for the remote repository as well as the tracking branch information. The command helpfully tells you that if you’re on the master branch

## Status
Usage: git status  
This command lists all the files that have to be committed.
## Master Branch
A branch in Git is simply a lightweight movable pointer to one of these commits. The default branch name in Git is master. As you start making commits, you’re given a master branch that points to the last commit you made. Every time you commit, the master branch pointer moves forward automatically.
