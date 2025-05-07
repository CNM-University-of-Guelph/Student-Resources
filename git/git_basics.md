# Git Basics

Now that Git is installed and configured, this page walks you through the core concepts and actions you'll use when working with Git. These basics will help you manage your own projects and contribute to shared repositories like those on GitHub.

## **What Is a Git Repository?**

A **Git repository** (or _repo_) is a folder that Git is tracking. Once a folder has been initialized as a repository, Git begins recording the history of any changes made to the files inside.

To create a Git repository in an existing folder in the project folder terminal run:

```bash
git init
```

This sets up version control in the folder, allowing you to start tracking your work over time.

## **Staging and Committing Changes**

Git monitors changes to your files, but it does not automatically record those changes in your project's history. Instead, it uses a two-step process to decide which changes to include:

1. **Staging** marks specific files or changes that you want to save.
2. **Committing** takes a snapshot of the staged changes and adds it to your version history, along with a message describing what changed.

```bash
git add filename.py       # Stage a specific file
git add .                 # Stage all changed files
git commit -m "commit message"  # Commit the staged changes
```

Each commit is like a version of your project at a specific point in time. You can view your project’s history or revert to earlier versions using these commits.

## **What Is a Branch and Why Use It?**

A **branch** is a parallel version of your project where you can make changes independently of the main version. This is especially useful when developing new features, testing changes, or fixing issues without disrupting the main codebase.

To create and switch to a new branch:

```bash
git checkout -b new-feature
```

To switch back to the main branch:

```bash
git checkout main
```

## **Working with GitHub (Push & Pull)**

Although Git works locally on your computer, it is often paired with GitHub — an online platform for hosting Git repositories. Once your local repository is connected to a GitHub repository, you can:

- **Push** your commits to GitHub (upload changes)
- **Pull** the latest changes from GitHub (download updates)

Example push command:

```bash
git push origin branch-name
```

Example pull command:

```bash
git pull origin branch-name
```

To connect your local project to GitHub, refer to this guide: [Managing remote repositories](https://docs.github.com/en/get-started/getting-started-with-git/managing-remote-repositories)

## **What Is a Pull Request (PR)?**

A **pull request** is a formal way of proposing changes to a project on GitHub. It allows collaborators to review, discuss, and approve updates before they are merged into the main branch.

Typical steps:

1. Make changes in a separate branch (e.g. `fix-bug`)
2. Push the branch to GitHub
3. Click “Compare & pull request” on GitHub
4. Submit the PR with a description of your changes

Pull requests are essential for collaborative projects, but they are also helpful when working independently to organize and track your progress.

## **Merging Changes**

Once the changes in a branch are complete and reviewed (typically via a pull request), they can be **merged** into the main branch.

To merge changes locally:

```bash
git checkout main
git merge new-feature
```

You can then delete the feature branch to keep your project organized:

```bash
git branch -d new-feature
```

## **Pulling Latest Changes**

To make sure your local project stays up-to-date with the latest changes on GitHub, use:

```bash
git pull origin main
```

This downloads and integrates any new commits from the remote repository.

## **Summary of Common Git Commands**

| Task                              | Command                              |
| --------------------------------- | ------------------------------------ |
| Initialize a Git repository       | `git init`                           |
| Check file status                 | `git status`                         |
| Stage file(s) for commit          | `git add filename.py` or `git add .` |
| Commit staged changes             | `git commit -m "Your message"`       |
| View commit history               | `git log`                            |
| Create and switch to a new branch | `git checkout -b branch-name`        |
| Switch to an existing branch      | `git checkout branch-name`           |
| Push changes to GitHub            | `git push origin branch-name`        |
| Pull updates from GitHub          | `git pull origin branch-name`        |
| Merge another branch              | `git merge other-branch`             |
