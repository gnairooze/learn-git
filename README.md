git short notes
===============

$ git init

$ git status

$ git add octocat.txt

$ git status

$ git commit -m "Add cute octocat story"

$ git add '*.txt'

$ git commit -m 'Add all the octocat txt files'

$ git log

$ git remote add origin https://github.com/try-git/try_git.git

$ git push -u origin master

$ git pull origin master

$ git diff HEAD

$ git add octofamily/octodog.txt

$ git diff --staged

#remove file from staging area. But it is still in the file system
$ git reset octofamily/octodog.txt

#Files can be changed back to how they were at the last commit by using the command: git checkout -- <target>. get rid of all the changes since the last commit for octocat.txt
$ git checkout -- octocat.txt

#create branch
$ git branch clean_up

#switch to branch
$ git checkout clean_up

#remove all files from the file system and stage the file removal to be ready for commit
$ git rm '*.txt'

$ git commit -m "Remove all the cats"

#switch to master
$ git checkout master

#from the master branch merge clean up branch to it.
$ git merge clean_up

#delete a branch
$ git branch -d clean_up

#push the change on origin
$ git push

#git clone from a branch other than master
git clone -b Fix-1 --single-branch git://github.com/gnairooze/learning-cards.git

#change remote to point to https instead of git
git remote set-url origin https://github.com/gnairooze/learning-cards.git

#push current to remote branch instead of master
git push origin Fix-1:Fix-1

#when cloning repo you are clong all the branches.