# Git Hands-on Exercise 1

## Check Git Version

```bash
git --version
```

Checks whether Git is installed and displays the installed version.

---

## View Global Git Configuration

```bash
git config --global --list
```

Displays the current global Git configuration, including username, email, and editor.

---

## Configure VS Code as the Default Git Editor

```bash
git config --global core.editor "code --wait"
```

Sets Visual Studio Code as the default editor used by Git.

---

## Verify the Configured Editor

```bash
git config --global core.editor
```

Displays the currently configured Git editor.

---

## Create a New Directory

```bash
mkdir GitDemo
```

Creates a new directory for the Git repository.

---

## Navigate to the Directory

```bash
cd GitDemo
```

Moves into the newly created project directory.

---

## Initialize a Git Repository

```bash
git init
```

Creates a new local Git repository.

---

## Check Repository Status

```bash
git status
```

Displays the current status of the repository.

---

## Create a Text File

```bash
echo "Welcome to the version control" > welcome.txt
```

Creates a file named `welcome.txt` with sample content.

---

## View File Contents

```bash
cat welcome.txt
```

Displays the contents of `welcome.txt`.

---

## Stage the File

```bash
git add welcome.txt
```

Adds the file to the Git staging area.

---

## Verify Staged Changes

```bash
git status
```

Confirms that the file has been staged for commit.

---

## Commit the Changes

```bash
git commit -m "Add welcome.txt"
```

Creates a commit with a descriptive commit message.

---

## Verify Working Tree

```bash
git status
```

Confirms that the working tree is clean and there are no pending changes.