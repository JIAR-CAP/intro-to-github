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

## Git

### What is Git?

Reference: https://git-scm.com/book/en/v2/Getting-Started-What-is-Git%3F

Cheatsheet: https://ndpsoftware.com/git-cheatsheet.html#loc=index

### Install Git

Download installer here: https://git-scm.com/downloads

One-time setup from your terminal (`macOS: Terminal` or `Windows: Git Bash`):

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

### Branching and merging

Create a new local branch:

```
git checkout -b my-new-branch
```

Make changes and commit:

```
git add .
git commit -m "commit on the new branch"
```

Switch back to the main branch:

```
git checkout main
```

Merge changes on branch back to main:

```
git merge my-new-branch
```

### Stashing Changes

Stash away changes temporarily (acts as a stack):

```
git stash
```

Restore the stashed changes:

```
git stash apply
```

### Git in VS Code

https://code.visualstudio.com/docs/sourcecontrol/intro-to-git

### Advanced CLI commands

* `git grep`: Grep, but ignores `.git/` and `.gitignore` matches
* `git diff HEAD~1`: diff HEAD against previous commit (adjust number as needed)
* **[x]** `git add -p`: add patches, allows staging only parts of your changes
* `git commit -p`: same as above, but also commit
* **[x]** `git rebase -i`: interactive rebase, reorder/merge/drop **local** commits
* **[x]** `git tag`: tagging commits (i.e., releases)
* `git show`: like `status` but shows latest commit message and content

### Future Topics

Worktrees, ???

## GitHub

### Prerequisite: Setup SSH

This simplifies connecting to GitHub.

1. Generate a new SSH key on your machine (choose platform): https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
2. Add the SSH key to your account: https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account

Clone the [playground repo](https://github.com/JIAR-CAP/intro-to-git-and-github-playground):

```
cd ~/repos/
git clone git@github.com:JIAR-CAP/intro-to-git-and-github-playground.git
cd intro-to-git-and-github-playground
```

### Push to GitHub

Commit a change, then:

```
git push
```

This will push the change up to the remote repo on GitHub. Verify by opening the repo page.

### Pull from GitHub

Make a change to the README on GitHub, then commit via UI. Go to your local repo:

```
git pull
```

Verify that you see the README commit locally.

### Create a Pull Request (PR): Add your username to the repo

Create a new branch locally:

```
git checkout -b add-my-username
```

Add your username to two places:

1. New file under the `add-your-username-file` folder.
2. Entry in `add-your-username.yml`

Commit & push to GitHub. Visit GitHub UI to create a new pull request (PR).

### Create a Pull Request (PR): Implement the multiply CLI in Python

Task: implement a `multiply` CLI subcommand and add a test for it.

Create a new branch:

```
git checkout -b multiply
```

Commit your change(s) to the branch, then push the branch to GitHub.

You can now open a PR and merge it. Explain: merge vs. squash.

### Create a Pull Request (PR) from a fork

1. Open an issue to add a new file under `attendees`.
2. Fork the main repo: https://github.com/JIAR-CAP/intro-to-git-and-github
3. Open a PR to add your name & close the issue you created.
    * Filename should match your username

### Future Topics

GH Actions, GH Pages, ???

## Resources

### Git

* Git book: https://git-scm.com/book/en/v2
* Git cheatsheet: https://ndpsoftware.com/git-cheatsheet.html#loc=index;

### GitHub

* GitHub cheatsheet: https://training.github.com/downloads/github-git-cheat-sheet.pdf 

