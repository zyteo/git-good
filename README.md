# Get good at git
##### Just want to get better at git so let's git good! Just some commmands here and there for my own reference.

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
Git push\
Git checkout –b newbranchname (create new branch and switch to it)\
Git branch –d deletebranchname\
Git diff filename (check difference)\
Git add –p filename (add specific part of file)\
Might be handy: git status/git log/git remote –v\
git fetch and git pull are also important for getting the latest remote code\
NOTE git switch -c newbranchname & git checkout -b newbranchname are SIMILAR (not exactly the same. refer to [link](https://stackoverflow.com/questions/57265785/whats-the-difference-between-git-switch-and-git-checkout-branch))

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

##### Other references
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



