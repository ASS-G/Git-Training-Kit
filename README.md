<h1 align="center">
  <br>
  Git and GitHub Training Kit
  <br>
</h1>

<p align="center">
  Sourced by Active Specialized Support Group (ASS-G)
</p>

## Index
  1. [**What Is Version Control?**](#what-is-version-control)
  2. [**What Is Git?**](#what-is-git)
  3. [**Getting Started**](#getting-started)
  4. [**Configure tooling**](#configure-tooling)
  5. [**Create repositories**](#create-repositories)
  6. [**Make changes**](#make-changes)
  7. [**Group changes**](#group-changes)
  8. [**Review history**](#review-history)
  9. [**Redo commits**](#redo-commits)
  10. [**Synchronize changes**](#synchronize-changes)
  11. [**Workflow Summary**](#workflow-summary)
  
  
## What Is Version Control?
Version control helps developers track and manage changes to a software project’s code. As a software project grows, version control becomes essential. Take WordPress…

At this point, WordPress is a pretty big project. If a core developer wanted to work on one specific part of the WordPress codebase, it wouldn’t be safe or efficient to have them directly edit the “official” source code.

Instead, version control lets developers safely work through **branching** and **merging**.

With **branching**, a developer duplicates part of the source code (called the repository). The developer can then safely make changes to that part of the code without affecting the rest of the project.

Then, once the developer gets his or her part of the code working properly, he or she can **merge** that code back into the main source code to make it official.

All of these changes are then tracked and can be reverted if need be.


## What Is Git?
Git is a specific **open-source version control system** created by Linus Torvalds in 2005.

Specifically, Git is a distributed version control system, which means that the entire codebase and history is available on every developer’s computer, which allows for easy branching and merging.

According to a Stack Overflow developer survey, **over 87% of developers use Git**.


## Getting Started 
Follow the instructions [here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) to install git (if it's not already installed). Note that for this tutorial we will be using git on the command line only. While there are some great git GUIs (graphical user interfaces), We think it's easier to learn git using git-specific commands first and then to try out a git GUI once you're more comfortable with the command. 


### Install Git
Git distributions for Linux and POSIX systems are available on the official Git SCM website.

#### Git for all platforms (Recommended) 
http://git-scm.com

Alternatively, GitHub provides desktop clients that include a graphical user interface for the most common repository actions.

#### GitHub Desktop
https://desktop.github.com/


## Configure tooling
##### Configure user information for all local repositories

Sets the name you want attached to your commit transactions
```bash
$ git config --global user.name "[name]"
```

Sets the email you want attached to your commit transactions
```bash
$ git config --global user.email "[email address]"
```

## Create repositories
##### Start a new repository or obtain one from an existing URL

Creates a new local repository with the specified name
```bash
$ git init [project-name]
```

Downloads a project and its entire version history
```bash
$ git clone [url]
```


## Make changes
##### Review edits and craft a commit transaction

Lists all new or modified files to be committed
```bash
$ git status
```

Shows file differences not yet staged
```bash
$ git diff
```

Snapshots the file in preparation for versioning
```bash
$ git add [file]
```

Shows file differences between staging and the last file version (file in previous commit)
```bash
$ git diff --staged
```

Unstages the file, but preserves its contents
```bash
$ git reset [file]
```


## Group changes
##### Name a series of commits and combine completed efforts

Lists all local branches in the current repository
```bash
$ git branch
```

Creates a new branch
```bash
$ git branch [branch-name]
```

Switches to the specified branch and updates working directory
```bash
$ git checkout [branch-name]
```

Combines the specified branch’s history into the current branch
```bash
$ git merge [branch-name]
```

Deletes the specified branch
```bash
$ git branch -d [branch-name]
```


## Review history
##### Browse and inspect the evolution of project files

Lists version history for the current branch
```bash
$ git log
```

Lists version history for the file, including renames
```bash
$ git log --follow [file]
```

Outputs metadata and content changes of the specified commit
```bash
$ git show [commit]
```


## Redo commits
##### Erase mistakes and craft replacement history

Undoes all commits after [commit], preserving changes locally
```bash
$ git reset [commit]
```

Discards all history and changes back to the specified commit
```bash
$ git reset --hard [commit]
```


## Synchronize changes
##### Register a remote (URL) and exchange repository history

Downloads all history from the remote repository
```bash
$ git fetch [remote]
```

Combines the remote branch into the current local branch
```bash
$ git merge [remote]/[branch]
```

Uploads all local branch commits to GitHub
```bash
$ git push [remote] [branch]
```

Downloads bookmark history and incorporates changes
```bash
$ git pull
```

## Workflow Summary
You now have everything you need to successfully clone a repository, create a branch, make changes, and push those changes up to a master branch. Your workflow should look something like this:
- `git clone <url>` (clone a Git repository)
- `cd` (change directory) into your newly cloned repository
- `git checkout -b <branch-name`> (create and switch to your new branch)
- `git status`(the output of this should be pretty boring right now)
- make your changes
- `git status` (you should see a list of the files you changed now)
- `git diff` (make sure you actually want these changes)
- `git add` (add your changes to your staging index)
- `git status` (yes, it’s my favorite command, do it)
- `git commit` (commit your changes)
- `git push` (push your changes up to the remote branch)
- merge your changes in GitHub or other cloud VCS services
- `git checkout master` (switch back to the master branch)
- `git pull` (pull down the changes your just merged)
- `git status` (just to make sure everything is nice and clean)
- repeat! (except step 1, you only need to clone once)


###### [[Back to Top]](#----git-and-github-training-kit--)

![wave](http://cdn.thekrishna.in/img/common/border.png)
