git config --global user.name "girishl"

git config --global user.email "girishlingappa7@gmail.com"

git config --global color.ui true


Create a new repository
sudo mkdir machine_learning
cd machine_learning

Open it and perform a 
 git init to create a new git repository
sudo git init
ls -al

Your local repository consists of three "trees" maintained by git. the first one is your Working Directory which holds the actual files. the second one is the Index which acts as a staging area and finally the HEAD which points to the last commit you've made.

git status

cd .git/objects/

You can propose changes (add it to the Index) using
sudo git add one.py
sudo git add *

git stauts

This is the first step in the basic git workflow. To actually commit these changes use
git commit
git commit -m "Commit message"

Now the file is committed to the HEAD, but not in your remote repository yet. 

Log in its simplest form, you can study repository history using.. git log
You can add a lot of parameters to make the log look like what you want.  

git log


Branches are used to develop features isolated from each other. master branch is the "default" branch when you create a repository. Use other branches for development and merge them back to the master branch upon completion. 

#To show branches
git branch

#To create a new branch
sudo git branch SECOND	
git status


#switching working dir to givben brnach
sudo git checkout SECOND
git status





Show changes between commits, commit and working tree, etc
git diff


git add -p

git branch -v


Merge both dir(branch) together
sudo git merge SECOND


Delete the branch
sudo git branch -d SECOND

Our changes are now in the HEAD of your local working copy. To send those changes to your remote repository, execute 

sudo git remote add origin  https://github.com/girishl/machine_learning.git
git remote -v

sudo git init

sudo git push origin master













