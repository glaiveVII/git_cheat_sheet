# Github cheat sheet !!!!!

https://github.com/taniarascia/git
https://gist.github.com/jedmao/5053440
https://github.github.com/training-kit/downloads/github-git-cheat-sheet.pdf

idea : gitflow , alias, flow pour d'autre feature 


## Aliases : game changer, trust me 

#### Basic Github shortcut : 

alias gs='git status' <br/>
alias ga='git add' <br/>
alias gaa='git add .' <br/>
alias gc='git commit -m' <br/>
alias gm='git push origin master' <br/>
alias cr='clear' <br/>


#### Shortcut for a framework : Rails shortcut 

alias rs='rails s' <br/>
alias dd='rails db:drop' <br/>
alias dc='rails db:create' <br/>
alias dm='rails db:migrate' <br/>
alias ds='rails db:seed' <br/>
alias da='rails db:drop db:create db:migrate db:seed' <br/>
alias rc='rails c' <br/>
alias rr='rails routes' <br/>

#### Github' shortcuts when collaborating : 

alias gb = 'git branch' <br/>
alias gco = 'git checkout' <br/>
alias gcob = 'git checkout -b' <br/>
alias gp='git push origin' <br/>
alias gl='git pull origin' <br/>
alias pom = 'git push origin master' <br/>
alias puom = 'git pull origin master' <br/>

#### Make your life easier, for example : 

###### Open slack
alias slk="open -a 'slack'" <br/>

###### Open chrome
alias crm="open -a 'Google Chrome'" <br/>






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

#### Check that the repo is empty : 
6. $ git pull origin master

7. $ git add .

8. $ git commit -m "initialize the repository"

9. $ git push origin master

:warning: ONLY TIME YOUR ARE ALLOWED TO PUSH ON MASTER OF COURSE (btw you can make a branch also here !) 

#### Check it works ! 
10. $ git status

## Cloning a repository on your laptop : 

1. $ mkdir ~/code/OWNER_GITHUB_USERNAME
2. $ cd ~/code/OWNER_GITHUB_USERNAME
3. $ git clone git@github.com:OWNER_GITHUB_USERNAME/PROJECT_NAME.git
4. $ cd PROJECT_NAME

----------------------------------------------------------------------------------------------------------------------------


