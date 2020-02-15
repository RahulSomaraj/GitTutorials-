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