# Git Commands – VTU/AEC Lab (1 Credit)

### 1. Setting Up and Basic Commands

Task: Initialize a Git repository, create a file, stage it, and commit the changes.

```
# Initialize Git repository
git init

# Create a new file
touch README.md

# Add file to staging area
git add README.md

# Commit changes
git commit -m "Initial commit"
```

### 2. Creating and Managing Branches

Task: Create a feature branch, switch to master, and merge the feature branch into master.

```
# Create a new branch
git branch feature-branch

# Switch to master branch
git switch master

# Merge feature branch into master
git merge feature-branch
```

### 3. Stashing Changes

Task: Stash changes, switch branches, and apply the stashed changes.

```
# Stash current changes
git stash

# Switch to another branch
git switch feature-branch

# Apply stashed changes
git stash apply
```

### 4. Collaboration and Remote Repositories

Task: Clone a remote Git repository to your local machine.

```
git clone https://github.com/username/repository.git
```

### 5. Fetch and Rebase

Task: Fetch the latest changes from a remote repository and rebase the local branch onto the updated remote branch.

```
# Fetch latest changes
git fetch origin

# Rebase local branch onto remote master
git rebase origin/master
```

### 6. Merge with a Custom Commit Message

Task: Merge `feature-branch` into `master` with a custom commit message.

```
git switch master

git merge --no-ff -m "Merged feature branch into master" feature-branch
```

### 7. Git Tags and Releases

Task: Create a lightweight Git tag named `v1.0`.

```
git tag v1.0
```

To display the created tag:

```
git tag
```

### 8. Cherry-Pick a Range of Commits

Task: Cherry-pick a range of commits from `source-branch` into the current branch.

```
git cherry-pick <start-commit>^..<end-commit>
```

Note: This includes both the starting and ending commits.

### 9. View Details of a Specific Commit

Task: Display the author, date, commit message, and changes for a given commit ID.

```
git show abc123
```

### 10. Display Commits by Author Within a Date Range

Task: Display all commits made by author `JohnDoe` between January 1, 2025 and December 31, 2025.

```
git log --author="JohnDoe" --since="2025-01-01" --until="2025-12-31"
```

### 11. Display the Last Five Commits

Task: Display the last five commits in the repository history.

```
git log -5
```

### 12. Undo Changes Introduced by a Commit

Task: Undo the changes introduced by commit ID `abc123`.

```
git revert abc123
```

Note: `git revert` creates a new commit that reverses the changes introduced by the specified commit without deleting existing history.

## Quick Revision – Git Commands

| No. | Operation              | Git Command                |
| --- | ---------------------- | -------------------------- |
| 1   | Initialize repository  | `git init`                 |
| 2   | Stage a file           | `git add filename`         |
| 3   | Commit changes         | `git commit -m "message"`  |
| 4   | Create branch          | `git branch branch-name`   |
| 5   | Switch branch          | `git switch branch-name`   |
| 6   | Merge branch           | `git merge branch-name`    |
| 7   | Stash changes          | `git stash`                |
| 8   | Apply stash            | `git stash apply`          |
| 9   | Clone repository       | `git clone URL`            |
| 10  | Fetch changes          | `git fetch origin`         |
| 11  | Rebase                 | `git rebase origin/master` |
| 12  | Create lightweight tag | `git tag v1.0`             |
| 13  | Cherry-pick commits    | `git cherry-pick A^..B`    |
| 14  | View commit details    | `git show commit-id`       |
| 15  | View last five commits | `git log -5`               |
| 16  | Undo a commit          | `git revert commit-id`     |

