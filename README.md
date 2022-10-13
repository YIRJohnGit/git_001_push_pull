# Git Quick Reference Sheet #

## Git Installation if not found (Optional)##
```
sudo apt install -y git 
```

## …or create a new repository on the command line ##
```
mkdir test_pig_v01
cd test_pig_v01
git init # Initialiating the Git Repository

git config --global user.name "YIRJohnGit" # Specify the Author Name
git config --global user.email yirjohn@gmail.com # Specify the Git Registered Email

git add .
git commit -m "First commit"
git branch -M main
git remote add origin https://github.com/YIRJohnGit/hadoop_pig.git
git push -u origin main
```

## ...or push an existing repository from the command line ##
```
git remote add origin https://github.com/YIRJohnGit/hadoop_pig.git
git branch -M main
git push -u origin main
```

## ...cloing the Sample file from the GIT Repository ##
```
git clone https://github.com/YIRJohnGit/hadoop_pig.git
cd hadoop_pig
```

## ...pulling from remote github repository, make change or add more files of contents,  and then pushit to Githuub Repository##

_Creating New Directory in the Terminal_
```
mkdir test_pig
cd test_pig/

_Initializing Git with User Details_
git init # Initialiating the Git Repository
git config --global user.name "YIRJohnGit" # Specify the Author Name
git config --global user.email yirjohn@gmail.com # Specify the Git Registered Email
# git commit --amend --reset-author #Reset the Author Name

-Pull the remote repository to the local repository -
# git checkout main
git pull https://github.com/YIRJohnGit/hadoop_pig.git
ls -lshrt

_Making Change or Adding the contents or files_
``
echo "Hi" > index.html
``
_Adding the Change to the Local Repository_
```
git add . # Adding the Git in Local Repo
git commit -am "first update..." # Committing the File
git status
```
_Add the branch and Pushing to the Remote repository_
```
git remote add "master" git@github.com:YIRJohnGit/hadoop_pig.git
git push --set-upstream https://github.com/YIRJohnGit/hadoop_pig.git master
```
_Result_ 
![image](https://user-images.githubusercontent.com/111234771/195471429-9e85f615-d1e6-419a-a0cf-19265c23f631.png)
