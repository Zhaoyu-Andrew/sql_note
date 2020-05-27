# git command

##  git log
**shows all the commits executed**
```bash
git log
```
**show all commits in condense format**
```bash
git log -- oneline 
```



## checkout commit
**first check out all commit tags using**
```bash
git log -- oneline 
```
**check out specific commit in the history (open file to see changes)**
```bash
git checkout b7b2d3d
```
back to master branch
```bash
git checkout master
```


## revert commit 
**cancel out a commit**
```bash
git revert b7b2d3d
```
then type `shift + ":"` on the bottom and type `wq` to quit the window

## reset 
**delete all the commits after specific commit**
```bash
git reset b7b2d3d
```
all the work done after the commit `b7b2d3d` is still preserved in the 
file, but all the commit points after `b7b2d3d` been disappear

**permanantly remove all the commit including its content****
```bash
git reset b7b2d3d --hard
```

## branch
**create branch('feature-1' is the name of the created branch)**
```bash
git branch feature-1
```
**shows all the branch**
```bash
git branch -a
```
**checkout created branch**
```bash
git checkout feature-1
```
**Delete branch**
first go back to master branch
```bash
git checkout master
```
then type:
```bash
git branc -D feature-1
```
**create branch called 'feature-a' and checkout feature-a**
```bash
git checkout -b feature-a
```
 ## merge branch
```bash
git checkout master
```
then merges feature-a into master
```bash
git merge feature-a
```

## push to github 
origin = alias of the URL
```bash
git remote add origin URL
```
push everything on the local repository to the master branch on URL
```bash
git push origin master
```

## clone from github to local
```bash
git clone URL
```
after clone, can push directly to github without insert URL
```bash
git remote -v
```
## collaborate on github
pull all the code on origin to local master
```bash
git pull origin master
```
add and commmit change in this separate branch instead of the local master branch, then push the secondary branch to github, do not edit on master local master branch and then push the local master branch because it will overwrite the github master branch

```bash
git checkout -b branchname
```
after our changes are made from second branch is agree 

```bash
git checkout master
git pull origin master
```
second command this will update the local master branch


## forking 
first find repository, and click on the "fork" button copy all the file on someones' repository and create a new repository in your own github



