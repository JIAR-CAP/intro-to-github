# Introduction to Git & GitHub

Playground repo: https://github.com/JIAR-CAP/intro-to-git-and-github-playground

## Outline

### Git

**Pre-req**: create your first GitHub repo to be used for rest of this section.

1. What is Git, brief history, motivation
2. Basic CLI commands: init/add/restore/commit/log
3. More commands
4. Branching
5. Using Git in VS Code
6. ???

### GitHub

1. Fork playground repo
2. Open an issue
3. Create a pull request (PR) from a local branch
4. Fork main repo
5. Create a pull request from the fork

Future topics: GH Actions, GH Pages, ???

## Git

### What is Git?

Reference: https://git-scm.com/book/en/v2/Getting-Started-What-is-Git%3F

Cheatsheet: https://ndpsoftware.com/git-cheatsheet.html#loc=index

### Install Git

Download installer here: https://git-scm.com/downloads

One-time setup:

```
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com

# Optional
git config --global init.defaultBranch main
```

### Create your first repo

```
mkdir -p ~/repos/hello-git

cd ~/repos/hello-git

git init .
```

### Basic CLI commands

* `git status`
* `git diff`
* `git add`
* `git restore [--staged]`
* `git commit -m`
* `git push`
* `git commit --amend`

### `.gitignore`

Use this to ignore files you don't want to track.

### Git in VS Code

### Branching

### Advanced CLI commands

* `git grep`: Grep, but ignores `.git/` and `.gitignore` matches
* **[x]** `git stash` / `git stash apply`: stow away changes for later use
* `git diff HEAD~1`: diff HEAD against previous commit (adjust number as needed)
* `git add -i`: interactive staging, select multiple files to stage
* **[x]** `git add -p`: add patches, allows staging only parts of your changes
* `git commit -p`: same as above, but also commit
* **[x]** `git rebase -i`: interactive rebase, reorder/merge/drop **local** commits
* **[x]** `git tag`: tagging commits (i.e., releases)
* `git show`: like `status` but shows latest commit message and content


## GitHub

Repo: https://github.com/JIAR-CAP/intro-to-git-and-github

> [!NOTE]
> **Instructor**: Mark the repo as public.

1. Open an issue to add a new file under `attendees`.
2. Fork the repo.
3. Open a PR to add your name & close the issue you created.
    * Filename should match your username

## Resources

### Git

* Git book: https://git-scm.com/book/en/v2
* Git cheatsheet: https://ndpsoftware.com/git-cheatsheet.html#loc=index;
* Intro to Git in VS Code: https://code.visualstudio.com/docs/sourcecontrol/intro-to-git

### GitHub

* GitHub cheatsheet: https://training.github.com/downloads/github-git-cheat-sheet.pdf 

