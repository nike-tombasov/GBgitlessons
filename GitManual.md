# GIT manual. First steps in VS Code

## Before starting

1. **Open** *TERMINAL*

2. **Enter** commdand `git config --global user.name "YOUR NAME"`

3. **Enter** commdand `git config --global user.email "<адрес_почты@email.com>"`

## Main starting steps

1. **Open** or **create** your target `folder` in *EXPLORER*
2. **Enter** commdand `git init` while inside target `folder` (creating reposit)
3. **Create** target file (-s)

## Main steps for creating versions

1. Allways **save** all changes in file (-s) 
2. Tracking files:
    * **Enter** commdand `git add "FILE NAME"` to track one file (tracking file within reposit)   
    * **Enter** commdand `git add .` to track all files in folder (tracking files within reposit)
3. **Enter** commdand `git commit -m "YOUR VERSION COMMENT"` (save new version within reposit)
4. As long as working files are the same `git commit -am "YOUR VERSION COMMENT"` can be used several times after **step 2**

## Other commands

* `git log` - call list of last versions (before current)
* `git reflog` - call list of all versions
* `git status` - current info about changes within reposit
* `git checkout "COMMIT NAME"` - upload target version from **reflog** list
* `git checkout master` - upload last commited version
* `git diff` - show difference between current uncommited version and master version (within saved files)
* `git diff "COMMIT NAME 1" "COMMIT NAME 2"` - show difference between two specific versions

## Other terms

* `Master` - last commited version
* `Head` - current working version