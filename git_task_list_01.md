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

## Task 9: Renaming and deleting branches
```
git branch -m old-branch-name new-branch-name
```
it will rename the branch name
```
git branch-d feature-login
```
it will delete the branch 
## Task 10: using git stash
```
echo "Temporary work" >> temp.md
```
create new file with the given content
```
git stash
```
temporarily saves uncommited changes in git so we can work on something else without losing your progress
```
git stash list
```
display the list of all stashes currently saved in git repository
```
git stash apply
```
this used to reapply the changes saved in a stash
```
git stash drop
```
it is used to delete specific stash entry
# Task 11: Rewriting History with Interactive Rebase
```
echo "Commit 1" > file1.txt && git add file1.txt && git commit -m "Commit 1"
echo "Commit 2" > file2.txt && git add file2.txt && git commit -m "Commit 2"
echo "Commit 3" > file3.txt && git add file3.txt && git commit -m "Commit 3"
```
this will create three files file1.txt ,file2.txt ,file3.txt and will add to staging area and will commit
```
git rebase -i HEAD~3
```
this will help us to rewrite the last three commit in git branch 
# Task 12: Cherry-Picking Commits
```
git checkout -b cherry-pick-example
```
this will create new branch and switch to it immediately
```
git cherry-pick <commit-hash>
```
this allow to copy the changes from specific commit in one branch and apply them as a new commit to your current branch.
# Task 13: Tagging Commits
```
git tag -a v1.0 -m "Version 1.0 release"
```
This creates an annotated tag named v1.0 and associates it with the current commit, adding a message "Version 1.0 release."
```
git push origin v1.0
```
This pushes the tag v1.0 from your local Git repository to the remote repository (origin).
# Task 14: Working with Remote Repositories
```
git remote add origin <repository-url>
```
this connects local git repository to remote repository on platform like github
This pushes the commits in your local main branch to the remote repository's main branch on the remote named origin.
# Task 15: Forking and Contributing
```
git clone <forked-repo-url>
```
this will clone the repo code to your local
```
git checkout -b fix-typo
echo "Typo fixed" >> README.md
git add README.md
git commit -m "Fixed a typo"
git push origin fix-typo
```
it will create new branch and switch to it immediately and will create file nd add it to stagging area then will commit it with given message  and will push it to github
# Task 16: Simulate Team Collaboration

# Task 17: Git Ignore
```
echo "node_modules/" > .gitignore
```
create new file if not present at current repo
```
git add .
```
add to stagging area


