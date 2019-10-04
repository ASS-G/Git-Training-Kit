<h1 align="center">
  <br>
  Git and GitHub Training Kit
  <br>
</h1>

<p align="center">
  Sourced by Active Specialized Support Group (ASS-G)
</p>


## Install Git
GitHub provides desktop clients that include a graphical user interface for the most common repository actions and an automatically updating command line edition of Git for advanced scenarios.

#### GitHub Desktop
https://desktop.github.com/

Git distributions for Linux and POSIX systems are available on the official Git SCM website.

#### Git for all platforms
http://git-scm.com

## Configure tooling
Configure user information for all local repositories

$ git config --global user.name "[name]"

Sets the name you want attached to your commit transactions

$ git config --global user.email "[email address]"

Sets the email you want attached to your commit transactions

## Create repositories
Start a new repository or obtain one from an existing URL

```bash
$ git init [project-name]
```

Creates a new local repository with the specified name

```bash
$ git clone [url]
```

Downloads a project and its entire version history

## Make changes
Review edits and craft a commit transaction

```bash
$ git status
```

Lists all new or modified files to be committed

```bash
$ git diff
```

Shows file differences not yet staged

```bash
$ git add [file]
```

Snapshots the file in preparation for versioning

```bash
$ git diff --staged
```

Shows file differences between staging and the last file version

```bash
$ git reset [file]
```

Unstages the file, but preserves its contents

```bash
$ git commit -m"[descriptive message]"
```

Records file snapshots permanently in version history

## Group changes
Name a series of commits and combine completed efforts

```bash
$ git branch
```

Lists all local branches in the current repository

```bash
$ git branch [branch-name]
```

Creates a new branch

```bash
$ git checkout [branch-name]
```

Switches to the specified branch and updates working directory

```bash
$ git merge [branch-name]
```

Combines the specified branch’s history into the current branch

```bash
$ git branch -d [branch-name]
```

Deletes the specified branch

## Refactor file names
Relocate and remove versioned files

```bash
$ git rm [file]
```

Deletes the file from the working directory and stages the deletion

```bash
$ git rm --cached [file]
```

Removes the file from version control but preserves the file locally

```bash
$ git mv [file-original] [file-renamed]
```

Changes the file name and prepare it for commit

## Suppress tracking
Exclude temporary files and paths

```bash
*.log
build/
temp-*
```

A text file named .gitignore suppresses accidental versioning of files and paths matching the specified patterns

```bash
$ git ls-files --others --ignored --exclude-standard
```

Lists all ignored files in this project

## Save fragments
Shelve and restore incomplete changes

```bash
$ git stash
```

Temporarily stores all modified tracked files

```bash
$ git stash pop
```

Restores the most recently stashed files

```bash
$ git stash list
```

Lists all stashed changesets

```bash
$ git stash drop
```

Discards the most recently stashed changeset

## Review history
Browse and inspect the evolution of project files

```bash
$ git log
```

Lists version history for the current branch

```bash
$ git log --follow [file]
```

Lists version history for the file, including renames

```bash
$ git diff [first-branch]...[second-branch]
```

Shows content differences between two branches

```bash
$ git show [commit]
```

Outputs metadata and content changes of the specified commit

## Redo commits
Erase mistakes and craft replacement history

```bash
$ git reset [commit]
```

Undoes all commits after [commit], preserving changes locally

```bash
$ git reset --hard [commit]
```

Discards all history and changes back to the specified commit

## Synchronize changes
Register a remote (URL) and exchange repository history

```bash
$ git fetch [remote]
```

Downloads all history from the remote repository

```bash
$ git merge [remote]/[branch]
```

Combines the remote branch into the current local branch

```bash
$ git push [remote] [branch]
```

Uploads all local branch commits to GitHub

```bash
$ git pull
```

Downloads bookmark history and incorporates changes

###### [[Back to Top]](#----git-and-github-training-kit--)

![wave](http://cdn.thekrishna.in/img/common/border.png)
