# git-commands
#addinga file in git repo

Right click the directory and select gitbash here to open gitbash directly
 (or)
change the directory =  cd D:/
Creating project folder =  mkdir project 
select the file to be taken by git =    git init

creating a readme text file inside the directory = touch new.txt
to list the files in the directory =  ls
to get the status of commits in the git directory =    git status
to add the repositery =   git add . 
to commit the file =    git commit -m "sample commit instructions"
create a new empty repo on github.com
to set a link for repositary =  git remote add origin "repo link"
to check all the remote repo = git remote -v
to push into repo =  git push -u orgin master

#cloning a file and uploading it again
go to a representive folder and do gitbash here.
to clone a online repo = git clone "add the link"
to show the files cloned = ls -la
to check the status = git status
to save the changes made = git add . (or) git add filename
to commit the added files locally = git commit - m "message" -"description"
add the ssh key generating setup
to upload it in remote repositary = git push origin master

#connecting local machine to git repo to athenticate 
~ ssh-keygen -t rsa -b 4096 -C "email@example.com"
a default file is created in this loacation give a name
blank passphrase
get the key from local repo
.pub is public and other one is private 
copy the public key
now go to github-> settings-> ssh and gpg keys->new ssh key -> paste the key
~ ssh-add -K ~/.ssh/id_rsa

#Master Brannch- main branch 
#Feature Branch- sub branch to be linked to main soon  
#Hot fix Branch- before linking it to master fixing bugs 

#creating and jumping in branches
to see the branches= git branch
to exit = q
creating new branch = git checkout -b nameofbranch
You are now in the featured branch to check that do = git branch
to switch between branches use = git checkout master
this * represents the branch you are in

#to add the changed files in branch
to save locally = git status -> git add . -> git commit -m "comment"
to check and compare the changes in master and featured = git diff "freatured branch name"
pushing the changes to github = git push
creating a new branch in github(without merging) = git push -u origin nameofbranch

the changes in featured branch does not show up in master until you(local) = git merge "other branch name"

#merging on github.com
go to pull request -> open a pull request -> create a pull request by adding tittle and description -> check for the changes and comments -> merge pull request 

pulling the merged repo(in master branch) = git pull
delete the featured branch = git branch -d nameofbranch

#undoing in git
undoing all added files = git reset 
undo a single added file = git reset filename
undo a commit(undo one commit) = git reset HEAD~1
shows all list of commits = git log
copy the commit hashcode
go back to a specific commit in the list = git reset hashcode

#forking = to get other peoples repo and edit it using git 






