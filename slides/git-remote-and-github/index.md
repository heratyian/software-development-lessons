---
marp: true
title: Git Remote and GitHub
paginate: true
---
# Git Remote and GitHub

---
# TODO

✅ Push your notes to a remote repository on GitHub

✅ Push your GitPod workspace to GitHub


---
# Scenario

* Working on a project 👨‍💻
* Want to go home and work on it from a different computer 🏠
* Need to access and sync with the latest version 🤨


---
# Create Repository on GitHub

[Create New Repository](https://github.com/new)

![contain](github-repo.png)


---

# Add remote and push (CLI)

```
git remote add origin <your-repository-url.git>
git branch -M main
git push -u origin main
```

---

# Create remote repository and push (VSCode)

![bg right 75%](./vscode-publish-branch.jpg)

Follow wizard to create a new repository and push

---

# Resources

[Create personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token#creating-a-personal-access-token-classic)

[Using personal access token in CLI](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token#using-a-personal-access-token-on-the-command-line)