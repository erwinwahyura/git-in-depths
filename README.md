# Git
## What is Git?

Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.


## Initialize Git Repo
Create a new sample project folder, run `git status` to see that is not yet a git repository. use `git init` to initialize it as a repository.

```git
$ mkdir sample

$ cd ~/sample

$ git status
fatal: not a git repository (or any of the parent directories): .git

$ git init
Initialized empty Git repository in /Users/erwinramadhan/Documents/learn/sample/.git/
```

## First Commit
Create a new document, stage it for a commit, then commit it to your repository.

```git
$ echo 'hello world' > sample.txt

$ git add sample.txt

$ git commit -m "initial commit" 
[main df56141] initial commit
 1 file changed, 1 insertion(+)
 create mode 100644 sample.txt

$ git push origin main
```

another way to add directs git to `save` a snapshot of the current project state  you can use `git add .` it means you add all the things to commit to your repository.

## Git Clone
Git clone is a Git command line utility which is used to target an existing repository and create a clone, or copy of the target repository. Cloning a local or remote repository. Cloning a bare repository. Using shallow options to partially clone repositories. Git URL syntax and supported protocols.

```git
$ git clone https://github.com/erwinwahyura/git-in-depths
Cloning into 'git-in-depths'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.

$ cd ~/git-in-depths
// start working on the projects

```

## Git Config
The git config command is a convenience function that is used to set Git configuration values on a global or local project level. These configuration levels correspond to .gitconfig text files. Executing git config will modify a configuration text file. We'll be covering common configuration settings like email, username, and editor. We'll discuss Git aliases, which allow you to create shortcuts for frequently used Git operations. Becoming familiar with git config and the various Git configuration settings will help you create a powerful, customized Git workflow.

```
$ git config user.email "erwinwahyura@gmail.com"
```

## Git Branch
Git branches are effectively a pointer to a snapshot of your changes. When you want to add a new feature or fix a bug—no matter how big or how small—you spawn a new branch to encapsulate your changes

The git branch command lets you create, list, rename, and delete branches. It doesn’t let you switch between branches or put a forked history back together again. For this reason, git branch is tightly integrated with the git checkout and git merge commands.

```git
$ git branch
*main

$ git branch <branch_name> // to create a new branch

$ git checkout <branch_name> // to move a branch

$ git branch -d <branch_name> // to delete a branch
```

## Git Merge
TBD

## Git Merge Conflict
TBD

## Merge Strategies
TBD

## Avoid Rebase Hell
TBD

## Tips
TBD