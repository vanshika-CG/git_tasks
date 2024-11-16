## Task 1 : install and configure git
```
git config --global user.name "vanshika"
git config --global user.email "vanshika.jangamcg@gmail.com"
 ```
this command are used to store the info that who is committing the changes 

``` 
git config --list
```
this command will list all the config 
## Task 2 :initialize a repository
```
mkdir myproject
cd myproject
```
mdkir will make the new folder name "myproject" <br>
cd will navigate inside the folder
```
git init
```
this will initialize a repository
## Task 3 : create a file and make a multiple commits
```
echo "my first project" > README.md
```
create a mew file name "README.md" and with the content my first project
```
git add README.md
```
this will add the file to stagging area
```
git commit -m "initial commit :added README.md"
```
this  will commit file with  this "initial commit :added README.md" message
```
echo "added a description" >> README.md
```
this will make changes inside the content of README.md 
```
git add README.md
git commit -m "updated README with description"
```
git add will add file to stagging area and commit will commmit the file with the given message
## Task 4 : check status and log
```
git status
```
it will check the current status of repository
```
git log --oneline --graph --decorate
```
it will give commit history in detail
## Task 5: create and clone a repository
```
git clone http://codinggita.com/example-repo
```
this will clone codinggita repository locally in vs code
## Task 6: understanding the git workflow
```
echo "Workflow example" > workflow.md
```
create new file with name workflow.md with the given content
```
git add workflow.md
```
it will add this to stagging area
```
git commit -m "Added workflow example"
```
it will commit the file with given message
## Task 7: branching and merging 
```
git branch feature-login
git checkout feature-login
```
or use
```
git checkout -b feature-login
```
git branch will create branch and git checkout will switch the branch whereas git checkout -b will do both create and swith the branch

```
echo "login page" > login.html
git add login.html
git commit -m "Added login page"
```
it will create file with "login.html" name and with the given content and then it will add to stagging area then it  commit the file with the given message
```
git checkout main
git merge feature-login
```
git checkout will switch the branch and merge will merge the changes from feature-login to main branch
## Task 8: handling merge conflicts

