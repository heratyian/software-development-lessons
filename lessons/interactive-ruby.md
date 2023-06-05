# Interactive Ruby
This lesson goes over interactive ruby (irb): why and how we use it

<!-- TODO: update slides -->
## [Slides](../slides/interactive-ruby/index)

## Topics
- Ruby

## Interactive Ruby
- You're working on a coding problem 🧑‍💻.
- You need to test and experiment with small snippets of Ruby code quickly and interactively test an idea.
- Luckily, you have the IRB shell 🪄✨.
- In the IRB shell, you can try out lines of Ruby code and see the results immediately, without the need for writing and running a whole program.
- It's like having a virtual playground where you can experiment and explore the capabilities of Ruby in real-time ⚙️🔬.
- With each session in the IRB shell, your skills grow stronger, and you'll become more confident in your ability to write robust and efficient Ruby code 💪💎.


### Locally


### Replit

https://replit.com/



# TODO

1. Play around with `irb`
2. Create `Workspace/scratch` folder
3. Setup and configure your code editor (vscode)
4. Write and run a ruby program on your machine



# Terminal
open your terminal
<!-- command + space (open spotlight search) -->
<!-- search 'terminal', press `enter` -->



# Ruby
Ruby comes preinstalled on macOS

`ruby --version` or `ruby -v` to check version

This is your system ruby. You'll need to install different versions when developing rails applications. We'll get into this later.

Make sure you are using the correct version in [Ruby Docs](https://ruby-doc.org/) 




## Interactive Ruby (irb)

type in `irb`

play around with ruby

type `exit` to exit irb shell







# Setup vscode

[vscode](https://code.visualstudio.com/) is a code editor that works well with ruby, rails, and pretty much any language

1. Open vscode

2. File -> Open Folder... -> (click `Workspace/scratch/` folder)



# Create And Run Ruby File
<!-- we should be in vscode scratch folder -->
Create `hello.rb` file in `scratch/`

Open `hello.rb` in vscode
  1. ⌘ + p to open vscode file search
  2. type in filename `hello.rb`

create program that asks for name and says hello

```ruby
print 'What is your name? '
name = gets.chomp
puts "Hello #{name}"
```

Enter `ruby hello.rb` in the terminal



# Download Treehouse Workspace

Click `File`, `Download Workspace`

![bg right](treehouse-workspace.png)



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

## 1337 Hacker

Install xcode command line tools `xcode-select --install`

[Install multiple Ruby versions with rbenv](https://github.com/rbenv/rbenv)
