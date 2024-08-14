# Databases

# DB Browser for SQL Lite

# Module 1: Introduction to SQL Databases 

![image](https://github.com/user-attachments/assets/62e498d0-37b8-4f7a-9c23-282c3fd6b7c5)
Figure 1: DB Browser for SQL Lite

- When dealing with SQL, you will want a tool to write statements and send them to a database for results. Numerous programs grasp SQL, often embedding statements in code. Instead of diving into complex setups, let's use a   
  hassle-free app available on Windows, Mac, and Linux — DB Browser for SQLite. 

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

  ![image](https://github.com/user-attachments/assets/287a7801-a2dd-4b03-9b4e-1332ceb05c46)
  Figure 11: SQL Statements - Field and Table names

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










