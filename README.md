# GitTutorials-
Learn Git From Scratch 

Install Git to the particular Operating system 

## Git Config 

git config --global user.name = name 
git config --global user.email = email
git config --list -----> list the username and password 

## For help 

git help config ------> helps for a particular package 
git --help -----------> list of all details in the git 
                        all commands typically its like 
                        an index for all commands 

### For already existing project push to git 

add all files ----> git add .
commit all files ---------> git commit -m "message"
git remote add origin "git@github" (repo link from clone) 


### Fror creating a local project a git repository 

git init -----> initialises it as a git repository 
To stop tracking just delete the .git repo 

## To know the status of local repo before commitinng 

git status 

## To not save files to git create a gitingnore file 

touch .gitignore

whatever we wirte inside the gitignore will be eliminated while we push the  
data 

## to stage the files to git 

git add [filename][*]

git add -A -----> add all file to staging area

## reset from staging 

git reset  [filename][*]

## commiting stashed files to git 

git commit -m "message before commit "

## To view all git logs 

git log 

### How ot download from a remote git directory 

git clone [link]

## how to get all details of a repo

git remote -v -----> versions of the project 

git branch -a ---->>> get all branches of a repo 

### To see the changes before commiting  

 git diff


 ## Before commititng do a push to the git repository 
 git pull origin master 

 ## create a branch 

 git branch [branchname]
 git checkout [branchname]

 check branch 

 git branch -a 

 ## workflow 

 create a branch 
 
 git checkout branch
 
 git add  * 
 
 git commit 
 
 git push 
 
 git checkout master 
 
 git pull
 
 git merge [branch]
 
 git push origin master 
 
 git branch --merged 
 
 git branch -d [branchmain]   ------->  only local branch deleted 
 
 git push origin --delete [branch]
 


## stashing  before creating a branch 

git stash

git stash pop 


#### feature branches 


$ git checkout -b myfeature develop
Switched to a new branch "myfeature"

$ git checkout develop

Switched to branch 'develop'

$ git merge --no-ff myfeature
Updating ea1b82a..05e9557

(Summary of changes)
$ git branch -d myfeature

Deleted branch myfeature (was 05e9557).
$ git push origin develop

#### feature branches delete multiple branches at the same time 

# git branch | grep 'feature/' | xargs git branch -d

# git push origin --delete $(git ls-remote --heads origin 'feature/*' | awk -F/ '{print "feature/" $NF}')

https://nvie.com/posts/a-successful-git-branching-model/




