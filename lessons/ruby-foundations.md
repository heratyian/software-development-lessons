# Ruby Foundations
This lesson discusses the basics of the ruby language

<!-- TODO: update slides -->
## [Slides](../slides/ruby-foundations/index)

## Topics
- Ruby

## Objects & Methods

- In Ruby, all data are objects:

```ruby
​"hello"

8.3

[4, 8, 15]
```

- Every object is a member of some class.
- Every object has a method called `.class` which will tell you what it is

```ruby
​"hello".class
=> String

8.3.class
=> Float

[4, 8, 15].class
=> Array
```

- The class that an object belongs to determines what it can do. (i.e., what *methods* we can call on it)
- We attach the method name to the object with a dot.

```ruby
# String#capitalize
"ian".capitalize
=> "Ian"

# String#length
"ian".length
=> 3

# Float#round
8.3.round
=> 8

# Float#ceil
8.3.ceil
=> 9

# Array#sort
[3, 2, 1].sort
=> [1, 2, 3]

# Array#length
[4, 8, 15].length
=> 3
```


- Methods return a value, which is, like everything, an object; perhaps of the same class as the original object, perhaps not.

```ruby
# returns another Array
[4, 8, 15].reverse
=> [15, 8, 4]

# returns an Integer
[4, 8, 15].length
=> 3
```

- The return value replaces the original expression in the program, and then the program continues.

```ruby
[4, 8, 15].length.odd?
=> true
```

## First Letters
- The first letter of each word, or *token*, in a program is how Ruby determines what it is:
- **lowercase letter**: local variable, unless it's one of a handful of keywords like:
    - if
    - elsif
    - else
    - def
    - do
    - self
    - class
    - end
    - and more!

- **digit**: an Integer or Float
- **"double" or 'single' quotes**: a String literal
- **[square brackets]**: an Array literal
- **{curly braces}**: a Hash literal
- **:colon**: a Symbol
- **CapitalLetter**: a class

## What Kind of Thing?
- The most important things you should be asking yourself are:
    1. **"What class is the object that I have?"**
    2. **"What methods does it have?"**
    3. **"Which method will get me one step closer to my goal?"**

- It doesn't matter what class of object you wish you had. It only matters what you actually have.
- Your job is to invent a way to get from your starting point to your goal, using the tools at hand.
- Sometimes Ruby or a third-party library will have a method that will get you 90% of the way.
- Most of the time, you'll have to do the work yourself using the fundamental building blocks of any program:

## Building Blocks
- **Expressions**: `object.method(argument) # => returns a value`
- **Variables**: to save the results of expressions `variable = object.method(argument)`
- **Conditionals**: `if` statements
- **Loops**

That's all we need for now. We can build anything with these.

<!-- There are other tools that will let us be more concise; but we first just want to make things work, as simply and as readably as possible. It's okay if the program is long, as long as it's clear. -->


## We Are Inventors
- When you signed up to learn how to program, you signed up to become an *inventor*.
- Software developers tackle unsolved problems.
- There aren't predefined solutions to look up and apply.
- Otherwise, we'd just buy something off the shelf and be software users.
<!-- Much cheaper, if a solution to your problem already exists -->
- When faced with a task, your first instinct should be:
>
> **"How can I solve this puzzle with the tools I have?"**
>

- Your first instinct **shouldn't** be: "Let me Google for a solution to this problem." 
- Developers do a lot of that, of course, but only after we've tried to solve it with what we already have.
- **"Google Fu"** is a hugely important skill to practice in software development. But, the answers you find may not be suitable for beginners; they may even slow you down.
- The tasks assigned in *Yet Another Ruby Introduction* are achievable using the classes, methods, and keywords introduced in the Ruby Chapters. Your job is to invent a combination of them that gets the job done.
- For now, ask us questions — we are your Google.

### Resources
- [The One Ruby Reference](https://chapters.firstdraft.com/chapters/774)
- [Try Ruby (optional)](https://try.ruby-lang.org/)
- [Official Ruby Documentation](https://ruby-doc.org/)
- [Ruby Programming In one video](https://youtu.be/8wZ2ZD--VTk)
