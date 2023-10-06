# git_lesson

## start with local GIT

- #Install GIT to your pc <br>
sudo apt install git
- #Initalise GIT<br>
git init
- #check GIT configuration<br>
git config
- #check GIT status <br>
git status
- #delete GIT from foulder <br>
rm -rf .git

---------------

## generate SSH keys public and private

- #go to your home directory <br>
cd ~
- #check if you already have a generated ssh key <br>
ls -la .ssh/
- #generate public/private rsa key pair <br>
ssh-keygen -t ed25519 -C your@email.on-github
- #check that key pair has been generated correctely <br>
ls -a ~/.ssh

--------

## create public GIT repo

- #create an account on github.com
- #create new repo
- #insert ssh key. Settings-->SSH and GPG keys --> New SSH key
- #check availability of your SSH key on github <br>
ssh -T git@github.com 

----------

## Connect local GIT and remote repo

- #connect local GIT and remote repo <br>
git remote add origin git@github.com:XandrAsh/git_lesson.git
- #ensure that local git and remote repo are connected
git remote -v

------------

## make changes to remote repo from local git

- #add all changes to commit queue <br>
git add --all
- #commit all changes <br>
git commit -m 'my comment for commit'
- #push all changes to remote repo for the first time <br> 
git push -u origin master
- #compare and pull-request <br>
- #create pull-request <br>
- #merge pull-request <br>
- #confirm merge  <br>

----------

## Other usefull git commands
- create isolated development environments within a single repository  <br>
git branch 
- check out old commits and old file revisions, navigate existing branches  <br>
git checkout
- Remove untracked files from the working directory  <br>
git clean 
- Create a copy of an existing Git repository  <br>
git clone 
- Fetch downloads a branch from another repo, along with all of its associated commits and files  <br>
git fetch 
- explore the previous revisions of a project  <br>
git log
- integrate changes from divergent branches  <br>
git merge 
- download a branch from a remote repository and merge it into the current branch  <br>
git pull 
- clean up or completely remove changes that have not been pushed to a public repository  <br>
git reset 

