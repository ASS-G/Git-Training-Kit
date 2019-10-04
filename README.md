<h1 align="center">
  <br>
  Git and GitHub Training Kit
  <br>
</h1>

<p align="center">
  Sourced by Active Specialized Support Group (ASS-G)
</p>

## Index
  1. [**Install Git**](#install-git)
  2. [**Configure tooling**](#configure-tooling)
  3. [**Create repositories**](#create-repositories)
  4. [**Make changes**](#make-changes)
  5. [**Group changes**](#group-changes)
  6. [**Review history**](#review-history)
  7. [**Redo commits**](#redo-commits)
  8. [**Synchronize changes**](#synchronize-changes)
  
  
## Install Git
GitHub provides desktop clients that include a graphical user interface for the most common repository actions and an automatically updating command line edition of Git for advanced scenarios.

#### GitHub Desktop
https://desktop.github.com/

Git distributions for Linux and POSIX systems are available on the official Git SCM website.

#### Git for all platforms
http://git-scm.com


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



###### [[Back to Top]](#----git-and-github-training-kit--)

![wave](http://cdn.thekrishna.in/img/common/border.png)
