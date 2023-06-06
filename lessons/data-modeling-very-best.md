# Data Modeling - Very Best
This lesson practices data modeling

## [Slides](../slides/data-modeling-very-best/index)

## Topics
- Data Modeling

## Domain Modeling
- What information does the application need to keep track of?

1. Where is that information coming from?
- users?
- government dataset?
- etc.
2. How would I keep track of that information on paper?
- Can I answer the "question" that each feature represents by looking through my tables?

### Computers can't do anything that we couldn't do by looking through paper tables

### Caveat #1
- We can't add tables or columns while recordkeeping. We (the developers) create all of the tables and columns up front.
- After we deploy the app, users only **create**, **read**, **update**, and **delete** (CRUD) rows in our tables.
- Users can CRUD a million rows per second if they want to. They can't add any tables or columns.

### Caveat #2
- We can only store one value per cell.
- A value can be a long blob of text, like a bio; but it can't be multiple bios for different people.
1. This will save a lot of trouble when it comes to retrieving the values later, and having to figure out where one value ends and the next one begins.
2. There are other important reasons to avoid multiple values in a single cell as well.

## Try to domain model: Very best
- Click around [Very Best](https://verybest.matchthetarget.com/), another app we might build during this course:
- You can sign in with any of the following (all of their passwords are password):
    - alice@example.com
    - bob@example.com
    - carol@example.com
    - eve@example.com

- Or you can sign up for your own new account (it doesnʼt need to be a real email address)
- It allows you to keep track of which restaurant in the city serves your favorite version of a particular dish. (eg Your favorite hot dog could be Portillo's)

1. Try to figure out what database tables back this app.
2. Write out all of the tables you think you'll need, with names and all columns (including foreign keys and join tables).
3. In order to test your database design, what questions can you ask?
4. Compare your designs against another group. Ask them the questions you came up with to test your design and provide helpful critiques.

## Next Up

[Interactive Ruby](./interactive-ruby)
