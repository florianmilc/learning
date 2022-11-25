# Git Commands Cheatsheet

## user settings
change global user.name: `git confing --global user.name "userName"`
change global email: `git config --global user.email userEmail`

change local user.name: `git config user.name "userName"`
change local email: `git config user.email userEmail`
    tip: perform in a repo root folder

check setting: `git config --list`

## listing branches
list all local: `git branch`
list all remote: `gir branch -r`

## checking out branch
`git checkout branchName`
example: `git checkout master`

check current status: `git status`

## deleting branches
delete local: `git branch -d localBranchName`
delete remote: `git push origin --delete remoteBranchName`

## commit and push
check changes: `git status`
stage changed files:
    adding a new file: `git add fileName` example: `git add docs/example.md`
    deleting a file: `git rm fileName` example: `git rm docs/example.md`
commit: `git commit -m "commitMessage"`

push: `git push origin`

## other
reset user settings after a commit: `git commit --amend --reset-author --no-edit`