# Learning-git
-learning git is Awesome
```console
    git init
    git status
    git add .
    git stash ->  pop, clear
    git commit -m "message"
    git log --all --graph
    git restore 
    git reset
    git remote add origin url
    git remote -v
    git remote remove origin
    git branch 
    git branch new_branch
    git branch -d branch_name 
    git checkout new_branch 
    git checkout -b new_branch
    git push origin new_branch
    git fetch --all --prune
    git reset --hard upstream/main

```
point :
whta if i want to undo the commit after creating the pull request
    just reset the commit and force push it 
    force push: -f
```console
    git push origin branch -f
```