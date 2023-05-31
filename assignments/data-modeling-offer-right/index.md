# Explore this target application: [Offer Right](https://offer-right.matchthetarget.com/).

## It's a simplified version of the real [Offer Up](https://offerup.com/) — a two-sided market. Users can:

- post items to sell
- browse items to purchase
- chat with sellers to make offers
- sellers can mark items as sold once satisfied
- buyers and sellers coordinate meeting up on their own
- Sign up for a new account or use our standard (alice/bob/carol@example.com with password of password). Explore and experiment with the features. I suggest taking notes on the following:

## Identify all of the screens in the app.
On each screen:
- What information can you see?
- What actions can you take? Usually, this means: "what links and buttons can you click?"
For each action:
- What screen do you end up on after you take it?
- What information was created/read/updated/deleted along the way?
Keeping the notes you took above in mind: design a data model that can support all user actions that you observe in app. I.e., a complete listing of tables and columns.

## Some old slide decks that might be handy to refer to:
- [Very Best](../very-best/index.html)
- [Yap](../yap/index.html)

It's usually very helpful to keep in mind database designs that you're already familiar with:

- [MSM tables.pdf](./msm-tables.pdf)
- [Yap tables.pdf](./yap-tables.pdf)

Remember that it's usually helpful to create your tables on paper or in a spreadsheet and entering some sample records to make sure you can record everything you're trying to record, before attempting to create the compact Entity Relationship Diagram (ERD).

Finally, draw an ERD of your schema design in [ideas.firstdraft.com](ideas.firstdraft.com). You can refer to the written documentation on how to use firstdraft.

Ask lots of questions!

## Requirements
Submit the firstdraft URL of your ERD. Everyone in your group should submit their own URL — we want you to get practice with the tool.

The ERD should be able to support every action a user can take in the target app.
Practice:
- Identifying the main entities of the problem.
- Identifying necessary attributes for each main entity.
- Identifying any one-to-many, many-to-many relationships.
- Naming any join tables.
- Designing tables in the standard ERD format.
