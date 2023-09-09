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

