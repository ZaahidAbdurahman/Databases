# Databases

# DB Browser for SQL Lite

# Module 1: Introduction to SQL Databases 

![image](https://github.com/user-attachments/assets/62e498d0-37b8-4f7a-9c23-282c3fd6b7c5)

Figure 1: DB Browser for SQL Lite

- When dealing with SQL, you will want a tool to write statements and send them to a database for results. Numerous programs grasp SQL, often embedding statements in code. Instead of diving into complex setups, let's use 
  a hassle-free app available on Windows, Mac, and Linux — DB Browser for SQLite. 

![image](https://github.com/user-attachments/assets/65c9dcf5-359f-4ddf-b3a7-ae47b01fbc01)

Figure 2: SQL Lite

# What is a Database?

- Before diving into the language for chatting with databases, let's get what a database is.

- At its core, it is a stash of info. Picture this: a list of folks, where they reside, and their go-to color.

- Here, we have got three nuggets – a name, a city, and a hue. Now, in a database, these bits of info get sorted into columns, and each bunch of info lands in rows.

![image](https://github.com/user-attachments/assets/ddddf331-31b5-4e28-b1bd-1f8b345c0483)

Figure 5: Database Explanation

- The blueprint for all this – how fields, tables, and links are set – that is the schema. Now, we will not get into making these setups in this course.

![image](https://github.com/user-attachments/assets/0d570f78-f87b-462a-8a13-5cfb4e48a07e)

Figure 6: Card Representing an Individual

# What is SQL?

- SQL, short for Structured Query Language, is a tool for handling and defining data in databases.

- It came into play in 1974 and became a standard in 1986.

- It offers a standardized way to interact with databases, asking specific questions or making structured queries that databases can understand.

![image](https://github.com/user-attachments/assets/9d0d7439-5e9e-4481-99f1-75a78123904d)

Figure 8: Pronunciation of SQL

- SQL simplifies this process, letting us pose questions that databases grasp.

- No genius is required. SQL's become a powerhouse in data thinking, integrated into many database products, each with its quirks. 

  ![image](https://github.com/user-attachments/assets/bfe6621d-3de2-4240-a97c-a88a38326cf0)

   Figure 9: SQL Statements

-  A statement, the heart of SQL, is what you write to get info or tweak a database. It is made up of clauses, the building blocks.

-  Statements can do a lot: ask questions, modify data, or even create, tweak, or nix tables.

-  When it is tweaking existing tables, that is SQL as a DML (data manipulation language), working the CRUD operations (create, read, update, delete).

-  CRUD is your go-to term for database data gymnastics. 

[image](https://github.com/user-attachments/assets/287a7801-a2dd-4b03-9b4e-1332ceb05c46)
  
Figure 11: SQL Statements - Field and Table names

# Requesting Data From a Database

# SELECT Statement

![image](https://github.com/user-attachments/assets/7846a240-666a-4984-a91a-c4064732b906)

Figure 13: SELECT Statement

- The fundamental way to fetch information in SQL is by using a select statement.

- Just kick it off with the select keyword, indicating that we want the database to pick out specific information and hand it back to us.

- You can even ask for non-database text by tossing in some quotes and a semicolon.

![image](https://github.com/user-attachments/assets/6926fce4-21a7-4333-98cb-dbe76fc9ef8d)

- To understand the database content, you can click on "browse data" and choose a specific table, like 'people'.

- Each field in the table can be used to request information.

- So, to retrieve all the first names from the 'people' table, it is as simple as writing "SELECT first_name FROM people;".

![image](https://github.com/user-attachments/assets/08f190cb-1205-4519-a82e-982056beb518)

Figure 15: Execute SQL

![image](https://github.com/user-attachments/assets/3d0126f1-a965-4e6f-9e97-5f58220ab4dc)

Figure 16: The Art Of Refining Our Queries

#  WHERE Statement

- When we are craving specific info from the database, the WHERE keyword becomes our trusty sidekick.

- It helps us set conditions within a SELECT statement. Let's say you want records only for Californians; toss in a WHERE clause with the condition 'state_code=CA'.

- Beware of case sensitivity, though. 'CA' and 'ca' are different in the database. So, make sure your caps match.

  ![image](https://github.com/user-attachments/assets/92b80b2c-b4c6-491f-99fc-dcdf8aa6de21)

   Figure 18: Results of WHERE Statement

- You can spice it up by exploring different fields. For instance, to find folks who opted for a shirt instead of a hat, switch your WHERE condition to 'shirt_or_hat=shirt'.

- Remember, the order of your clauses matters. If you jumble them, the database gets confused. Keep practicing and use white space wisely.

![image](https://github.com/user-attachments/assets/f59c2cd7-91c8-4be3-91ab-d67f8952b890)

Figure 19: Order of Clauses

# Statement Criteria

![image](https://github.com/user-attachments/assets/21d99958-22e2-4ab8-a90f-da800ff05f50)

Figure 20: Statement Criteria

- Let's add a dash of logic to our queries! The AND logical operator becomes our buddy.

- Want the names of Californians who wanted a shirt? Easy-peasy: "SELECT first_name, last_name FROM people WHERE state_code=CA AND shirt_or_hat=shirt.

- " You can string multiple conditions with AND or even use OR to get results that meet one of two conditions.

- Just remember those parentheses; they are your guiding light in complex queries.

# Statement Responses

![image](https://github.com/user-attachments/assets/4c5f58e6-23ff-4b16-8ff5-b7502b19ae9e)

- Sometimes, we do not want an exact match; we want to be a bit fuzzy. Enter the LIKE operator.

- It allows us to look for values that match part of a field. Need all states starting with 'C'? Instead of a long OR statement, try 'state_code LIKE 'C%''.

# Organizing with ORDER BY

- When the database serves up data, it might be all over the place. Here is where ORDER BY comes to the rescue. Stick it at the end of your query and pick a field for sorting. 

![image](https://github.com/user-attachments/assets/3e6ff759-40bb-4f76-bf65-9a71e61e70c4)

Figure 26: ASC or DESC

# Finding More Data

![image](https://github.com/user-attachments/assets/e11c7162-2149-4ae1-880d-9e11362b37fa)

Figure 28: DISTINCT Function

![image](https://github.com/user-attachments/assets/d4ea16f3-6a29-4ab6-b9ab-edc13221ca51)

Figure 29: Explore The Power Of SQL

# Data Types and Arithmetic Operators

# SQL Data Types

- Alright, let's dive into SQL data types. Now, in a database, fields are like containers holding specific kinds of data.

- You've got names, dates, ID numbers, or even the points scored in a competition. Now, databases like us to declare upfront what kind of data each field will hold when we create a table.

- This is where data types come into play.

![image](https://github.com/user-attachments/assets/950f855e-9b30-4fc6-99fc-94541eba176c)

Figure 31: SQL Data Types

- SQL has a few categories to be aware of binary for ones and zeros, dates and times for temporal info, numbers for numeric values, and text for characters.

- Now, within each of these, there are specific types tailored for different purposes. Remember, not every type is supported in every SQL implementation, so always check your documentation.

# SQL Maths Operators

- Now, let's talk SQL math. We've got various operators to play with – addition, subtraction, multiplication, division, and even modulo.

- Stick to integers unless you want unexpected results. Logical comparison operators, like greater than, less than, and equal to, can help filter results. 

![image](https://github.com/user-attachments/assets/9110ed19-74b5-4670-a1e7-52ea4334cb24)

Figure 32: Math in SQL

Databases also provide nifty math functions – check your software's documentation for the full list. Let's do a quick demo. If you want to add 4 and 2. Run that query, and bam, 6! 

![image](https://github.com/user-attachments/assets/88ec33ec-a968-43ac-ac17-56a9eb02e2e5)

Figure 33: Division

![image](https://github.com/user-attachments/assets/165cf934-722a-4e05-ab01-3af1069b1b2c)

Figure 35: ORDER BY

Flip the comparison to find those with scores of 70 or less. Now, let's dig into aggregate functions. Want the max and min quiz scores? Easy. Want the total points earned? Use the sum function. 

![image](https://github.com/user-attachments/assets/480acbf2-07f4-42ed-9529-fa32d5d9ca9b)

Figure 36: GROUP BY

# Compound Select

# Transforming SQL Data

- Now, let's talk about transforming SQL data – because sometimes, you have to mold it to fit your needs. Ever want to change the case of a string? Well, there is LOWER for lowercase and UPPER for uppercase. 

![image](https://github.com/user-attachments/assets/2da4f94c-cf9e-4cec-b62c-55f373972114)

Figure 39: Lower and Upper Case

Now, for those times when you need data to wear a different hat, there is CAST. 

![image](https://github.com/user-attachments/assets/93f922a9-46a7-4820-8314-8fa86d57d532)

Figure 42: CAST

- It lets you interpret one data type as another – useful when you cannot tweak the database schema. Oh, and keep in mind, sorting can behave differently based on how you treat data types.

# Aliases

- Alright, let's wrap up with a quick chat about aliases. You know, the names of the fields we get back in our queries – sometimes, they could use a makeover. If you want to give them a friendlier name, throw in the AS keyword. 

![image](https://github.com/user-attachments/assets/2553b6a0-7ce5-4bf4-a5ba-01fa21edf159)

- Like, check this out: instead of having UPPER(last_name) as a column header, let's call it 'surname'. And for first_name, how about 'firstname' without the underscore?   

# Modify or Adding Data

# Adding Data to Tables

![image](https://github.com/user-attachments/assets/f759ff22-7810-4329-aca4-543b9b162c80)

Figure 45: Adding Data to Tables

Carol's last name has been forgotten. SQL does not like that, it has to have some data. 

![image](https://github.com/user-attachments/assets/892a653b-4637-4469-8f4c-ab53400109c1)

# Modifying Table Data

- Alright, let's get into the groove of modifying data. We use the update keyword for this. 

![image](https://github.com/user-attachments/assets/ccb833f0-1c51-45ed-b278-5876922dff5b)

Figure 50: Modifying Table Data

![image](https://github.com/user-attachments/assets/75af5347-e380-47cd-bb8e-865f9c1a9470)

Figure 52: Carlos Morrison 

# Removing Table Data

- Alright, time to clean house. The delete keyword is your go-to for kicking records out of a table.

- Like update, you gotta tell the database where to drop the bomb, and it is smart to throw in a condition to keep things targeted.

- You do not wanna wipe out the entire guest list accidentally.

![image](https://github.com/user-attachments/assets/efbd10e5-e341-486a-9c4a-9e527bde9c93)

Figure 55: Removing Table Data

![image](https://github.com/user-attachments/assets/6904bf5b-8825-401d-beac-9671351237a3)

Figure 56: Delete From People

# Module 2: Introduction to MongoDB

# Introduction to MongoDB

- A widely used document database, MongoDB, is recognized for its robustness and user-friendliness.

- The course aims to provide developers with essential MongoDB knowledge, including installation, database deployment setup, fundamentals like the document model, database structure, and MQL.

- What is MongoDB?

- In 2009, MongoDB gained popularity among web developers for its user-friendly approach, enabling them to work with data in a format consistent with their applications — documents. 

- Its native drivers seamlessly integrated data with code.

# Relational DB vs MongoDB

- In this course, we will explore MongoDB's workings and distinctions from traditional relational databases.

- At a broad level, databases organize data, and more intricate databases adhere to specific design and data
  modeling standards.

![image](https://github.com/user-attachments/assets/46ff0ba2-a4a4-45e1-a1e5-5540784cb07c)

Figure 2: Relational (SQL)

![image](https://github.com/user-attachments/assets/6b327912-0c6f-47f8-a02d-07ede9981297)

Figure 4: Structured Query Language

![image](https://github.com/user-attachments/assets/3aeab4b8-e314-40b5-a3b6-9267c8a16ae5)

Figure 5: Joining Related Data

![image](https://github.com/user-attachments/assets/aecbd356-a9fe-49ef-bf14-fa2d8d5d1bfd)

MongoDB's flexible document store is a key feature, where data is stored in documents rather than tables.

![image](https://github.com/user-attachments/assets/05d16bd0-8838-4868-b06f-9cec0bedbe95)

# Documents and Collections

Creating a document

- Documents in MongoDB are essentially field-value pairs stored in BSON, a JSON-like format.

- The process involves creating documents and saving them to a database.

- While demonstrating this in the course using MongoDB shell on a Mac, it's emphasized that the same commands are applicable in Codespaces. 

![image](https://github.com/user-attachments/assets/7ad12c4f-1f73-4e3f-94f1-7dfcad63d705)

Figure 9: MongoDB JSON file

- The process of inserting documents into the database is explained using the Mongo shell command. 

- JavaScript can be written in this shell, and the importance of connecting to the correct database is highlighted.

![image](https://github.com/user-attachments/assets/4065d315-8911-4c55-8172-ef39cf455c19)

Figure 10: Creating a document

![image](https://github.com/user-attachments/assets/c3fd5d02-4171-462b-b7e1-1e65ef74940b)

Figure 11: Formatting a document

# Querying Documents

- The find command in MongoDB, similar to a SELECT statement in SQL, is fundamental for querying recipe documents. 

- It requires a query document as its first parameter; an empty query document retrieves all documents by default.

![image](https://github.com/user-attachments/assets/d9393ef1-6329-4af2-be04-218c0614b7a1)

Figure 13: Using .find with parameters

- Numeric range searches, greater than or less than queries, and other advanced features will be explored in the next section.

# Storing Data in a Document

- MongoDB documents provide a versatile solution for storing diverse data in various formats, offering flexibility not commonly found in traditional relational databases.

- While traditional databases might rely on text or number fields, MongoDB enables us to handle more complex structures, such as a recipe, without the need for extensive refactoring.

![image](https://github.com/user-attachments/assets/33e06582-b384-4315-bd80-4103eef4b02f)

Figure 14: Entering Data into document

![image](https://github.com/user-attachments/assets/f7270e30-b211-40bd-bed0-7453a0b374fc)

Figure 15: Using insert 

Collections

-  The flexibility inherent in MongoDB's document model offers numerous advantages for developers, but maintaining organization becomes challenging over time.

-  Collections play a pivotal role in addressing this challenge.

![image](https://github.com/user-attachments/assets/f51b2de7-fb9e-4190-bfe1-6ff8b9dcb8cf)

Figure 18: Recipe - User - Blog Post

![image](https://github.com/user-attachments/assets/94bb02bd-7a05-407c-a533-020423334f7e)

Figure 19: Collections and Databases

- In our queries, we have been using collections consistently, like in db.recipes.find to retrieve documents.
  
- Essential commands include show dbs to display all databases and show collections to list collections within the current database. 

- You can identify the current database using db.getName. Both databases and collections are created dynamically as you insert data.

![image](https://github.com/user-attachments/assets/66437892-702e-4b4f-81e8-dc65e608c12c)

Figure 20: Collections

![image](https://github.com/user-attachments/assets/6e2d1b61-7ad2-4973-b6e4-bff181d9620a)

Figure 22: Validating Collections

This comprehensive understanding of MongoDB collections sets the stage for more advanced topics later in the course. The upcoming challenge will allow us to apply our knowledge effectively.




 
