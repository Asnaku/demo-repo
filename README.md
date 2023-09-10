# Github basics
## This is all about github basics.
Step1. Started by creating new file by clicking 'New' or '+' button.
Step2. The file name should be describing, README.md
## How to clone repo (Eg. this demo-repo) from remote to local machine/pull
1. open code editer (type cmd at ur directory then 'code .' then opens vs code editor)
2. in terminal of vs code type command 'git clone PastehttpFrom_clone'
## How to add SSH key
1. go to setting in github, then SSH key
2. give Title to your Key
3. hold on for Key field to fill
4. open gitbash then type 'ssh-keygen -t rsa -b 4096 -C "your_email@example.com" -f ~/.ssh/my_custom_key' to generate ssh key with passphrase 'my_custom_key', fill if asked.
5. give the directory you want where .ssh is saved or press enter then it by default saves in C:\Users\it's asneComplexo
6. then go to directory where it saved,
7. open .ssh folder and copy my_custom_key.pub file content
8. paste in key field of github
9. then press add key

## staging or tracking changes to file then commit then push 
for this purpose I have created file in demo-repo 'index.html'
1. first check 'git status', if file name is red it means not tracked
2. Add file to stage 'git add .' or 'git add index.html'
3. recheck 'git status', file name should be green and 'new file:   index.html'
4. commit 'git commit -m "msg" -m "description" ' press enter
So, in this 'git commit -m "Adding index.html file" -m "Description later"
Again check git status. 
Still the git commit also saved in local machine not in remote repo, So push comes here
5. before pushing, check the branch you are working with by
        'git remote show origin', if main
    then 'git push origin main'

## For repo created local machine may be via vs code editor,

it should be pushed to remote git repository, So to do this, first initialize your project. on terminal of that project directory type this git command 'git init', initializes the project in git repo.
now after tracking and commiting it, git push command don't pushes because the repo in remote should created by same name first. 'git remote add origin git@github.com:Asnaku/demo-repo2.git' to connect project(demo2) to remote 'git remote -v' to check any connected remote repo. 'git push -u origin master' to push, -u is upstream, helps to next time without saying origin master

## Git Branching

to switch to branches 'git checkout branchName' to create new branch 'git checkout -b feature-issue/description'

## Merging changes from remote to local machine

if you made changes in github/gitlab repo, remotly then
got to directory of your project on local machine in terminal

1. 'git branch' chech to branch, from which branch to which, then if main say main
2. 'git fetch origin'
3. 'git merge origin'
4. 'git rebase origin'
