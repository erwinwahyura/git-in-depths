# Git
## What is Git?

Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.


# Initialize Git Repo
Create a new sample project folder, run `git status` to see that is not yet a git repository. use `git init` to initialize it as a repository.

```git
$ mkdir sample

$ cd ~/sample

$ git status
fatal: not a git repository (or any of the parent directories): .git

$ git init
Initialized empty Git repository in /Users/erwinramadhan/Documents/learn/sample/.git/
```

# First Commit
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
