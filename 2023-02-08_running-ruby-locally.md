# Running Ruby On Your Own Machine


## Why?
Now that we've been using ruby in gitpod and treehouse it's time to start running ruby on your own machine.
1. more typical day to day developer experience
2. helpful for learning
3. fun to start hacking your own scripts


## Terminal
open terminal
* command + space (open spotlight search)
* search 'terminal', press `enter`

macOS is in the unix family so we have these useful commands
* `ls` - list directory contents
* `pwd` - print working directory
* `mkdir` - make directory
* `cd` - change directory
* `touch` - updates last open time of file
* `open` - open files and directories
* Use `man` to learn more about each command


## Ruby
Ruby comes preinstalled on macOS
* `ruby`
* `ruby --version` or `ruby -v` to check version
This is your system ruby. This version of ruby is included in macOS for compatibility with legacy software. 
 It's best to install different versions when developing rails applications. We'll get into this later.
* `gem list` to see all the libraries installed with this ruby


## Interactive Ruby (irb)
* type in `irb`
* play around with ruby
* type `exit` to exit irb shell


## Setup vscode
code editor
works great with ruby, rails, and pretty much any language

* [install vscode](https://code.visualstudio.com/)
* open vscode
* open 'command palette' (command + shift + p)
* add `code .` to your bash profile
  * this way we can open vscode from the terminal
  * `.` is shorthand for current directory


## Create Workspace Folder
* open terminal (command + space, search terminal)
* create workspace for all your different projects `mkdir Workspace`
  * be capitalize to be consistent with other folders in root
  * generally use lowercase and no spaces
* navigate to workspace `cd Workspace`
* create scratch folder `mkdir scratch`
* open scratch in vscode `code scratch`


## Create And Run Ruby File
* `touch hello.rb`
* open `hello.rb` in vscode
  * (command + p) to open search
  * type in filename `hello.rb`
* add code to ask for name and say hello

```ruby
print 'What is your name? '
name = gets.chomp
puts "Hello #{name}"
```

* in the terminal enter `ruby hello.rb`


## Create And Open HTML File
* `touch hello.html`
```html
<h1>hello world</h1>
```
* open in chrome


## Download Treehouse Workspace
https://piazza.com/class/ldj532ul5a0621/post/ldxaz2gw9ve7o7
* Click `File`, `Download Workspace`


## Resources

### vscode Extensions
[Ruby](https://marketplace.visualstudio.com/items?itemName=rebornix.Ruby)
[HTML CSS Support](https://marketplace.visualstudio.com/items?itemName=ecmel.vscode-html-css)
[GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)


### Ruby Docs
https://ruby-doc.org/
