# git_lesson

## start with local GIT

- Install GIT to your pc <br>
sudo apt install git
- Initalise GIT<br>
git init
- check GIT configuration<br>
git config
- check GIT status <br>
git status
- delete GIT from foulder <br>
rm -rf .git

---------------

## generate SSH keys public and private

- go to your home directory <br>
cd ~
- check if you already have a generated ssh key <br>
ls -la .ssh/
- generate public/private rsa key pair <br>
ssh-keygen -t ed25519 -C your@email.on-github
- check that key pair has been generated correctely <br>
ls -a ~/.ssh

--------

## create public GIT repo

- create an account on github.com
- create new repo
- insert ssh key. Settings-->SSH and GPG keys --> New SSH key
- check availability of your SSH key on github <br>
ssh -T git@github.com 

----------

## Connect local GIT and remote repo

- connect local GIT and remote repo <br>
git remote add origin git@github.com:XandrAsh/git_lesson.git
- ensure that local git and remote repo are connected
git remote -v

------------

## make changes to remote repo from local git

- add all changes to commit queue <br>
git add --all
- commit all changes <br>
git commit -m 'my comment for commit'
- push all changes to remote repo for the first time <br> 
git push -u origin main 










