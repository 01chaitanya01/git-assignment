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
## Branching and Merging

### Step 1: Create a New Branch

Create a new branch named `feature` and switch to it:

```sh
git checkout -b feature
```

### Step 2: Create a New File

Create a new file `feature.txt` and add some content:

```sh
touch feature.txt
```

### Step 3: Add and Commit the New File

Add and commit the new file:

```sh
git add feature.txt
git commit -m "feature file added"
```

### Step 4: Switch Back to the Master Branch

Switch back to the master branch:

```sh
git checkout master
```

### Step 5: Merge the Feature Branch

Merge the `feature` branch into the `master` branch:

```sh
git merge feature
```

### Step 6: Push Changes to GitHub

Push the changes to GitHub:

```sh
git push origin master
```

This is a conflicting change.

## Handling Merge Conflicts

### Step 1: Create a New Branch

Create a new branch named `conflict` and switch to it:

```sh
git checkout -b conflict
```

### Step 2: Edit the README.md File (Conflict Branch)

Edit the `README.md` file to add conflicting content. For example, add the following line:


### Step 3: Add and Commit the Changes (Conflict Branch)

Add and commit the changes:

```sh
git add README.md
git commit -m "Add conflicting content to README.md"
```

### Step 4: Switch Back to the Master Branch

Switch back to the master branch:

```sh
git checkout master
```

### Step 5: Edit the README.md File (Master Branch)

Edit the `README.md` file to add different content that will conflict with the `conflict` branch. For example, add the following line:


### Step 6: Add and Commit the Changes (Master Branch)

Add and commit the changes:

```sh
git add README.md
git commit -m "Add different conflicting content to README.md"
```

### Step 7: Attempt to Merge the Conflict Branch into Master

Attempt to merge the `conflict` branch into `master`:

```sh
git merge conflict
```

### Step 8: Resolve the Merge Conflict

Open the `README.md` file. The conflicting changes will be marked like this:



Edit the file to resolve the conflicts and keep the necessary changes. For example:



### Step 9: Add the Resolved File

Add the resolved file:

```sh
git add README.md
```

### Step 10: Complete the Merge

Complete the merge:

```sh
git commit -m "Merge branch 'conflict'"
```

### Step 11: Push Changes to GitHub

Push the changes to GitHub:

```sh
git push origin master
```