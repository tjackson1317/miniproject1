# GitFlow and Git Terminology

## About GitFlow 
The Gitflow workflow is a branching model for Git that provides a robust framework for managing larger projects. It is ideal for collaboration and scaling a development team. Its unique features, including parallel development that isolates new development from finished work (feature branches), release staging area (develop branch), and support for emergency fixes (hotfix branches) make it great for a release-based software workflow. Gitflow gives each of these branches very specific roles and defines exactly how and when they should interact.

First, new development, which includes new features and non-emergency bug fixes, are built in feature branches. These feature branches are branched off of the develop branch; then, once finished and ready for release, features and fixes are merged back into the develop branch. In other words, the develop branch serves as an integration branch for features.

When the time comes to make a release, a release branch is created off of the develop branch. The code in that release branch is deployed onto a test environment, where a cycle of deploy, test, fix, redeploy, and retest continues until the release is finished and ready for customers.

At this point, the release branch is merged into both the master and develop branches in order to ensure that any changes made in the release branch are not accidentally lost by new development. The master branch is used to track released code only; thus, the only commits to master are merges from release branches and hotfix branches. It is convenient to tag all commits in the master branch with a version number.

Used to create emergency fixes, hotfix branches are branched directly from a tagged release in the master branch. Like previously discussed with the release branch, hotfix branches are also merged into both the master and develop branches to prevent any unintentional loss of the fixes when the next regular release occurs. 

## Repository
A repository is like a folder or storage space for a GIT project. A project's repository contains all of its files, such as code, documentation, images, and more. It also tracks every change that a developer (or his/her collaborators) make to each file, so the developer can always go back to previous versions of the project to fix any mistakes. In summary, a repository is a collection of commits, branches, and tags to identify commits.

## Clone
A clone is a copy of a repository that does not live on a website's server, but rather on a computer. The term can also be used as a verb to mean the act of making that copy. Clones can be useful when a developer wants to edit files in his/her preferred editor (without having to be online), but still wants to use Git to keep track of the changes. The clone is still connected to the remote version, so changes are synced between the two.

## Fork
A fork is a copy of a repository. It allows a user to freely experiment with changes without affecting the original project. Most commonly, forks are used to either propose changes to another user’s project, or to use another user’s project as a starting point for a new project. One example of using forks to propose changes is for bug fixes. Simply fork the repository, make the fix, then submit a pull request to the project owner.

## Branch
A branch is a parallel version of a repository. In other words, it is contained within the repository, but does not affect the master branch. This allows a developer to work freely without disrupting the live version of the repository. Once the desired change are made, a branch can be merged back into the master branch, which publishes the changes.

## Commit 
This command records or snapshots the file permanently in the version history.
git commit -m “[ Type in the commit message]”  
git commit -a  
This command commits any files you’ve added with the git add command and also commits any files you’ve changed since then.

<img src= "https://www.earthdatascience.org/images/workshops/version-control/git-checkout.png" alt= add,commit and checkiut> 
## Merge:
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
<img src="https://d186loudes4jlv.cloudfront.net/git/images/git_push.jpg>
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
<img src="https://i.stack.imgur.com/F00b8.png alt="Master Branch">
