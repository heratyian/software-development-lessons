# Ruby on Rails Phase 1

## [101: RPS RCAV](https://github.com/appdev-projects/rps-rcav)
[video](https://share.descript.com/view/QzA5UP0kaE1)
[slides](https://slides.com/raghubetina/06-routing-rcav?token=43w7FD8Q)
[reading](https://chapters.firstdraft.com/chapters/779)
[diagram](https://chapters.firstdraft.com/chapters/882)

## [102: Fortune Teller](https://github.com/appdev-projects/fortune-teller)

## [103: Omnicalc 1](https://github.com/appdev-projects/omnicalc-1)
[video](https://share.descript.com/view/pyUjjNG6uPx)

## [104: Omnicalc Debug (more form practice)](https://github.com/appdev-projects/omnicalc-debug)

Need API Keys in ENV
```
DARK_SKY_KEY=''
GEOCODING_API_KEY=''
```

## [107: Refactoring Fortune Teller with Dynamic Routes](https://github.com/appdev-projects/refactoring-fortune-teller)

[notes](https://chapters.firstdraft.com/chapters/841)


## [108: Dashboards](https://github.com/appdev-projects/dashboards)
[video](https://dpi.instructure.com/courses/176/pages/video-dashboards-dynamic-route-segments)


## [109: MSM Queries](https://github.com/appdev-projects/msm-queries)
[video](https://dpi.instructure.com/courses/176/pages/video-msm-queries-intro-to-databases)

## [110: Classroom Queries Debug](https://github.com/appdev-projects/classroom-queries-debug)
Here is some more practice on building a web interface to our database using ActiveRecord.

## [111: Refactoring MSM Queries](https://github.com/appdev-projects/refactoring-msm-queries-1)

We're going to refactor MSM Queries with a powerful technique for taking advantage of one-to-many and many-to-many associations between tables.

First, load this project and read through the code, starting as usual with config/routes.rb. The starter code for this project is the solution to the first MSM Queries project. How does my solution compare to yours? Where does it differ?

Then, following along with this [Video: Refactoring MSM Queries 1](https://uchicago.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=64250a40-f6c3-417f-8f43-af3100cc532e&start=0). In it, I demonstrate how to refactor the project. Just watch while I do the first part, and if you have any questions pause the video and ask us.

Then you'll have a chance to do more yourself. Open up and read through this Chapter for a detailed written explanation: [Refactoring MSM Queries with Methods](https://chapters.firstdraft.com/chapters/843).

## [115: Different Ruby Styles](https://chapters.firstdraft.com/chapters/787)

## [120: MSM Validations](https://github.com/appdev-projects/msm-validations)

[reading](https://chapters.firstdraft.com/chapters/845)


## [125: Photogram GUI](https://github.com/appdev-projects/photogram-gui)
[video](https://dpi.instructure.com/courses/176/pages/video-photogram-gui)

## [130: Very Best Debug](https://github.com/appdev-projects/very-best-debug)
Practice building a web CRUD interface by debugging. 

## 135: Build a resource from scratch

**CRUD resources** are the foundational building blocks of web applications — a database table, along with routes/actions/views/forms/links that allow users to see and manipulate entries in that table. Being a web developer means identifying, building, and assembling these resources in useful ways all day, every day.

Now that you've seen a few examples of how to wire a complete CRUD resource (in Photogram GUI and Very Best Debug), try building some on your own, from scratch.

Imagine that we're building a simple, *anonymous* neighborhood bulletin board:

- There should be a page with a form to create posts.
- Each post should have a title and some content.
- If either the title or the content is left blank, the [post should not save](https://chapters.firstdraft.com/chapters/845).
- There should be a page with a list of the titles of all of the posts (ordered by most recently created first).
- People should be able to click on a "Show details" link next to each title to view a details page for the post.
- The details page of a post should display the post's title, content, and a comments section.
- There should be a link to click to delete a post (anyone can delete any post).
- The comments should be ordered by most recently created first.
- There should be a form at the bottom of the comments section to add a new comment.
- There should be a link to click to delete a comment (anyone can delete any comment).
- There should be a link that goes to a page that has a form to edit the post.
- After a person edits a post, the person should end up back on its details page.

(If you want to, feel free to come up with your own, different data model / user stories. But keep it simple — 2-4 tables and a simple CRUD UI, without sign-in/sign-out.)

### Suggested steps:

On paper or a whiteboard, draw a rough wireframe of the app you plan to build. Things to think about:
- What pages or screens will there be?
- What information will be displayed on each screen? What table(s) will it come from?
- What links and forms will each screen contain?
- When each link/form is clicked/submitted, what screen will the user end up at? Will there be any records in the database Created, Destroyed, or Updated along the way?
[Start a new Rails app from scratch](https://chapters.firstdraft.com/chapters/851).
[Generate the database tables](https://chapters.firstdraft.com/chapters/770#the-quick-way-to-create-a-table) that you think you'll need.
- Populate your tables with some rows using the interface located at /rails/db or from the Rails console.
- Decide on URLs for the screens you identified above.
- Pick a screen to start with and connect the R→C→A→V dots. Make it say "hello". Then make it do what it's actually supposed to do.
- Rinse and repeat until you've built all the screens.
Ask lots of questions along the way!

## [140: Reading — draft:resource generator](https://chapters.firstdraft.com/chapters/773)

## [145: Cookies Intro](https://github.com/appdev-projects/cookies-intro)
[notes](https://chapters.firstdraft.com/chapters/842)
[video](https://dpi.instructure.com/courses/176/pages/video-cookies-intro)

If you'd like to get the Google Translate portion working (optional), then you'll have to create the following [environment variables](https://chapters.firstdraft.com/chapters/792) (don't forget to restart your workspace after doing so):

 
```.env
TWILIO_ACCOUNT_SID: 
TWILIO_AUTH_TOKEN: 
TWILIO_SENDING_PHONE_NUMBER: 
MAILGUN_API_KEY: 
TRANSLATE_PROJECT:
TRANSLATE_CREDENTIALS:
```

## [150: Photogram Signin](https://github.com/appdev-projects/photogram-signin)
[video](https://dpi.instructure.com/courses/176/pages/video-photogram-signin-intro-to-authentication)

In the video, you’ll see me using a hash called session instead of a hash called cookies to store and fetch the signed in user’s ID. We use session exactly the same way as cookies, but it’s more secure. [read more](https://chapters.firstdraft.com/chapters/850#session)

## [155: MSM Signin](https://github.com/appdev-projects/msm-signin)
[video](https://uchicago.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=0325615f-63d3-473f-be6b-ae4b00eaec85)

## [160: Todo List 1 (Phase 1 practice exam)](https://github.com/appdev-projects/todo-list-1)

This is the practice exam. It is intended to help you identify areas to review before the real one.

Attempt to complete it under circumstances similar to the real exam: you can (and should) use your notes, previous work, the videos, Chapters, Google, and other resources; but not a live human being.

If you're well and truly stuck, then get help (from an instructor, ideally). Once you've completed this project, filled in gaps in your notes, and feel ready for the real exam, ask an instructor to unlock it for you.

## [165: Delivery Tracker 1 (Phase 1 exam)](https://github.com/appdev-projects/delivery-tracker-1)

This is the exam.

- You may use all your notes, the videos, the readings, etc. 
- You may not get help from anyone else in real-time. Doing so is a violation of the [honor code](https://cs.illinois.edu/academics/honor-code).
- You have 24 hours to complete the project.
- It is designed to be completed in less than 3 hours if you're confident in the material, so don't plan to take all 24 hours. The 24 hours is there to accommodate for any interruptions that might come up.
