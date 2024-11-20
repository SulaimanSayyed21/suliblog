---
date: "2024-01-12"
draft: false
title: "Git Commands"
categories:
  - "Programming Languages"
description: "The most used git commands."
tags:
  - "bash"
  - "shell"
series:
  - "bash"
images:
  - "gitcm.webp"
featured: true 

authors: 
  - Sulaiman
---



### **Essential Git Commands**

Git is an essential tool for version control in software development, allowing teams to track changes, collaborate efficiently, and manage project histories. Whether you're working on a solo project or collaborating with a team, mastering Git commands is key to navigating and managing repositories. This guide highlights the most essential Git commands, helping you get started with version control and streamline your workflow with Git.


## Git Configuration Commands

### `git config`
```bash
git config [options]
```
Configures Git settings.

#### Options:
- `--global`: Applies the configuration globally for the user.
- `--local`: Applies the configuration for the current repository.

#### Example:
- Set your name:
  ```bash
  git config --global user.name "Your Name"
  ```
- Set your email:
  ```bash
  git config --global user.email "your.email@example.com"
  ```

---

## Repository Initialization and Status Commands

### `git init`
```bash
git init
```
Initializes a new Git repository in the current directory.

#### Example:
```bash
git init
```

---

### `git status`
```bash
git status
```
Displays the status of the working directory and staging area, including changes to tracked files and untracked files.

#### Example:
```bash
git status
```

---

## Adding and Committing Changes

### `git add`
```bash
git add [file_or_directory]
```
Adds files or directories to the staging area.

#### Example:
- Add a specific file:
  ```bash
  git add file.txt
  ```
- Add all files in the current directory:
  ```bash
  git add .
  ```

---

### `git commit`
```bash
git commit -m "commit message"
```
Records changes to the repository with a descriptive message.

#### Example:
```bash
git commit -m "Add feature X"
```

---

## Branching and Merging

### `git branch`
```bash
git branch [branch_name]
```
Creates a new branch.

#### Example:
```bash
git branch feature-branch
```

---

### `git checkout`
```bash
git checkout [branch_name]
```
Switches to a different branch.

#### Example:
```bash
git checkout feature-branch
```

---

### `git merge`
```bash
git merge [branch_name]
```
Merges changes from the specified branch into the current branch.

#### Example:
```bash
git merge feature-branch
```

---

## Remote Repository Commands

### `git clone`
```bash
git clone [repository_url]
```
Clones a remote repository to your local machine.

#### Example:
```bash
git clone https://github.com/user/repo.git
```

---

### `git remote`
```bash
git remote [options]
```
Manages connections to remote repositories.

#### Options:
- `add`: Adds a remote repository.
- `remove`: Removes a remote repository.
- `-v`: Shows the URLs of remote repositories.

#### Example:
- Add a remote repository:
  ```bash
  git remote add origin https://github.com/user/repo.git
  ```

---

### `git pull`
```bash
git pull [remote] [branch]
```
Fetches and integrates changes from a remote repository into the current branch.

#### Example:
```bash
git pull origin main
```

---

### `git push`
```bash
git push [remote] [branch]
```
Uploads changes from your local repository to a remote repository.

#### Example:
```bash
git push origin main
```

---

## Viewing and Undoing Changes

### `git log`
```bash
git log
```
Shows the commit history.

#### Example:
```bash
git log
```

---

### `git diff`
```bash
git diff
```
Displays differences between the working directory and the staging area.

#### Example:
```bash
git diff
```

---

### `git reset`
```bash
git reset [options]
```
Resets the current branch to a specific state.

#### Options:
- `--soft`: Keeps changes staged.
- `--mixed`: Keeps changes in the working directory (default).
- `--hard`: Discards all changes.

#### Example:
```bash
git reset --hard HEAD~1
```

---

### `git revert`
```bash
git revert [commit_hash]
```
Creates a new commit that undoes the changes from a specific commit.

#### Example:
```bash
git revert abc1234
```

---

## Stashing Changes

### `git stash`
```bash
git stash
```
Saves uncommitted changes for later use.

#### Example:
```bash
git stash
```

---

### `git stash apply`
```bash
git stash apply
```
Restores the most recently stashed changes.

#### Example:
```bash
git stash apply
```

---

