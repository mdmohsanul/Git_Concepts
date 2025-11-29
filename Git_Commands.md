# git --version  -> returns the current version installed
# Git is a software that we need to install in our system.
# git status -> It is used to get the status of git software.

# git init -> It is used to initialize git in our folder so that it can tracked by git. (one time per project)
- creates a .git folder --> a hidden folder to keep history of all files and sub-folders.

# .gitIgnore
- In this file we can keep the files and folders that we don't want to push in github repo.
- we can alse generate .gitIgnore file data online by selection which project we are making like (node, C++,Ruby)

# .gitKeep
- just to keep these file 

# Staging Area - It is an intermediate zone before you make any commit


### Commands

- git status -> 
- pwd -> to check the present work directory
- ls -> to get the list of files in that particular file
- ls -la -> all list including the hidden files(works only in command line like git bash)

* To set or connect to github to our local
- git config --global user.email "your@gmail.com"
- git config --global user.name "yourname"

- git config --list -> to check all the configuration

## Create/commit a repo

# git status -> to check if there is already git initialize or not
# git init -> It will create a working directory
# git add <filename> -> It add our files to staging area
# git restore --staged testTwo.txt -> to unstage a file

# git log -> log of commit with commit hash
# git log --oneline -> it will give logs in shorter


# git remote -v -Lists remote repositories and their URLs.
