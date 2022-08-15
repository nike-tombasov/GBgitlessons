# GIT manual. First steps in VS Code

## Before starting

1. **Open** *TERMINAL*

2. **Enter** commdand `git config --global user.name YOUR_NAME`

3. **Enter** commdand `git config --global user.email your_mail@email.com`

## Main starting steps

1. **Open** or **create** your target *folder* in *EXPLORER*
2. **Enter** commdand `git init` while inside target *folder* (creating reposit)
3. **Create** target file (-s)

## Main steps for creating versions

1. Allways **save** all changes in file (-s) 
2. Tracking files within reposit:
    * **Enter** commdand `git add FILE_NAME` to track one file
    * **Enter** commdand `git add .` to track all files in folder
3. **Enter** commdand `git commit -m YOUR_VERSION_COMMENT` (save new version within reposit)
4. As long as working files are the same `git commit -am YOUR_VERSION_COMMENT` can be used several times after **steps 1-2**

## Other commands

* `git log` - calls list of last versions (before current)
* `git log --graph` - call graphical list of last versions and branchs
* `git reflog` - calls list of all versions/branches/checkouts
* `git status` - current info about changes within reposit
* `git checkout NAME` - upload target version/branch from **log**/**reflog**/**branch** list
* `git checkout master` - upload master version/branch
* `git diff` - show difference between current uncommited version and master version (within saved files)
* `git diff COMMIT_NAME_1 COMMIT_NAME_2` - show difference between two specific versions

## Other terms

* `Master` - last commited version within main branch
* `Head` - current working version

# NEW - lection 2 - branches

`clear` - clean terminals text

`git branch` - calls list of branches (* - current branch)

`git branch BRANCH_NAME` - creat new branch beside master

`git checkout -b BRANCH_NAME` - creat new branch and upload it

`git branch -d BRANCH_NAME` - delete some branchs

`git merge BRANCH_NAME` - insert branch version into current branch

`git merge BRANCH_NAME_1 BRANCH_NAME_2` - insert several branchs into current branch

`git merge --abort` - abort last merge

Add file `.gitignore` in main folder and make list of file to ignore via `git status` (don't forget to commit ignore list into master branch)


# NEW - lection 3 - GitHub.com

`git clone https:\\LINK_ADDRES` - dublicate remote reposite to local machine

`git pull` - download and merge all changes from remote reposite 

`git push` - upload and merge all changeas from local machine to remote reposite (auth can be requested)

## Creating and working with remote reposites
1. **Create** *Github.com* account
2. **Create** local reposite
3. **Create** reposite on *github.com* and **link** (instructions are within github.com) it with local reposite
4. **Push** local reposite to *github.com*
5. **Pull** reposite from *github.com* to local if remoted version was changed

## Working with 3rd-party remote reposites
1. **Fork** 3rd-party remote reposite on *github.com* within your account 
2. **Clone** forked reposite to local
3. **Create** new branch and commit only in this branch
4. **Push** new commited version to your *github.com* 
5. **"Compare & Push"** version on *github.com* to send it to origin account with pull requset