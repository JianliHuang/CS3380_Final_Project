# CS3380_Group-Project
CS 3380 Group Project- Online Book Order System


Please visit our Book Order System application at this url:http://jiacong.rf.gd/login.php


## World Book
---

<!-- TOC -->
- [World Book](#world-Book)
   - [Team Members](#team-members)
   - [Description of Application](#description-of-application)
   - [The Schema For the Database (The Table Definitions)](#the-schema-for-the-database-the-table-definitions)
   - [Explanation of Where the App is doing create, read, update, and delete](#explanation-of-where-the-app-is-doing-create-read-update-and-delete)
   - [Entity Relationship Diagram (ERD)](#entity-relationship-diagram-erd)





<!-- /TOC -->

---

### Team Members
---
- *Jianli Huang*
- *Jiacong Ma*




### Description of Application
---

> An easier way to figure out which kind of book you want to read next 

- This is a website for a Book Store. This website couold lets customers to view different category of book and allows store manger to add, delete and update books. In home page, viewer will be asked to login as manger or view as customer. 

- The customer version can see the list of book from 5 different categories of book with pictures and leave the comment about the book.
- The manager version can login to the website, add books, delete the books and update books information. Manager could also add a new catergory of book.  




### The Schema For the Database (The Table Definitions)
---

1. **Arts**
```sql
" CREATE TABLE WorldBook.Arts (
"  id int NOT NULL AUTO_INCREMENT  PRIMARY KEY,
"  Name varchar(35) NOT NULL,
"  Price int(11) DEFAULT NULL,
"  Stock int(35) DEFAULT NULL
"  );
```

2. **Biographies**
```sql
" CREATE TABLE WorldBook.Biographies (
"  id int NOT NULL AUTO_INCREMENT  PRIMARY KEY,
"  Name varchar(35) NOT NULL,
"  Price int(11) DEFAULT NULL,
"  Stock int(35) DEFAULT NULL
"  );
```

3. **Business**
```sql
" CREATE TABLE WorldBook.Business (
"  id int NOT NULL AUTO_INCREMENT  PRIMARY KEY,
"  Name varchar(35) NOT NULL,
"  Price int(11) DEFAULT NULL,
"  Stock int(35) DEFAULT NULL
"  );
```

4. **Comics**
```sql
" CREATE TABLE WorldBook.Comics (
"  id int NOT NULL AUTO_INCREMENT  PRIMARY KEY,
"  Name varchar(35) NOT NULL,
"  Price int(11) DEFAULT NULL,
"  Stock int(35) DEFAULT NULL
"  );
```

5. **Literature**
```sql
" CREATE TABLE WorldBook.Literature (
"  id int NOT NULL AUTO_INCREMENT  PRIMARY KEY,
"  Name varchar(35) NOT NULL,
"  Price int(11) DEFAULT NULL,
"  Stock int(35) DEFAULT NULL
"  );
```




### Explanation of Where the App is doing create, read, update, insert, delete and drop
---

- **Create** 
   1. Create new category of book, for example "History", "Teen".  
   -Create a new table by getting table name from input of user. 
   
   This step is creating a new table in our database. 
      
- **Read**
   1. Read `Name`, `Price`, `Author` , `Stock`  by manager from one table.
   2. Read `Name`, `Price`, `Author` , `Stock` by customer from one table.
   3. Display all books from 5 categories by manager. 
   4. Display all books from 5 categories by customer.
   -Select table and display it by getting table name from input of user.
   
   This step is using select sql to get result from database and display result
   
- **Insert**

  1.Add a new book of a category.
  -Create new book by getting input 'Name', 'Price', 'Author' and 'Stock' of user.
  
  This step is inserting new data into a table of database.
  
- **Update**
   1. Change price of a book in certain category. 
   - Change the price of a book in a table by getting input new price and book id from user.
   
   This step is updating 'Price' data for a specific dish id in table of database.
   
 - **Delete**
   1. Delete a book inside a catergory table.
   - Delete a book by getting input book 'Name' from user.
   
   This step is delete specific data in a table of database.

 - **Drop**
   1. Drop a category of book in manager version.
   - Drop a table by getting input of table name from user.
   
   This step is dropping a specific table of database.
### Entity Relationship Diagram (ERD)
