# GitLearning

This is a testing repo for learning Git

# Notes about Git

## Git commands

### 1-  git init
to create reop in the current directory

### 2- git add fileName 
to add the current folder to be commited

### 3- git add .
to add all what's in the current directory to be commited

### 4- git commit fileName
to commit the file to the global repo

### 5- git commit fileName -m "commit message to be sent"

### 6- git log
shows the list of commits made

### 7- git log -n 'x'
x is a number -> shows the last x commits made

### 8- git log author="name"
searchs for the commits made by anyone have that name

### 9- git status 
gets a report about files in the staging area and that is in the working directory and not in the staging to be added or commited

### 10- git diff
it shows the differences between the files on the working tree and the ones on the repo


## Git notes

### 1- git uses a three tree archticture by having a repo and the working tree (those two are like any other version control systems) but git also have a third tree which is the staging index that is between both other trees.

### 2- when we do add command files are copied from the working tree to the staging tree and when we commit they are copied to the reop.