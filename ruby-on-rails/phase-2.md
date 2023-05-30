# Ruby on Rails Phase 2

## [201: Refactoring MSM Queries — 2](https://github.com/appdev-projects/refactoring-msm-queries-2)

In this project, we'll learn about the very powerful has_many and belongs_to shortcuts by refactoring MSM Queries again.

Follow along with this [recording](https://share.descript.com/view/XPeNADzGRwV). I start by reviewing a task from the Very Best Debug project, and then later I start in on Refactoring MSM 2.

## [[Optional] 205: Refactoring Photogram Associations](https://github.com/appdev-projects/photogram-associations)

This project is optional practice at re-writing association accessor methods with ActiveRecord’s powerful has_many and belongs_to helpers.

You may not be able to re-write all of the associations that you find, depending on how complicated they are. See how many you can get.

## [210: Photogram Complete](https://github.com/appdev-projects/photogram-final)

Finally: to synthesize the many, many techniques you've learned so far, build a fully-functional permissioned social network, complete with image uploads. 

Detailed notes/instructions in this [chapter](https://chapters.firstdraft.com/chapters/837).

## [220: Scaffold - Getting Started](https://github.com/appdev-projects/ad2-getting-started)

Until now, we've been writing fully-functional but very verbose, beginner-friendly code.

Over the next few projects, we're going to refactor our code to be concise and industrial-grade — more along the lines of what professional Rails developers would write.

Following along with this [video](https://share.descript.com/view/i66WXoNgrab) to get started.

## 222: Rails Guide on Testing

Read Sections 1, 2, 4, 5, 6, and 7 of the [Rails Guide on Testing](https://guides.rubyonrails.org/testing.html). These are the kinds of tests that we write most frequently.

Then, begin on the next assignment, Helper Methods Pt 1. In that project, we have one fully functional web resource, movies. Create a test file, test/system/movie_test.rb, and take a stab at writing some System tests in it to lock down the current functionality of the application. For example, try adding a test that checks to make sure the URL /movieshas an <h1>element on it. Run your tests with:

rails test test/system/movie_test.rb

After you’ve spent 20-30 minutes on it, you’re allowed to look at the example specs in test/system/example_specs.rb. You can copy-paste some or all of them into your own test file.

As we refactor for the rest of the project, you should run the tests periodically to ensure you didn’t break anything.

## [224: Helper Methods, Pt 1](https://github.com/appdev-projects/helper-methods)

This is a continuation of the Scaffold: Getting Started project, but you should click the "Load assignment in a new window" button here to set up a separate workspace and pick up from this new starting point.

Follow along with the [video](https://share.descript.com/view/bY2qZcJtJHl).

## 226: Helper Methods, Pt 2

Follow along with the second walkthrough: [Video: Helper Methods, Pt 2](https://share.descript.com/view/XxjXgxaPFr6).

Use the same Gitpod workspace that you created in Helper Methods, Pt 1.

## [228: Helper Methods, Pt 3](https://github.com/appdev-projects/helper-methods-3)

We're going to tie up a few loose ends.

Set up a new workspace by clicking the "Load assignment in a new window" button below.

[Follow along with the recording.](https://share.descript.com/view/mQOqBmvJmSo)

There are helpful notes in the README — keep it open in a tab.

## 230: Learn Git Branching

We are going to start incorporating more Git into our workflows. A key aspect of Git is branching, or maintaining multiple versions of the codebase in parallel.

Play the first part, the Introduction Sequence, of [this interactive tutorial on Git branching](https://learngitbranching.js.org/).

Later, whenever you feel the need to learn more advanced Git, go through the other parts.


## 235: Git CLI

We’ve been using the handy visual interface to Git located at /git in our projects, but it’s time to start learning the command-line interface (CLI) to Git — the way most developers use it.

Reading: [Command-line Git Basics](https://chapters.firstdraft.com/chapters/859)
Reading: [Git Aliases](https://chapters.firstdraft.com/chapters/857)

## [240: Photogram Industrial](https://github.com/appdev-projects/photogram-industrial)

In this project, we'll rebuild Photogram (again). This time, it will be industrial grade™ — the kind of code you could charge money for. We'll use database indexes and constraints, advanced association accessors, scopes, validations, view helper methods like link_to and form_with everywhere, partials to DRY up code judiciously, the Devise gem for authentication and password reset emails, authorizing access to each action explicitly, and many other industrial-strength upgrades.

There are extensive notes in the README — keep it open in a tab.

There are five parts to the walkthrough video:

[Photogram Industrial, Pt 1](https://uchicago.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=2da4310d-36a0-41cd-8469-af5000f57bce) (Sorry about the poor audio quality in this part, the rest are better) - getting started.
[Photogram Industrial, Pt 2](https://uchicago.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=42da95e9-f663-41f2-92a2-ad0d0085e3ce#) - up through writing the sample data task
[Photogram Industrial, Pt 3](https://uchicago.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=5469d83c-9b11-43d3-9942-ad0d01525deb) - up through adding Bootstrap, etc, and setting up basic navigation
Please note that we're using Bootstrap v4 in the video. The official Bootstrap docs now show v5 by default, so when referring to the docs, you should [switch to v4.6 using the dropdown in the top-right](https://getbootstrap.com/docs/4.6/getting-started/introduction/). Or a good exercise would be to implement the same (or better) styling using v5 classes.
[Photogram Industrial, Pt 4](https://uchicago.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=59e372bb-4074-4916-b41a-ad0e00136924&start=0) - starting the user profile page
[Photogram Indsutrial, Pt 5](https://uchicago.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=5bb87c95-729d-4931-bee9-ad0e00000225) - adding a tabbed interface to the user profile page
Note that there are example solution model, migration, and sample data files located in the public/ folder. Don't peek at them until you try it yourself, and don't copy-paste — type it out yourself.

As always, make lots of commits as you work. Practice our new [command-line Git workflow](https://chapters.firstdraft.com/chapters/859). We added some Git aliases that make things a bit easier.

[Here is a target to work towards](https://pg-industrial-2-final.herokuapp.com/).

## 250: JavaScript — The Slimmest Guide

Let's (finally) get a taste of JavaScript.

[Open these detailed notes in a tab](https://chapters.firstdraft.com/chapters/893).

Since we're moving away from Gitpod, from now on I recommend [GitHub Codespaces](https://github.com/features/codespaces), or [installing locally](https://chapters.firstdraft.com/chapters/865).

## [260: Photogram Ajax](https://github.com/appdev-projects/pg-ajax-1)

It's time to Ajaxify our apps!

[Detailed notes here](https://chapters.firstdraft.com/chapters/863).

## [265: Rails UJS Practice](https://github.com/appdev-projects/ujs-practice-1)

Practice Ajax with Rails UJS. Notes in the README.
