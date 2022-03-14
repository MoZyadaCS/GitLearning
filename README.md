# GitLearning

This is a testing repo for learning Git

# Notes about Git

## Git commands

### 1-  git init
to create reop in the current directory.

### 2- git add fileName 
to add the current folder to be commited.

### 3- git add .
to add all what's in the current directory to be commited.

### 4- git commit fileName
to commit the file to the global repo.

### 5- git commit fileName -m "commit message to be sent"
if we didn't put -m Git will ask for the message and then we can put multiple line message
### 6- git log
shows the list of commits made.

### 7- git log -n 'x'
x is a number -> shows the last x commits made.

### 8- git log author="name"
searchs for the commits made by anyone have that name.

### 9- git status 
gets a report about files in the staging area and that is in the working directory and not in the staging to be added or commited.

### 10- git diff
it shows the differences between the files on the working tree and the ones on the staging tree.

### 11- git diff --staged
shows the differences between the files on the staging tree and the files on the reop.

### 12- git rm fileName
it adds the changes of the delete file and delete it from the staging area.
or delete the file if not deleted and adds that change to the staging area.


### 13- re-nameing a file
    a- we change the file name in the directory and then do a delete with rm to the old name then add the new name and git will recognize they are the same file (if there is 50% similarity).

    b- git rv oldName newName 
    we use this command to move the file from one path to another path which changes the name.
### 14- git commit -a / git commit --all 
to add the changes from the working directory to the repo directly without having to put them in the staging area.

### 15- git show commitID
to show the details about specific commit using its id or part of it(the first 9 or 10 digits).

<<<<<<< HEAD
### 16- git diff olderCommitID..newerCommitID 
to show the difference or to compare between two different commits.

### 17- git checkout -- fileName 
to replace the file on the working directory with the one on the repo(to undo changes made on the working area by mistake).


### 18 - git reset HEAD fileName
to restore the file from the staging area (undo the add command).

### 19- git commit --amend -m "the commit message here"
to add some changes to the last commit that is already on the reop

### 20- git checkout CommidID -- fileName
to retrieve an old version of that file that was after that commit (with the id) happened.

### 21- git revert CommitId
revert the changes that happened from that commit and make them in a new commit with a new message.

### 22- git clean -n / -f
the command is to remove the untracked files by git (-n to show what would happen before you remove)
(-f actually removes them)
## Git notes

### 1- git uses a three tree archticture by having a repo and the working tree (those two are like any other version control systems) but git also have a third tree which is the staging index that is between both other trees.

### 2- when we do add command files are copied from the working tree to the staging tree and when we commit they are copied to the reop.

### 3- using .gitignore file to put some filenames or rules for the files that wouldn't be tracked by git.