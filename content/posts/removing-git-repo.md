---
title: "Removing Git Repo"
date: 2023-03-24T11:05:32-07:00
draft: false
---

Sometimes you may accidentally create a GitHub repo where you weren't supposed to. It can happen when you can accidentally run '''git init''' in the wrong folder. You should be able to know if this happened if you notice files that aren't in your project folder being tracked by git. 

### How to fix
#### 1. Locate the the source directory of the your git repository. 
From your terminal, you can locate the directory of your git repo by running:
```
git rev-parse --show-toplevel
```
This will list you a file path with the location of the .git folder.
```
content/posts $ git rev-parse --show-toplevel
/Users/xavierloeraflores/Code/Projects/fsa-acc-resources
```
#### 2. Deleting the .git folder
Once you have navigated to directory containing the git repo, running the following command will delete the .git folder from your workspace. 
```
rm -rf .git
```
### 3. Ensuring the git repo has been removed
Running the ```git status``` command should output the following result if the .git folder was successfully deleted. 
```
Projects/fsa-acc-resources $ rm -rf .git
Projects/fsa-acc-resources $ git status
fatal: not a git repository (or any of the parent directories): .git
Projects/fsa-acc-resources $ 
```

Congrats. You just deleted the removed the git repository from you local machine. You may already accidentally pushed some files to GitHub. Double check your GitHub repos for any personal and private files and delete them accordingly. 

