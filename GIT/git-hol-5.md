# Git Hands-on Exercise 5

## Objective

- Learn how to synchronize a local Git repository with a remote repository.
- Pull the latest changes from the remote repository.
- Push local commits to the remote repository.

---

## Connect Local Repository to GitHub

```bash
git remote add origin https://github.com/IHac-er/GitDemo.git
```

Adds the GitHub repository as the remote named `origin`.

---

## Verify the Remote Repository

```bash
git remote -v
```

Displays the configured remote repository for fetch and push operations.

---

## Push the Repository for the First Time

```bash
git push -u origin main
```

> If your default branch is `master`, use:

```bash
git push -u origin master
```

Pushes the local repository to GitHub and sets the upstream branch.

---