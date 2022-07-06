# Get good at git
##### Just want to get better at git so let's git good! Just some commmands here and there for my own reference.


For a new repo:\
git init\
git add README.md\
git commit -m "first commit"\
git branch -M main\
git remote add origin https://github.com/accountname/reponame.git \
git push -u origin main

Add folder which already has a git repo (i.e. already on git enterprise, want to make one in github)\
1.git remote add github(NOT origin) https://github.com/accountname/reponame.git \
2.git branch -M main\
3.git push -u github(NOT origin) main\
4.git remote –v should now show the different accounts
