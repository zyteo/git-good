# Get good at git
##### Just want to get better at git so let's git good! Just some commmands here and there for my own reference.

Set git username and email for all repos\
git config --global user.name "username"\
git config --global user.email "email@mail.com"

For a new repo:\
git init\
git add README.md\
git commit -m "first commit"\
git branch -M main\
git remote add origin https://github.com/accountname/reponame.git \
git push -u origin main

Add folder which already has a git repo (i.e. already on git enterprise, want to make one in github):\
git remote add github(NOT origin) https://github.com/accountname/reponame.git \
git branch -M main\
git push -u github(NOT origin) main\
git remote –v should now show the different accounts

Just some notes:\
git add . or add –a\
git add -u to exclude untracked changes. refer [link](https://stackoverflow.com/questions/572549/difference-between-git-add-a-and-git-add)\
git reset (to undo git add)\
Git commit –m “message” / git commit (for subject+details)\
git commit --amend -m "New message" (to modify message that has already been pushed)\
git commit --amend also works\
Git push\
Git checkout –b newbranchname (create new branch and switch to it)\
Git branch –d deletebranchname\
Git diff filename (check difference)\
Git add –p filename (add specific part of file)\
Might be handy: git status/git log/git remote –v\
git fetch and git pull are also important for getting the latest remote code\
git pull is a git fetch + git merge. Use with caution.\
to avoid using git pull:\
git fetch\
git merge branchToMerge\
*make changes to conflicts

once changes made, as per usual\
git add/commit/push\
git merge --abort to stop process\
NOTE git switch -c newbranchname & git checkout -b newbranchname are SIMILAR (not exactly the same. refer to [link](https://stackoverflow.com/questions/57265785/whats-the-difference-between-git-switch-and-git-checkout-branch))\
git stash (to 'save' work in progress changes, but not wanting to push to repo. refer to [link](https://git-scm.com/docs/git-stash))

Git clone:\
git clone https://github.com/accountname/reponame.git \
cd reponame\
git branch -a (to see all branches)

When doing a git clone, and want to make a new branch and continue from there:\
git checkout -b branchname OR git switch -c newbranchname\
git add whatever files\
git commit -m "msg"\
git push --set-upstream origin branchname

Alternatively, doing a git clone, and want to continue from existing branch:\
git checkout existingbranchname\
edit files\
git add files\
git commit -m "msg"\
git push

deleting a local or remote branch\
git branch -d localBranchName\
git push origin --delete remoteBranchName

want to add everything except a particular file\
git add .\
git reset link/to/the/file.extension\
git commit -m "message as per usual"\
git push

##### Other references

Obtain cursor position
```
Add-Type -AssemblyName System.Windows.Forms
$X = [System.Windows.Forms.Cursor]::Position.X
$Y = [System.Windows.Forms.Cursor]::Position.Y
Write-Output "X: $X | Y: $Y"
```
Robo copy files excluding certain dirs
```
$source = "D:\Filepath"
$destination = "E:\Filepath"
$excludeDirs = "node_modules"

# Robocopy command
robocopy $source $destination /E /XD $excludeDirs
```
React\
npx create-react-app appname\
cd appname\
npm install react-router-dom react-router\
npm start

npm init vite@latest nameofapp -- --template react\
npm install\
npm run dev

Django\
Py manage.py makemigrations/migrate/check\
Py manage.py startapp xxx

Ubuntu cmd:\
sudo apt-get update && sudo apt-get upgrade (gets updates + upgrades)\
sudo apt-get install –y nameOfPgrm (install pgrm, default yes)\
sudo apt-get purge nameOfProgram\
sudo apt-get autoremove

VIM\
hjkl cursor\
:q! exit\
x delete\
i insert then ESC (normal mode)\
A (remember to shift a) to append text\
:wq save file and exit\
dw delete word\
d$ delete to end of line\
2w move forward 2 words\
3e move forward 3 words, to end of 3rd work\
0 move start line\
$ end of line\
:0 beginning of file\
:$ end of file\
d3w delete 3 words\
dd delete 1 line\
2dd delete 2 lines\
u undo last action\
2u undo last 2 actions\
U undo changes to one line\
Ctrl+r redo commands\
p put previously deleted text below the cursor\
rx replace character at cursor with x\
ce change until end of the word. ce + text + ESC\
c$ change until end of line\
:%s/the/THE/g replaces all the with THE\
Ctrl G shows location in file + file status\
Ctrl G G moves to bottom of file\
Ctrl G gg moves to start of file\
Ctrl G 100G moves to 100th line\
/ word ENTER search for word clockwise\
? word ENTER search for word anti clockwise\
n next word\
N next word in backwards direction\
Ctrl O go back where you came from\
Ctrl I go forward where you came from\
% to find a matching ), ], }



