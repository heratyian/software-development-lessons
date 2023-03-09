---
marp: true
title: Running Ruby On Your Own Machine
paginate: true
---

# Running Ruby On Your Own Machine

---
# TODO

1. Play around with `irb`

2. Create `Workspace/scratch` folder

3. Setup and configure your code editor (vscode)

4. Write and run a ruby program on your machine

---

# Terminal
open your terminal
<!-- command + space (open spotlight search) -->
<!-- search 'terminal', press `enter` -->

---

# Ruby
Ruby comes preinstalled on macOS

`ruby --version` or `ruby -v` to check version

This is your system ruby. You'll need to install different versions when developing rails applications. We'll get into this later.

Make sure you are using the correct version in [Ruby Docs](https://ruby-doc.org/) 


---

## Interactive Ruby (irb)

type in `irb`

play around with ruby

type `exit` to exit irb shell

---

# Create `scratch/` Folder

<!-- root path ~ -->
Enter `open .` in terminal window to open Finder

Create `Workspace/scratch/` folder

We can keep experimental ruby scripts in `scratch/`

---

# Setup vscode

[vscode](https://code.visualstudio.com/) is a code editor that works well with ruby, rails, and pretty much any language

1. Open vscode

2. File -> Open Folder... -> (click `Workspace/scratch/` folder)

---

# Create And Run Ruby File
<!-- we should be in vscode scratch folder -->
Create `hello.rb` file in `scratch/`

Open `hello.rb` in vscode
  * ⌘ + p to open vscode file search
  * type in filename `hello.rb`

create program that asks for name and says hello

```ruby
print 'What is your name? '
name = gets.chomp
puts "Hello #{name}"
```

Enter `ruby hello.rb` in the terminal

---

# Download Treehouse Workspace
* Click `File`, `Download Workspace`

![bg right](treehouse-workspace.png)

---

# Resources

## vscode
[install vscode](https://code.visualstudio.com/)
[Ruby Extension](https://marketplace.visualstudio.com/items?itemName=rebornix.Ruby)
[HTML CSS Support Extension](https://marketplace.visualstudio.com/items?itemName=ecmel.vscode-html-css)
[GitLens Extension](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)


## Ruby Docs
[Ruby Docs](https://ruby-doc.org/)

## Unix
[Commands Cheatsheet](https://www.alexji.com/UNIXCheatSheet.pdf)

---

## 1337 Hacker

Install xcode command line tools `xcode-select --install`

[Install multiple Ruby versions with rbenv](https://github.com/rbenv/rbenv)
