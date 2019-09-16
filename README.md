# Github cheat sheet !!!!!

https://github.com/taniarascia/git
https://gist.github.com/jedmao/5053440
https://github.github.com/training-kit/downloads/github-git-cheat-sheet.pdf

idea : gitflow , alias, flow pour d'autre feature 


## Aliases : game changer, trust me 

----------------------------------------------------------------------------------------------------------------------------

## Initialize a repository from your terminal : 

#### Be on your github file on your desktop : 

1. $ mkdir PROJECT-NAME

2. $ cd PROJECT-NAME

#### Make github track your files 
3. $ git init

#### Set a new remote & the repository name PORJECT-NAME on your github account
4. $ hub create
#### Verify that their is a new remote
5. $ git remote -v

You should get someting like : 

```
origin	git@github.com:GITHUB_USERNAME/PROJECT-NAME.git (fetch)
origin	git@github.com:GITHUB_USERNAME/PROJECT-NAME.git (push)
```

6. $ git pull origin master

7. $ git add .

8. $ git commit -m "initialize the repository"

9. $ git push origin master

:warning: ONLY TIME YOUR ARE ALLOWED TO PUSH ON MASTER OF COURSE (btw you can make a branch also here !) 

#### Check it works ! 
10. $ git status

----------------------------------------------------------------------------------------------------------------------------


