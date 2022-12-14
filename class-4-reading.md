# Class 4 reading

## What type of database is the best fit for the complex query intensive environment?

SQL queries are a goodfit. NoSql querys  do not have standard interfaces to perform such tasks.

## What type of database is the best fit for hierarchical data storage?

NoSQL is better for this type of storage, because it follows the "key-value pair" (much like a JSON file).

NoSQL is prefered for large data.

## Describe the differences in scalability between a SQl and NoSQL database as though you were speaking to a non-technical friend

SQL scalabililty is vertically scaled which means that they would stack on top of eacother... This may seem like a great idea however there is a cap as to how much you can stack on top. However with NoSQL you are able to add a whole other server side by side. so its like storing shoe boxes in your closet. you could stale them up... however you will only be able to get so many to fit. But with NoSql its like building another closet... or even A whole other house, and if that place fills up then you can build another and another. (no Cap... no i dont mean it like that).

## Among data tables, what is a one-to-many relationship and how do we “relate” them?

A one to many relationship is the joining of two tables. This is where we are able to connect lines from one table to another. We are able to state an employees info then one column states their department as a columns from there we can branch out and discuss their department as a table.

## Prior to designing your relational database, it might be useful to ___a___ of the database tables and their relationships

create a diagram.

## Explain the difference between a primary and foreign key

the primary key is dealing with our current table and its columns that obviously relate to the current table. while the foreign key is what matches our table to another table.

## How do we treat keywords and parameters differently in SQL syntax?


## Define normalization within the context of schemas and data

This helps us create/organize our DB and the structure as to not repeat which could muddy things up when there is alot of overlapping of data.

## Explain the difference between one-to-one, one-to-many, and many-to-many relationships to a non-technical recruiter

a one to one, is info that could link our two tables together, yet the "record in each table appears once..." [supportmicosoft](https://support.microsoft.com/en-us/office/video-create-one-to-one-relationships-a5868c76-50ea-44b7-892d-43f2af2802e0#:~:text=A%20one%2Dto%2Done%20relationship%20is%20a%20link%20between%20the,and%20the%20cars%20they%20drive.)

a one to many relatioship is where on piece of data on a table can be tied to one more more pieces of data on many other tables.

a many to many relatioship this connects one piece of data from one table to one OR MORE pieces of data to another table.

## overall notes

- SQL is known as Relational Databases(RDBMS). -  columns

- SQL are table DB's where NoSQL are Doc based. - key value pairs

- SQL predefined schema

## things i want to know more about

I have so many questions about all of this. I want to explore the `mysql workbench`