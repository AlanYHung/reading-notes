# Reading 03

### Version Control Types
1. Local Version Control - Developer controls versions locally on own machine.
1. Centralized Version Control (CVCS) - Team of Developers stores versions in a central location online/network.
1. Distributed Version Control (DVCS) - Multiple Developers create clones of the Central Repository, so can replace any lost data.

### What is Git?
1. Git is a DVCS file system made up of snapshots.
1. Git relies on local operations for speed in order to remove the need to fetch project history.
1. Git tracks all changes and detects file corruption
1. Git is set up to minimize the loss of data from data corruption.
1. Git has 3 main stages Committed, modified, and staged.

#### Git was developed by Linus Torvalds (chief architect of Linux Kernel) in response to the conflict between the Linux community and BitKeeper to make a DVCS similar to the structure of BitKeeper.

### Setup Git Resources
#### Windows
http://git-scm.com/download/win  
http://windows.github.com  
#### GUI
https://git-scm.com/downloads/guis

### Git Commands
1. git config --global user.name "Your Name"
1. git config --global user.email "Your Email"
1. git config --global user.name (should return Jane Smith)
1. git config --global user.email (should return example@email.com)
1. git config --global core.editor emacs (Default Text Editor)
1. git config --list
1. Help Commands
   1. git help command
   1. git command --help
   1. man git-command
1. git init
1. git add *.c
1. git add LICENSE
1. git commit -m “any message here”
1. git clone <Web Path>
1. git clone <Web Path> <Directory Path>
1. git status
1. git commit -a (commits all changes)
1. git push origin main
1. git stash (Use to hide changed files from showing up in the directory until ready to be committed)
1. git stash apply (Applies Stash changes)
1. git remote
1. git remote -v (To view all remote URLs)

### Resources
* [Git Introduction Tutorial](https://blog.udemy.com/git-tutorial-a-comprehensive-guide/)
  
[<-- Back](README.md)
