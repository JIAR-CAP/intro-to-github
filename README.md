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
* `git show`: like `status` but shows latest commit message and content
* `git stash` / `git stash apply`: stow away changes for later use
* `git diff HEAD~1`: diff HEAD against previous commit (adjust number as needed)
* `git add -i`: interactive staging, select multiple files to stage
* `git add -p`: add patches, allows staging only parts of your changes
* `git commit -p`: same as above, but also commit
* `git rebase -i`: interactive rebase, reorder/merge/drop **local** commits

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

