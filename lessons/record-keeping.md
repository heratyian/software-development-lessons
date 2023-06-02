# Record Keeping
This lesson reviews the history of record keeping and takes a first look at database design.

<!-- TODO: make separate slides -->
## [Slides](../slides/overview/index)

## Topics
- domain modeling
- database design

## History of Record Keeping
- Out of all the stuff we have to learn: where to begin?
- The foundation of the world was the written word
- The foundation of the world today is software
- What were they writing?
- Who is the first person whose name we know?
<!-- [Kushim](https://en.wikipedia.org/wiki/Kushim_(Uruk_period)) -->
- "29,086 measures barley; 37 months — Kushim"

>
> It is telling that the first recorded name in history belongs to an accountant, rather than a prophet, a poet, or a great conqueror.
>
> Yuval Noah Harari, Sapiens: A Brief History of Humankind

- What were they printing?

- What was the best-selling book? (after the Bible?)

- In the 17th century, English almanacs were bestsellers, second only to the Bible

- An almanac is an annual publication that includes information such as:
   - weather forecasts
   - farmers' planting dates
   - tide tables
   - tabular information often arranged according to the calendar.

- The killer application of writing, and printing, was recordkeeping

## The killer application of computing is also recordkeeping
- The heart of any application is the information it is keeping track of.
- Users, tweets, and who-follows-who in Twitter.
- Listings, bookings, and messages in Airbnb.
- Venues, reviews, and ratings in Yelp.

## IN THE BEGINNING, THERE WAS CRAIGSLIST
A categorized list of records

- We keep track of this information as records in plain old tables — just like they did in almanacs in the 17th century.
- One of the most important parts of application development is figuring out what information we need to keep track of, and a good set of tables to organize that information.
- This is part of the process known as data modeling (or "database design" or "database architecture").
- This is usually not taught in intro courses! But, it's the most important and most challenging part of app development.
- It's an art, not a science. We'll spend time every week practicing. Let's dive in!

## Databases
- A "database" is the software we use to store information. It is just a set of 2D tables; don't let the fancy name throw you. It's like a clipboard; or, an Excel workbook, where each table is one sheet.
- However, I don't want you to think about databases as software at all. Try to think of them as just paper, like almanacs.
- Whatever information we need to power our applications, we need to be able to figure out a way to store it in 2D tables, as if we were storing them in paper tables.
- And whatever logic we need to solve our users' problems with that information, we have to be able to describe how we'd do it as humans, given paper tables.
- Computers are just faster at doing it than us, but it will be the same operations — looking up data that's relevant to a certian user, ordering things in certain way, filtering things by certain criteria, etc.

## One approach to database design
* We (the developers) figure out the main things, or nouns, in our problem space and make a table for each.
* We add columns to each table for each attribute of the thing we need to keep track of.
* Our users create (or read, or update, or delete) rows.
* We say "create, read, update, or delete" so often — these are the fundamental 4 operations that all user actions map to — **CRUD**.
* 80%+ of the functionality of most SaaS applications is **CRUD**. This is what we will focus on learning how to build.

## Caveat #1
* Our users actions should *not* trigger creating tables or columns; only rows. We, the developers, will create all tables and columns up front, when we design and deploy the application.
* Users can **CRUD** a million rows per second if they want to. They just can't add tables or columns.

## Caveat #2

* **We only store one value per cell.**
* A value can be a long blob of text, like a bio; but it can't be *multiple* bios for different people.

## Must See Movies

* Okay, this is all pretty abstract. Let's look at some examples.
* Lets examine an [application](https://msm-associations-target.herokuapp.com/) that we'll build in class. It's a very simplified version of the IMDb (the Internet Movie Database).
* Click around it for a minute. Observe and identify:
* How are the URLs named? What is indicated by each part of the URL?
* What all information is being stored and displayed on each page?
* If you had to design tables to store all of the information required to power that app, what would they be? What columns would they have? Think of questions.
* Let's experiment on the whiteboard.


## Movies Table

### movies with director info
|id|title|desc|director_name|director_bio|director_dob|
|-|-|-|-|-|-|
|22|Shawshank|...(long)|Darabont|...(long)|28-Jan-1959|
|23|Godfather|...(long)|Coppola|...(long)|07-Apr-1939|
|26|Godfather II|...(long)|Coppola|...(long)|07-Apr-1939|
|28|Dark Knight|...(long)|Nolan|...(long)|30-Jul-1970|

### movies with director AND actors
|id|title|desc|director_name|director_bio|director_dob|actors|
|-|-|-|-|-|-|-|
|22|Shawshank|...(long)|Darabont|...(long)|28-Jan-1959|Freeman, Robbins|
|23|Godfather|...(long)|Coppola|...(long)|07-Apr-1939|Pacino, Keaton|
|26|Godfather II|...(long)|Coppola|...(long)|07-Apr-1939|Pacino|
|28|Dark Knight|...(long)|Nolan|...(long)|30-Jul-1970|Freeman|

### movies with director AND actors AND actor bios
|id|title|desc|director_name|director_bio|director_dob|actors|actor_bios?|
|-|-|-|-|-|-|-|-|
|22|Shawshank|...(long)|Darabont|...(long)|28-Jan-1959|Freeman, Robbins|😭|
|23|Godfather|...(long)|Coppola|...(long)|07-Apr-1939|Pacino, Keaton|😭|
|26|Godfather II|...(long)|Coppola|...(long)|07-Apr-1939|Pacino|😭|
|28|Dark Knight|...(long)|Nolan|...(long)|30-Jul-1970|Freeman|😭|

Not only does this break caveat #2 (We only store one value per cell), this breaks the **DRY** principle. Don't Repeat Yourself

### movies & directors tables
- We figure out the main things, or nouns, in our problem space and make a table for each.
- We can solve this by using a **foreign key**. Movies and Directors are separate *nouns* in this app.
- The *director_id* goes on the *movies* table because a movie belongs to a director. Our app allows only one director for the movie.

- 'id' - Every row in a table has a **Primary Key**
- '_id' - Some rows also have a **Foreign Key**, which refers to a row in another table

<u>movies</u>
|id|title|desc|director_id|
|-|-|-|-|
|22|Shawshank|...|12|
|23|Godfather|...|15|
|26|Godfather II|...|15|
|28|Dark Knight|...|18|

<u>directors</u>
|id|name|bio|dob|
|-|-|-|-|
|12|Darabont|...|...|
|15|Coppola|...|...|
|18|Nolan|...|...|
|20|Gerwig|...|...|

### movies & actors tables
- How about connecting movies to actors?
- Where do we put the foreign key?
- Does a movie have many (or one) actors?
- Does an actor have many (or one) movies?
- Remember caveat #2 (We only store one value per cell)

<u>movies</u>
|id|title|desc|
|-|-|-|
|22|Shawshank|...|
|23|Godfather|...|
|26|Godfather II|...|
|28|Dark Knight|...|

<u>actors</u>
|id|name|bio|
|-|-|-|
|87|Freeman|...|
|88|Pacino|...|
|89|Robbins|...|
|91|Keaton|...|


### characters table
- We solve this with a *join* table called 'characters' that connects movies to actors
- This is called a **many-to-many** relationship because a movie has many actors and and actor has many movies.

<u>movies</u>
|id|title|desc|
|-|-|-|
|22|Shawshank|...|
|23|Godfather|...|
|26|Godfather II|...|
|28|Dark Knight|...|

<u>characters</u>
|id|movie_id|actor_id|name
|-|-|-|-|
|48|22|87|Red|
|49|22|89|Andy|
|53|23|88|Michael|
|57|23|91|Kay|
|59|26|88|Michael|

<u>actors</u>
|id|name|bio|
|-|-|-|
|87|Freeman|...|
|88|Pacino|...|
|89|Robbins|...|
|91|Keaton|...|

## Next Up

[Records & Relationships](./records-and-relationships)
