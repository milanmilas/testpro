mkdir
cd ..
cd /c
ls
git init
git add
#only modified files
git add -u
#add all files
git add -A
git commti -m "this is the initial commit"
git status
#skipping the staging area
git commit -a -m
#renaming
git mv
git rm
git checkout -- 
git log
#press Q to exit
git log -p
git commit --amend
#reset cahnges in the stage/ unmodify files
git reset HEAD file
git checkout -- file

#with clone remoteNome= origin
git clone git://github.com/schacon/ticgit.git
git remote add pb git://github.com/paulboone/ticgit.git
git remote rename pb paul
git remote -v
#gets data from the remote to local repository, no merge
git fetch pb
#gets and merges data
git pull

git push origin master

#info
git remote show origin

git remote rm paul

git tag
git tag -a v1.4 -m 'my version 1.4'
git show v1.4
#tags are not pushed automatically
git push origin v1.5
#push all tags
it push origin --tags

git reset --HEAD~1
#changes will be returned to the staging area
git reset --soft HEAD~1

#remove files
git clean -f
#what remove command will do
git clean -n

git log --oneline
git log --oneline --graph
git shortlog
git log --format=short
#number of lines per user
git shortlog -sn
