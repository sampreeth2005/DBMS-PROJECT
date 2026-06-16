# 📸 Instagram Data Repository

A Database Management System (DBMS) project that models the core functionalities of Instagram using a relational database approach. The project demonstrates database design principles, normalization techniques, SQL operations, triggers, and relationship modeling for a social media platform.

---

## 🎯 Project Overview

The Instagram Data Repository is a structured database system designed to manage and maintain user-generated content and interactions on a social media platform similar to Instagram.

The repository stores and manages:

* User profiles
* Posts
* Comments
* Likes
* Followers and Following relationships

The project focuses on efficient database design, normalization, data integrity, and query optimization.

---

## 🏆 Academic Project

**Course:** Database Management Systems (DBMS)

**Project Title:** Instagram Data Repository

**Team:** Group 2

### Team Members

* M. Sisira
* Bhogela Chetan Sai Sampreeth
* Praveen
* Gani
* Mani Kumar

---

## 📖 Problem Statement

Social media platforms generate massive amounts of user data every day.

The challenge is to:

* Store data efficiently
* Maintain data consistency
* Avoid redundancy
* Support fast data retrieval
* Ensure scalability

This project demonstrates how a relational database can effectively manage social media interactions.

---

## 🚀 Features

### 👤 User Management

* User registration
* User profiles
* Email and password management

### 🖼️ Post Management

* Create posts
* Store captions
* Store content URLs
* Track creation dates

### ❤️ Likes System

* Like posts
* Track engagement metrics
* Maintain relationship integrity

### 💬 Comment System

* Add comments
* Store comment history
* Associate comments with posts and users

### 👥 Follow System

* Follow users
* Manage follower-followee relationships
* Track social connections

---

## 🏗️ Database Entities

### User

Stores user account information.

Attributes:

* User_ID
* User_Name
* Email
* Password

### Post

Stores content posted by users.

Attributes:

* Post_ID
* User_ID
* Caption
* ContentURL
* Created_At

### Comments

Stores comments on posts.

Attributes:

* Comments_ID
* User_ID
* Post_ID
* Content
* Created_At

### Likes

Stores post likes.

Attributes:

* Likes_ID
* User_ID
* Post_ID

### Follows

Stores follower relationships.

Attributes:

* Follower_ID
* Followee_ID
* Created_At

---

## 🔗 Entity Relationships

### One-to-Many

* User → Posts
* Post → Comments
* Post → Likes

### Many-to-Many

* User ↔ User (Follow System)

---

## 📊 ER Diagram

The project includes an ER Diagram representing:

* Entities
* Attributes
* Relationships
* Cardinality Constraints

```text
User
 │
 ├── Creates ──► Post
 │                │
 │                ├── Receives ──► Comments
 │                │
 │                └── Receives ──► Likes
 │
 └── Follows ──► Other Users
```

---

## 🧩 Database Normalization

The database has been normalized up to Fifth Normal Form (5NF).

### First Normal Form (1NF)

* Atomic values
* Unique records
* No repeating groups

### Second Normal Form (2NF)

* No partial dependencies
* Full dependency on primary keys

### Third Normal Form (3NF)

* No transitive dependencies

### Boyce-Codd Normal Form (BCNF)

* Every determinant is a candidate key

### Fourth Normal Form (4NF)

* No multi-valued dependencies

### Fifth Normal Form (5NF)

* No join dependencies causing redundancy

---

## 🛠️ SQL Operations Implemented

### DDL Commands

#### CREATE

Create database tables.

#### ALTER

Modify table structures.

#### RENAME

Rename tables.

#### DROP

Delete tables.

---

### DML Commands

#### INSERT

Add records.

#### UPDATE

Modify existing records.

#### SELECT

Retrieve information.

#### DELETE

Remove records.

---

## ➕ Arithmetic Operators

Implemented examples using:

* Addition
* Subtraction
* Multiplication
* Division

---

## 🔍 Relational Operators

### Select & Project

Data retrieval and filtering.

### Set Difference

Compare data sets.

### Join Operations

Combine records from multiple tables.

---

## 📈 Aggregate Functions

Implemented:

* COUNT()
* SUM()
* AVG()
* MAX()
* MIN()

---

## 🔄 Set Operators

### UNION

Combines distinct records.

### UNION ALL

Combines records including duplicates.

### INTERSECT

Returns common records.

---

## 🤝 Join Operators

### INNER JOIN

Returns matching records.

### LEFT OUTER JOIN

Returns all records from the left table.

### RIGHT OUTER JOIN

Returns all records from the right table.

---

## 🧠 Nested Queries

Implemented:

### IN

Checks multiple values.

### NOT IN

Excludes specified values.

### ANY

Condition true for any value.

### ALL

Condition true for all values.

---

## ⚡ Database Triggers

### Direct Message Trigger

Automatically responds when a message event occurs.

### Comment Trigger

Performs actions when users comment on posts.

These triggers demonstrate database automation and event-driven operations.

---

## 📂 Project Structure

```text
Instagram-Data-Repository/
│
├── SQL Scripts/
│   ├── create_tables.sql
│   ├── insert_data.sql
│   ├── queries.sql
│   ├── joins.sql
│   └── triggers.sql
│
├── ER_Diagram/
│
├── PPT/
│
└── README.md
```

---

## 🎓 Learning Outcomes

This project helped us understand:

* Relational Database Design
* ER Modeling
* Normalization
* SQL Queries
* Joins and Nested Queries
* Database Triggers
* Data Integrity
* Social Media Database Architecture

---

## 🔮 Future Enhancements

* Stories Module
* Reels Management
* Messaging System
* Hashtag Tracking
* Analytics Dashboard
* Recommendation System
* Content Moderation Features

---

## 📸 Application Inspiration

Inspired by Instagram's real-world architecture for handling:

* User-generated content
* Social interactions
* Follower relationships
* Engagement tracking

---

## 📜 License

This project was developed for academic and educational purposes.

---

## 🙏 Acknowledgements

* Database Management Systems Course
* Faculty Mentors
* Team Members
* Open-source SQL Community

---

⭐ If you found this project useful, consider giving the repository a star.
