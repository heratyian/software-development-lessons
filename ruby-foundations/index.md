---
marp: true
title: Ruby Foundations
paginate: true
html: true
---

# Ruby Foundations

---
# Objects & Methods

In Ruby, all data are objects:
`​"hello"` `8.3` `[4, 8, 15]`

Every object is a member of some class.
`​String` `Float` `Array`

The class that an object belongs to determines what it can do
(i.e., what *methods* we can call on it)
`String#capitalize` `String#length` `Float#round` `Float#ceil` `Array#sort` `Array#length`

---
# Objects & Methods

We attach the method name to the object with a dot.
```
[4, 8, 15].length
=> 3
```

Every object has a method called `.class` which will tell you what it is
```
[4, 8, 15].class
=> Array
```

---
# Objects & Methods

Methods return a value, which is, like everything, an object; perhaps of the same class as the original object, perhaps not.

`[4, 8, 15].reverse # => another Array`

`[4, 8, 15].length # => an Integer`

The return value replaces the original expression in the program, and then the program continues.

`[4, 8, 15].length.odd? # => true`


---
# First Letters
The first letter of each word, or *token*, in a program is how Ruby determines what it is:

**lowercase letter**: local variable
(unless it's one of a handful of keywords like if, elsif, else, def, do, self, class, end; and a few others that we won't use)

**digit**: an Integer or Float

**"double" or 'single' quotes**: a String literal

**[square brackets]**: an Array literal

**{curly braces}**: a Hash literal

**:colon**: a Symbol

**CapitalLetter**: a class

---
# What Kind of Thing?
The most important things you should be asking yourself are:

**"What class is the object that I have?"**
**"What methods does it have?"**
**"Which method will get me one step closer to my goal?"**

It doesn't matter what class of object you wish you had. It only matters what you actually have. Your job is to invent a way to get from your starting point to your goal, using the tools at hand.

Sometimes Ruby or a third-party library will have a method that will get you 90% of the way. Most of the time, you'll have to do the work yourself using the fundamental building blocks of any program:

---
# Building Blocks

**Expressions**: `object.method(argument) # => returns a value`
**Variables**: to save the results of expressions `variable = object.method(argument)`
**Conditionals**: `if` statements
**Loops**

That's all we need for now. We can build anything with these.

<!-- There are other tools that will let us be more concise; but we first just want to make things work, as simply and as readably as possible. It's okay if the program is long, as long as it's clear. -->

---
# We Are Inventors
When you signed up to learn how to program, you signed up to become an *inventor*.

Software developers tackle unsolved problems.

There aren't predefined solutions to look up and apply.

Otherwise, we'd just buy something off the shelf and be software users.
<!-- Much cheaper, if a solution to your problem already exists -->

When faced with a task, your first instinct should be: **"How can I solve this puzzle with the tools I have?"**

---
# We Are Inventors

Your first instinct **shouldn't** be: "Let me Google for a solution to this problem." 

Developers do a lot of that, of course, but only after we've tried to solve it with what we already have.

**"Google Fu"** is a hugely important skill to practice in software development. But, the answers you find may not be suitable for beginners; they may even slow you down.

The tasks assigned in *Yet Another Ruby Introduction* are achievable using the classes, methods, and keywords introduced in the Ruby Chapters. Your job is to invent a combination of them that gets the job done.

For now, ask us questions — we are your Google.
