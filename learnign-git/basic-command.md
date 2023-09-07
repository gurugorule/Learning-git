# learning git is Awesome

``` console

Confi guration
    git config --global user.name 'name'
    git config --global user.email 'email'
    git congit --global alias.s "status"   -> git s == git status
```

``` console

    git init
    git status
    git add .
    git stash ->  pop, clear
    git commit -m "message"
    git show 
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
    git diff branch_1 branch_2
    git push origin new_branch
    git fetch --all --prune
    git reset --hard upstream/main

```

point :
whta if i want to undo the commit after creating the pull request
    just reset the commit and force push it
    force push: -f

``` console
    git push origin branch -f
```