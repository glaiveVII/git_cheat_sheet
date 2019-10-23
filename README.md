# Github cheat sheet !!!!!

https://github.com/taniarascia/git
https://gist.github.com/jedmao/5053440
https://github.github.com/training-kit/downloads/github-git-cheat-sheet.pdf

idea : gitflow , alias, flow pour d'autre feature 

## GITHUB WORKFLOW :heart:

<p align="center">  
  <img src="github-flow.png" alt="drawing" width="1000" align="center"/>
</p>


## Usefull commands : 

  ##### To go to the GitHub web interface :
  ```
    $ hub browse
  ```
    
  ##### # Clear the command line window :
  ```
    $ clear 
  ```
   ##### To clear you terminal window on MacOs :
   ```
    cmd + k 
   ```
   ##### To access the history of commands you typed :
   ```
    $ history
   ```
   ##### To kill something executing in your terminal :
   ```
    control + c
   ```



  

## When working with other people : Pull request : 

    1. Never pull on the MASTER BRANCH 
    2. Don’t merge yourself unless 1000% sure :  Lead programmer closes your PR (merges your changes to remote master). But you’re not done yet!


## Aliases : game changer, trust me !

#### Basic Github shortcut : 

<pre>
    alias gs='git status' <br/>
    alias ga='git add' <br/>
    alias gaa='git add .' <br/>
    alias gc='git commit -m' <br/>
    alias gm='git push origin master' <br/>
    alias cr='clear' <br/>
</pre>


#### Shortcut for a framework : Rails shortcut 
<pre>
    alias rs='rails s' <br/>
    alias dd='rails db:drop' <br/>
    alias dc='rails db:create' <br/>
    alias dm='rails db:migrate' <br/>
    alias ds='rails db:seed' <br/>
    alias da='rails db:drop db:create db:migrate db:seed' <br/>
    alias rc='rails c' <br/>
    alias rr='rails routes' <br/>
</pre>
#### Github' shortcuts when collaborating : 

#### ---------- Simple aliases -----------
```
  alias gb = 'git branch' 
  alias gco = 'git checkout' 
  alias gcob = 'git checkout -b' 
  
  alias gcom='git checkout master'
  alias gd='git diff'
  alias gi='git init'
  alias glg='git log --graph --oneline --decorate --all'

  alias gp='git push origin' 
  alias gl='git pull origin' 
  alias pom = 'git push origin master' 
  alias puom = 'git pull origin master' 
```
#### ---------- Advanced aliases -----------
```
alias gpo='git push origin HEAD'
alias gbr='git branch -m'
alias ga='git add'
alias gaa='git add .'
alias gaaa='git add --all'
alias gau='git add --update'
alias gb='git branch'
alias gbd='git branch -D'
alias gc='git commit'
alias gcm='git commit --message'
alias gcf='git commit --fixup'
alias gco='git checkout'
alias gcam='git commit -am'
alias gt='git checkout -'
alias gcob='git checkout -b'
alias gcom='git checkout master'
alias gcos='git checkout staging'
alias gcod='git checkout develop'
alias gd='git diff'
alias gda='git diff HEAD'
alias gi='git init'
alias glg='git log --graph --oneline --decorate --all'
alias gld='git log --pretty=format:"%h %ad %s” --date=short --all"'
alias gm='git merge'
alias gma='git merge --abort'
alias gmc='git merge --continue'
alias gp='git pull'
alias gpr='git pull --rebase'
alias gr='git rebase'
alias gs='git status'
alias gss='git status --short'
alias gst='git stash'
alias gsta='git stash apply'
alias gstd='git stash drop'
alias gstl='git stash list'
alias gstp='git stash pop'
alias gsts='git stash save'
alias grh='git reset --hard HEAD'
alias gls="git for-each-ref --sort=-committerdate refs/heads/ --format='%(authordate:short) %(color:red)%(objectname:short) %(color:yellow)%(refname:short)%(color:reset) (%(color:green)%(committerdate:relative)%(color:reset))'"

alias ytbr="yarn tag-build-ready"
alias yd='yarn dev'
alias yyd='yarn && yarn dev'
alias ys='yarn start'
alias yt='yarn testn'
alias yst='yarn staticCheck'
alias ybys='yarn build && yarn start'
alias yf='yarn flow'

alias np='npm publish'
alias nptb='npm publish --tag beta'
```
#### ---------- Aliases to avoid being murdered -----------
```
aim idea here is to find a solution in order 
to block git push origin master or the same with -f 
i.e  to protect from all dangerous commands

or how to run command in order to block kind of command 
and returning a string or adding a [Y/N] or password ???
```


  
#### Make your life easier, for example : 

##### Open slack :
<pre>
    alias slk="open -a 'slack'" <br/> </pre>
##### Open chrome :
<pre>
    alias crm="open -a 'Google Chrome'" <br/> </pre>

----------------------------------------------------------------------------------------------------------------------------

## Initialize a repository from your terminal : 

#### Be on your github file on your desktop : 
1. $ mkdir PROJECT-NAME

2. $ cd PROJECT-NAME

#### Make github track your files :
3. $ git init

#### Set a new remote & the repository name PORJECT-NAME on your github account :
4. $ hub create
#### Verify that their is a new remote :
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

## Changes to tracked files:

$ git diff

## See changes/difference of a specific file:

$ git diff <file>
  
## Show all commits, starting with newest (it'll show the hash, author information, date of commit and title of the commit):

$ git log

----------------------------------------------------------------------------------------------------------------------------
## Create a GitHub Pull Request to improve repositories you find on github : 

1. Fork any open source GitHub repo you want 
2. Clone that repo in your PC :
```
  git clone https://github.com/YOUR-GITHUB-NAME/NAME-REPO-YOUR-FORKED
```
3. Make changes and commit/push these changes from your terminal :
```
  git add .
  git commit -m " My change for this repo"
  git push
```
4. Go to your fork, click open `Pull Request` link and create a PR : 
  Add a relevant description to comment your code 👌!

----------------------------------------------------------------------------------------------------------------------------

## If you want to improve this repository, follow these steps (work with all repository you don't own but you want to change)  :

1. Fork it ( https://github.com/PelDoingCode/git_cheat_sheet/fork )
2. Create your feature branch (git checkout -b my-new-feature)
3. Commit your changes (git commit -am 'Add some feature') - try to include tests
4. Push to the branch (git push origin my-new-feature)
5. Create a new Pull Request

----------------------------------------------------------------------------------------------------------------------------
## Never forget : in case of fire :fire:

  1. $ git commit
  2. $ git push
  3. LEAVE BUILDING

----------------------------------------------------------------------------------------------------------------------------
## :warning: :bomb: FORCE PUSH & PULL :bomb: :warning:
#### Force to push in case (bad practice) : :bomb: 
```
ga .
gc 'force to push in case of emergency'
git push origin master -f 
```
 ps : you can push on an other branch than master also 
 
 #### Force to pull to force update what you have in local (bad practice) : :bomb: 
 ```
 git fetch --all
 git reset --hard origin/master
 ```
  ps : you will force what you have on master to be on local

----------------------------------------------------------------------------------------------------------------------------

## 🍺 Buy me a beer 
If you like this project, feel free to donate:
* PayPal:
* Bitcoin: 

## ⭐️ Show your support
Please ⭐️ this repository if this project helped you, don't hesitate to reach me on Linkedin !
