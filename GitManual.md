# GIT manual. First steps in VS Code

## Before starting

1. **Open** *TERMINAL*

2. **Enter** commdand `git config --global user.name "YOUR NAME"`

3. **Enter** commdand `git config --global user.email "<адрес_почты@email.com>"`

## Main starting steps

1. **Open** or **create** your target *folder* in *EXPLORER*
2. **Enter** commdand `git init` while inside target *folder* (creating reposit)
3. **Create** target file (-s)

## Main steps for creating versions

1. Allways **save** all changes in file (-s) 
2. Tracking files within reposit:
    * **Enter** commdand `git add "FILE NAME"` to track one file
    * **Enter** commdand `git add .` to track all files in folder
3. **Enter** commdand `git commit -m "YOUR VERSION COMMENT"` (save new version within reposit)
4. As long as working files are the same `git commit -am "YOUR VERSION COMMENT"` can be used several times after **steps 1-2**

## Other commands

* `git log` - calls list of last versions (before current)
* `git log --graph` - call graphical list of last versions and branchs
* `git reflog` - calls list of all versions/branches/checkouts
* `git status` - current info about changes within reposit
* `git checkout "NAME"` - upload target version/branch from **log**/**reflog**/**branch** list
* `git checkout master` - upload master version/branch
* `git diff` - show difference between current uncommited version and master version (within saved files)
* `git diff "COMMIT NAME 1" "COMMIT NAME 2"` - show difference between two specific versions

## Other terms

* `Master` - last commited version within main branch
* `Head` - current working version



# NEW - lection 2

`clear` - clean terminals text
`git branch` - calls list of branches (* - current branch)
`git branch "BRANCH NAME"` - creat new branch beside master
`git branch -d "BRANCH NAME"` - delete branch
`git merge "BRANCH NAME"` - insert branch version into current branch

Add file `.gitignore` in main folder and make list of file to ignore via `git status` (don't forget to commit ignore list into master branch)