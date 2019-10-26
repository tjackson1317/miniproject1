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

