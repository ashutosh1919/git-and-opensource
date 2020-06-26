# Git Tutorial
This repository is made for the illustration purpose to learn git during the workshop. It includes repository creation, fork, clone, add, commit, push, branching, merge, pull request and issue creation.

## Git
- Git is Version Control System used to manage project so that it can easily track the code changes.
- Download git into your system from [here](https://git-scm.com/downloads).

## Create Repository
- Go to [Github](https://github.com/) and Login to your account.
- Create new repository by clicking `New` button over left top.
- Give project name as `testGit` and write any discription if you want.
- Check `Initialize this repository with a README`.
- Click `Create Repository`.

## Fork
- You can copy any repository (Other than your own) into your github using fork.
- To fork any repository, you can go to that repository and you can press `Fork` button on the top right corner.

## Clone
- To clone the repository into your local system, execute the following code.
- `git clone https://github.com/<your-github-username>/testGit.git`
- This will create the folder `testGit` into current working directory of your system.
- This folder is the local copy of that repository.

## Add, Commit, Push
- Update `README.md` file and add description `My name is Ashutosh` at the end of file.
- Now, our objective is to push these changes to remote branch over github.
- First we need to add these changes to local repository and we can do that using `git add .`. Note here that `.` represents that we are adding all changed files to our local repository.
- Secondly, we need to commit these added files to local repository using `git commit -m "Write the commit message here"`.
- To push the changes, give command `git push origin master`.

## Branch Creation
- You can see the branches using `git branch` command. The branch with the asterisk(*) is the current branch.
- Now, create a new branch using `git checkout -b new_branch`. It will create new branch and it will navigate the local repository to `new_branch`.

## Creating Pull Request
- Go to `README.md` and add `I am Indian` at the end of file.
- Save the file and execute following commands to push the new branch to your remote repository.
- `git add .`
- `git commit -m "New branch created"`
- `git push origin new_branch`
- Click on `Compare & Pull Request` on the repository page.
- Create Pull Request and Merge it.

## Pull The Changes
- `git pull` into master branch of your local repository.

## Delete Branch
- Delete the local branch using `git branch -d new_branch`. It will delete the branch.

## Merge
- Create new branch as `branch_1` using `git checkout -b branch_1`.
- Create a new file `Contribute.md` and write `Contributing to opensource.` in it.
- Now add and commit changes to `branch_1` using `git add .` and `git commit -m "Changes to be merged"`.
- Checkout to `master` branch using `git checkout master`.
- Execute `git merge branch_1` to merge `branch_1` to `master`.

## Issue Creation
- You can find `Issues` Section in each repository where you can create issues if you find the bug into code.
- You can also create issue for new feature requests.
