# Git Hands-on Exercise 2

## Objective

- Learn how to use `.gitignore`.
- Ignore unwanted files and folders from being tracked by Git.

---

## 1. Navigate to the Existing Repository

```bash
cd GitDemo
```

Moves to the existing Git repository.

---

## 2. Create a Log Folder

```bash
mkdir log
```

Creates a folder named `log`.

---

## 3. Create a Log File

```bash
echo "Application Started" > sample.log
```

Creates a sample log file.

---

## 4. Create a .gitignore File

```bash
touch .gitignore
```

Creates a `.gitignore` file.

---

## 5. Open the .gitignore File

```bash
code .gitignore
```

Opens the `.gitignore` file in Visual Studio Code.

---

## 6. Add Ignore Rules

```text
*.log
log/
```

Ignores all `.log` files and the `log` folder.

---

## 7. Verify Git Status

```bash
git status
```

Displays the repository status and verifies that ignored files are not tracked.

---

## 8. Stage the .gitignore File

```bash
git add .gitignore
```

Stages the `.gitignore` file.

---

## 9. Commit the Changes

```bash
git commit -m "Add .gitignore to ignore log files and folders"
```

Commits the `.gitignore` configuration.

---

## 10. Verify Repository Status

```bash
git status
```

Confirms that the working tree is clean.