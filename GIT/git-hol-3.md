# Git Hands-on Exercise 3

## Objective

- Learn how to create and manage branches.
- Make changes in a branch.
- Merge a branch into the main branch.
- View commit history.
- Delete the merged branch.

---

## 1. View Existing Branches

```bash
git branch
```

Displays all local branches.

---

## 2. Create a New Branch

```bash
git branch GitNewBranch
```

Creates a new branch named `GitNewBranch`.

---

## 3. List All Local and Remote Branches

```bash
git branch -a
```

Displays all local and remote branches. The `*` indicates the currently active branch.

---

## 4. Switch to the New Branch

```bash
git switch GitNewBranch
```

Switches to the newly created branch.

---

## 5. Create a File

```bash
echo "This file was created in GitNewBranch." > branch.txt
```

Creates a new file in the branch.

---

## 6. Stage the File

```bash
git add branch.txt
```

Stages the file for commit.

---

## 7. Commit the Changes

```bash
git commit -m "Add branch.txt in GitNewBranch"
```

Creates a commit in the new branch.

---

## 8. Verify Repository Status

```bash
git status
```

Displays the repository status.

---

## 9. Switch Back to the Main Branch

```bash
git switch master
```

> If your default branch is `main`, use:

```bash
git switch main
```

Switches back to the primary branch.

---

## 10. Compare Branches

```bash
git diff master GitNewBranch
```

> If your default branch is `main`, use:

```bash
git diff main GitNewBranch
```

Displays the differences between the two branches.

---

## 11. Merge the Branch

```bash
git merge GitNewBranch
```

Merges `GitNewBranch` into the current branch.

---

## 12. View Commit History

```bash
git log --oneline --graph --decorate
```

Displays a compact graphical commit history.

---

## 13. Delete the Merged Branch

```bash
git branch -d GitNewBranch
```

Deletes the merged branch.

---

## 14. Verify Repository Status

```bash
git status
```

Confirms that the working tree is clean.