Here are all the **Git commands** related to the **branching concept**:

### 1. **Branch Creation, Listing, and Deletion**

- **Create a new branch:**
  ```bash
  git branch <branch-name>
  ```

- **List all branches:**
  ```bash
  git branch
  ```
  - To list both local and remote branches:
    ```bash
    git branch -a
    ```

- **Delete a branch (local):**
  ```bash
  git branch -d <branch-name>
  ```
  - Force delete if the branch is not fully merged:
    ```bash
    git branch -D <branch-name>
    ```

- **Delete a branch (remote):**
  ```bash
  git push origin --delete <branch-name>
  ```

### 2. **Switching Branches**

- **Switch to an existing branch:**
  ```bash
  git checkout <branch-name>
  ```

- **Switch to a new branch and create it at the same time:**
  ```bash
  git checkout -b <branch-name>
  ```

- **Switch branches using the newer syntax (Git 2.23+):**
  ```bash
  git switch <branch-name>
  ```

- **Create a new branch and switch to it (Git 2.23+):**
  ```bash
  git switch -c <branch-name>
  ```

### 3. **Merging Branches**

- **Merge a branch into the current branch:**
  ```bash
  git merge <branch-name>
  ```

- **Abort a merge (if there are conflicts):**
  ```bash
  git merge --abort
  ```

### 4. **Rebasing**

- **Rebase the current branch onto another branch:**
  ```bash
  git rebase <branch-name>
  ```

- **Abort a rebase:**
  ```bash
  git rebase --abort
  ```

- **Continue after resolving conflicts during rebase:**
  ```bash
  git rebase --continue
  ```

### 5. **Tracking Remote Branches**

- **Create a branch that tracks a remote branch:**
  ```bash
  git checkout --track origin/<branch-name>
  ```

- **Push a local branch to a remote and set it to track the remote branch:**
  ```bash
  git push -u origin <branch-name>
  ```

- **List all branches with their remote tracking information:**
  ```bash
  git branch -vv
  ```

### 6. **Renaming a Branch**

- **Rename the current branch:**
  ```bash
  git branch -m <new-branch-name>
  ```

- **Rename a different branch:**
  ```bash
  git branch -m <old-branch-name> <new-branch-name>
  ```

### 7. **Comparing Branches**

- **View differences between two branches:**
  ```bash
  git diff <branch1> <branch2>
  ```

### 8. **Stashing Changes (before switching branches)**

- **Stash changes:**
  ```bash
  git stash
  ```

- **Apply stashed changes:**
  ```bash
  git stash apply
  ```

- **List all stashes:**
  ```bash
  git stash list
  ```

### 9. **Pulling and Fetching**

- **Pull changes from a remote branch:**
  ```bash
  git pull origin <branch-name>
  ```

- **Fetch changes from the remote without merging:**
  ```bash
  git fetch origin <branch-name>
  ```

These are the most commonly used commands related to Git branching.
