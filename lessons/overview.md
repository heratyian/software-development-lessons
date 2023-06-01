# Overview
This lesson provides an overview of the 12-week web development course.

## Topics
- Software as a Service (SaaS)

- [Slides](../slides/overview/index)

## Questions
- This course is question-driven.
- We need you to ask questions.
- Speak up whenever you feel like it, or raise your hand.
- If you're not sure whether it's relevant to everyone, wave over a TA and ask them; they'll decide and escalate.
- Outside of class, our rule: **You're only allowed to get stuck for 15 minutes before asking a question**.
- I'll be posted up in the class room, Slack, and Piazza.
- The course is organized according to the the 🔐 **lock-before-key** principle; until someone asks the question, I won't provide the info needed to solve an exercise.

## "app"
- There are three kinds of software:
  - **system software** (eg Windows and MacOS)
  - **utility software** (eg the system clock or clipboard)
  - **application software** — software that people ("users") use directly to achieve some specific goal. (eg a word processor or a social network)
- In this course, whenever you hear me say **app**, what I mean is **application software**.
- many people, when they say **app**, mean a native app
(something that you download from iOS App Store or Android Play Store and interact with through your phone's touch screen)
- We'll use the term more broadly, to mean **application software**, in this course.

## What does it mean to "know how to code"?
- Do you consider yourself someone who knows "how to code"?
- If someone has:
  - set up a landing page with Wix
  - a blog with Wordpress
  - or a store with Shopify
  - done data analysis with R or Stata
  - scraped websites with Python or Ruby
  - has written C++ or Java for a CS course
- ​does that mean they "know how to code"?
- There are so many different kinds of software — it's like saying you want to "learn science".
- I think when people say they want to learn "how to code," what they generally mean is that they want to be able to build the kind of software that they themselves use on a daily basis.
- Naturally, this is the kind of software that they are most familiar with.
- If they are the entrepreneurial type, if they have ideas, these are the kind of ideas they'll have and want to implement.

>
> **Knowing how to hack** also means that **when you have ideas, you'll be able to implement them**.... It's a big advantage, when you're considering an idea like putting a college facebook online, if instead of merely thinking 'That’s an interesting idea,' you can think instead '**That’s an interesting idea. I’ll try building an initial version tonight.**"
> 
> — Paul Graham, "How to Get Startup Ideas"

- What kind of software (excluding system and utility software) do you use most often?
  - R scripts for data analysis?
  - Python web scrapers?
  - Embedded C programs to run hardware devices?
- Possibly, but for most people probably not the above (at least not directly).
- How about Adobe Photoshop? Nintendo Switch games? Alexa Skills?
- Those are a bit closer to daily life.
- Which apps do you use most at work or school? When you're out with friends?


## [The kind of software applications that I use most frequently look like this](https://media.slid.es/videos/318017/DFU5XJsq/airbnb_2-1143.mp4)

>
> More and more major businesses and industries are being run on software and delivered as online services — from movies to agriculture to national defense.
> Many of the winners are Silicon Valley-style entrepreneurial technology companies that are invading and overturning established industry structures.
> Over the next 10 years, I expect many more industries to be disrupted by software, with new world-beating Silicon Valley companies doing the disruption in more cases than not."
>
> Marc Andreesen, "[Why Software Is Eating the World](https://a16z.com/2011/08/20/why-software-is-eating-the-world/)" (2011)
>

## Rather than "Why Software Is Eating The World"
- Why Internet-Delivered Software Is Eating The World
- Why "Cloud"-Based Software Is Eating The World
- Why Software-As-A-Service (SaaS) Is Eating The World

## We're going to learn how to build SaaS
- Not system software or utility software.
- Not 3D games.
- Not applications that are installed and run on a single device, without any communication to the outside world.
- We're building Software-as-a-Service (or "SaaS", or "cloud-based software") that delivers useful information to users over the internet, via URLs.
- At first, we'll focus on delivering that information through a web browser. Later, we can add other interfaces — iPhone, Android, Apple Watch, Alexa, etc.
- Not only are cloud-based apps a relatively straightforward class of software for beginners to cut their teeth on, it's a super-useful class of software — so much so that it's eaten the world!

## URL

Uniform Resource Locator

1. Type in a URL

(or the equivalents: click on a link, submit a form, tap on something, etc)

2. ???

3. Profit!

## About Me
- Hi! I'm Ian
- Back in 2012 I was living in Shenzhen, China teaching English
- I wanted to to learn "how to code".
- Specifically, I wanted to build an iOS app — but I didn't know anyone who knew how or what to learn to get there.
- Tried learning from books
  - c#
  - arduino
  - objective-c
- Massive Open Online Courses
  - Harvard CS50
  - Treehouse
  - Make School
- I moved back to Chicago in 2016 and got an internship building port/intermodal terminal solutions at Mi-Jack. Got on the job experience writing python, .NET C#, and LOTS of technical documentation.
- Hired by Nerdery to build iOS apps. Moved over to web development react js and .NET C# backend due to need and willingness to learn.
- Founded [https://biggreen.company](https://biggreen.company), [https://popping.live](https://popping.live), and [https://receipt-ai.com](https://receipt-ai.com) all with Ruby on Rails

## Computer Science

>
> That’s exactly the thing that will turn people away from programming forever,” he said. “It’s like teaching someone chemistry as the first thing if they want to learn how to paint."
>
> Raghu Betina, on teaching Computer Science to people who want to learn application development
>

## If not CS, then what should we start with if we want to learn how to write SaaS?

>
> On the back end, software programming tools and Internet-based services make it easy to launch new global software-powered start-ups in many industries — without the need to invest in new infrastructure and train new employees. In 2000, when my partner Ben Horowitz was CEO of the first cloud computing company, Loudcloud, the cost of a customer running a basic Internet application was approximately $150,000 a month. Running that same application today in Amazon’s cloud costs about $1,500 a month.
>
> Marc Andreesen, "Why Software Is Eating the World" (2011)

By the end of this course, you'll know how to do this for **$17/month**

- There were many things coming together in the 2000s to make SaaS companies ever cheaper to build and launch — datacenters for rent, the open-source movement, modern high-level languages and frameworks.
- It was not a coincidence that 2011 is also when coding bootcamps and online courses arose to fill the gap in developers that Computer Science departments were not addressing.
- Some of the same things that brought the cost of running a SaaS product down by two orders of magnitude are also why it became possible for beginners to build useful software from coding bootcamps and online courses.
- I heard about a few of these (Harvard CS50 / MakeSchool / Treehouse / Mobile Makers) and decided to give it a try while teaching in China.
- It worked! Finally, I learned "how to code" — I learned how to build the kind of software I had ideas for.

## *Not* learning these kinds of things
- How to implement lists, starting from scratch (i.e., working with the physical memory of the computer).
- How to sort those lists.
- How to actually draw to the pixels of the screen.
- These are solved problems. We can focus on our ideas instead.

## Learning *these* kinds of things
- Where to host our application, buy a domain name, etc.
- How to specify a list of URLs that people are allowed to visit.
- When someone visits a URL, how to retrieve the relevant resource that they trying to locate — usually from a database.
- How to make the information look nice with some formatting.
- This is what we'll learn, starting today.

## That's still a lot to learn in a few weeks...
- Did you know that the DNA of humans and chimpanzees is about 98% the same?
- Most of our DNA is the plumbing of being alive, being primates, etc.
- Only a tiny bit makes us distinct from chimpanzees.
- We have exactly the same 98% since we descended from a common ancestor, approximately 6-10 million years ago.
- Similarly, Twitter and Airbnb share 98% of their code.
- Most of any SaaS application are common plumbing: having a web server, connecting to the database, etc.
- Only a tiny bit makes them distinct from one another — tweets instead of listings, etc.
- Twitter and Airbnb, too, have exactly the same core code; since they too had a common ancestor.
- In 2003, a Chicago entrepreneur (Jason Fried) hired a Danish programmer (David Heinemeier Hansson) to build an idea he had for project management SaaS. They called it Basecamp.
- David loved an obscure programming language called Ruby, which was invented in Japan in the mid 1990's. Ruby was slow, but expressive and "beautiful" (to David). Jason didn't really care what David used so he said 👍
- Once he got Basecamp working, David extracted the 98% of it that was common plumbing for all SaaS and released it for free, open-source. He called this package of Ruby code that let you quickly get a web application up and running "Ruby on Rails." It was, at the time, revolutionary.
- So this is going to be our hack:
- Much like Twitter, Airbnb, NYTimes, GitHub, and thousands of other companies, we're going to borrow David's (and, by now, thousands of other contributors') code.
- This will let us skip re-inventing tens of thousands of lines of code and many years of learning.
- We just need to learn enough of the Ruby language to be able to navigate Ruby on Rails, the framework. ("Framework" just means "a bunch of code we're borrowing".)
- This will be our strategy. For example, we'll learn just enough of another language, CSS, to be able to use a CSS framework called Bootstrap to make our pages look professional.
- In general, we will stand on the shoulders of giants.

## Play the whole game
- The crucial piece in finally making programming "click" is learning all the skills needed to deploy an application, not just one or two. I.e., we become **full-stack developers**.
- Most courses or books teach you one language or skill, but then you're left wondering how that fits in with the 99 other things you need to know in order to deploy an application.
- Making a real, functional application is motivating! It gives you a reason to continue learning — to improve it, and to make the next one.

## Learning how to learn
- Our real goal during these 12 weeks is not to learn Ruby, Rails, Bootstrap, or any other particular language or framework.
- These are good, beginner-friendly, motivating choices for an introductory course.
- Our real goal is to learn how to learn, so that you can then go on to learn whatever interests you.
- Being a software developer means being a lifelong learner.
- There are always new languages, techniques, and frameworks to stay up-to-date on.
- Every single project involves learning new things, depending on what real-world problem you're being hired to solve.
- We are inventors. There are no formulas to look up and apply; we have to learn about the problem and then invent solutions.

## How the course will work
- Learning how to program from lectures is really hard.
- So many things to juggle — watching me, typing along, taking notes.
- Super easy to fall behind if you get stuck on something.
- Instead, we'll be using a partially "flipped" format. Instead of lectures, you'll have videos that you can pause, speed up, skip back, search, and reference whenever you want.
- During our class meetings, we'll do activities together to practice and reinforce what you learned from the videos and readings.
- M/W/F mornings — "class meetings". All the rest of the time (M/W/F afternoons, T/Th) is "lab" (with the exception of other seminars and guest lectures).
- There will be exceptions to this schedule, but that's the general plan.
- Friday morning we'll do activities together to reinforce and extend your learnings.
- During lab time, I will be posted up in the collab space next door.
- Please walk over and ask me (and the other instructors) lots of questions as you're working through the videos, readings, and projects.
- I may look like I'm busy on my laptop but I'm not. I'm there for one purpose only: waiting for you to come ask me questions.
- Canvas is our home base.
- All of your work will be under "Assignments".
- I recommend always clicking "Show by Type" (instead of the default "Show by Date").
- Most assignments are required. Optional ones will have "(Optional)" in their title.
- Try to complete all required assignments before the next class meeting, so that you are prepared for the activities we do together. Assignments will have due dates that you should try to hit.
* If you finish the required assignments:
    1. Try doing assignments over from scratch if you're not feeling confident. It should be easier the second time. Take notes on what's still confusing so we can discuss it during class.
    2. Try the optional assignments to extend your learning if you're feeling confident.
    3. Try applying the concepts you've learned to your own ideas. (Best possible way to learn.) I can bounce ideas with you.
    4. Some students have reported watching the videos over again at 2x speed is helpful.

## Next Up

[Record Keeping](./record-keeping)
