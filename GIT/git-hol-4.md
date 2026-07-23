# Git Hands-on Exercise 4

## Objective

- Learn how merge conflicts occur.
- Resolve merge conflicts.
- Update the `.gitignore` file.
- Delete the merged branch.

---

## 1. Verify Repository Status

```bash
git status
```

Checks whether the repository is in a clean state.

---

## 2. Create a New Branch

```bash
git branch GitWork
git switch GitWork
```

Creates and switches to the `GitWork` branch.

---

## 3. Create a File

```bash
echo "<message>Hello from GitWork</message>" > hello.xml
```

Creates a new file in the branch.

---

## 4. Stage and Commit

```bash
git add hello.xml
git commit -m "Add hello.xml in GitWork"
```

Commits the file to the branch.

---

## 5. Switch to the Main Branch

```bash
git switch master
```

> If your default branch is `main`, use:

```bash
git switch main
```

Returns to the primary branch.

---

## 6. Create the Same File with Different Content

```bash
echo "<message>Hello from Master</message>" > hello.xml
```

Creates the same file with different content.

---

## 7. Stage and Commit

```bash
git add hello.xml
git commit -m "Add hello.xml in master"
```

Commits the changes to the main branch.

---

## 8. View Commit History

```bash
git log --oneline --graph --decorate --all
```

Displays the commit history of all branches.

---

## 9. Compare Branches

```bash
git diff master GitWork
```

> If your default branch is `main`, use:

```bash
git diff main GitWork
```

Displays the differences between the branches.

---

## 10. Merge the Branch

```bash
git merge GitWork
```

Attempts to merge the branch into the current branch.

---

## 11. Resolve Merge Conflict

Open the conflicted file in Visual Studio Code, resolve the conflict, save the file, then stage it.

```bash
git add hello.xml
```

Marks the conflict as resolved.

---

## 12. Complete the Merge

```bash
git commit -m "Resolve merge conflict in hello.xml"
```

Creates the merge commit.

---

## 13. Update .gitignore

```text
*.bak
```

Adds backup files to the ignore list.

---

## 14. Stage and Commit

```bash
git add .gitignore
git commit -m "Ignore backup files"
```

Commits the updated `.gitignore`.

---

## 15. List Branches

```bash
git branch
```

Displays all local branches.

---

## 16. Delete the Merged Branch

```bash
git branch -d GitWork
```

Deletes the merged branch.

---

## 17. View Commit History

```bash
git log --oneline --graph --decorate
```

Displays the final commit history.