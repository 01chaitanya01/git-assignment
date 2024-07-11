# Git Assignment

This repository is a demonstration of the basic Git commands, workflow, and collaboration using GitHub.

## Project Setup

### Step 1: Setup Git Configuration

Configured Git with username and email:

```sh
git config --global user.name "username"
git config --global user.email "email@example.com"
```

### Step 2: Create a Local Repository

Initialized a new Git repository:

```sh
mkdir git-assignment
cd git-assignment
git init
```

### Step 3: Create a README File

Created a `README.md` file with initial content:

```sh
touch README.md
```

### Step 4: Add and Commit Changes

Staged and committed the `README.md` file:

```sh
git add README.md
git commit -m "Initial commit with README file"
```

### Step 5: Create a GitHub Repository

Created a new repository on GitHub named `git-assignment`.

### Step 6: Push Local Repository to GitHub

Linked local repository to GitHub and pushed changes:

```sh
git remote add origin https://github.com/01chaitanya01/git-assignment.git
git push -u origin master
```
