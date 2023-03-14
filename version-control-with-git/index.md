---
marp: true
title: Version Control; how to track what changed, who changed it, and why
paginate: true
---

# Version Control
how to track what changed, who changed it, and why

---

# TODO
✅ setup git to track changes in your `notes/` directory

(you will need install xcode command line tools `xcode-select --install`)

✅ make a commit

---


![bg contain](git-meme.png)

---

# Git is used by >90% of Fortune 100[*](https://octoverse.github.com)

![](git-companies.png)

---

# Scenario
* You're a software engineer working on a new feature 🧑‍💻
* You start writing code ✍️
* The app suddenly stops working ⚠️
* You try to remember which files you changed 🤷
* You wish there was an easy way to see and undo your changes 🧞‍♀️

---

![bg contain](./sourcetree-working.png)

---

![bg contain](./git-graph.png)

---

# Terms

* **Repository**
tracks and saves history of changes in a git project

* **Commit**
a snapshot in the repository timeline
* **Branch**
an independent version of the repository
* **Merge**
a git command that combines 2 branches into 1 branch

---

# Initialize a local git repository

We will be tracking changes in your `notes/` directory

Open a terminal and navigate to your `notes/` directory

Type in `git init` to setup a new git repository


___

# Status

Enter `git status` to see status of this repository

---

# Make a commit (cli)

1. Use `git add` to stage files you want to commit

    `git add .` If you want to add everything

2. `git commit -m "Initial commit"`


---
# Make a commit (vscode)

1. Open source control panel
2. Stage changes
3. Enter commit message
4. Click 'Commit'

---
# Commit Message

Commit messages help a future reader quickly understand what changed and why it changed

Please read this post on [Best Practices](https://initialcommit.com/blog/git-commit-messages-best-practices)

___

# Commit Message Examples

## Bad

`debugging`
`I added a delete route to the accounts controller`
`chanages`

## Good

`Enable logging globally`
`Add account delete route`


___

# Git GUI Tools
I **highly** recommend using a git GUI tool

vscode source control (with git graph)

[Sourcetree](https://sourcetreeapp.com)

[GitHub Desktop](https://desktop.github.com/)

---

# Resources

[git graph vscode extension](https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph)

[git cheatsheet](https://education.github.com/git-cheat-sheet-education.pdf)

