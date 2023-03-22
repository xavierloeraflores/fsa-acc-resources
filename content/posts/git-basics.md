---
title: "Getting Started with Git"
date: 2023-03-22T03:21:19-07:00
draft: false
---
This post introduces information relating to the basics of using git containing quick references for initializing a git repository, cloning a repository, and checking if you are currently within a git repository.  



## Checking for a git repository
The fastest way to know if you are currently within a git repository at your current directory is to run:

```
git status
```

You are not within a git repository if you see the following output: 
```
~ $ git status
fatal: not a git repository (or any of the parent directories): .git
~ $ 
```

Otherwise, you may see a variety of messages either mentioning that your current branch is up to date or that you have made changes that need to be committed. 

## Initializing a git repository
In order to create a git repository locally, you must navigate into your desire workspace folder and run the following command: 

```
git init
```

Alternatively, you can also log into your GitHub account and create a repository there. At that point, you can clone your repository locally. 

## Cloning a git repository
You can clone a GitHub repository by copying the SSH git url on GitHub. This url can be found the repository's GitHub page by clicking the green Code button on GitHub. 

Once you have the repository git url, you can clone it your computer by running:

```
git clone <repository url>
``` 

### Example
Let's say you wanted to clone this [repository](https://github.com/xavierloeraflores/SITE-Program-Prework). You would first click the Code button and copy the following git SSH url:

```
git@github.com:xavierloeraflores/SITE-Program-Prework.git
```

Once copied, you would navigate to your desired installation location and then run:

```
git clone git@github.com:xavierloeraflores/SITE-Program-Prework.git
```

