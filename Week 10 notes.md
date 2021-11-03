# CIT 114 Week 10
## Here are some important thinkgs I learned in Week 10
### Notes 08: Databases

#### What is a Database?

A database is a shared collection of related data used to support the activities of a particular organization. A database can be viewed as a repository of data that is defined once and then accessed by various users 

------

#### Database Properties

  * It is a representation of some aspect of the real world or a collection of data elements (facts) representing real-world information.
  * A database is logical, coherent and internally consistent.
  * A database is designed, built and populated with data for a specific purpose.
  * Each data item is stored in a field.
  * A combination of fields makes up a table. For example, each field in an employee table contains data about an individual employee.

------

#### Database Management System

A database management system (DBMS) is a collection of programs that enables users to create and maintain databases and control all access to them. The primary goal of a DBMS is to provide an environment that is both convenient and efficient for users to retrieve and store information.

With the database approach, we can have the traditional banking system. In this bank example, a DBMS is used by the Personnel Department, the Account Department and the Loan Department to access the shared corporate database.

Key Terms:
  * data elements: facts that represent real-world information
  * database: a shared collection of related data used to support the activities of a particular organization
  * database management system (DBMS): a collection of programs that enables users to create and maintain databases and control all access to them
  * table: a combination of fields

------

#### Characteristics and Benefits of a Database

Managing information means taking care of it so that it works for us and is useful for the tasks we perform. By using a DBMS, the information we collect and add to its database is no longer subject to accidental disorganization. It becomes more accessible and integrated with the rest of our work. Managing information using a database allows us to become strategic users of the data we have.

We often need to access and re-sort data for various uses. These may include:
  * Creating mailing lists
  * Writing management reports
  * Generating lists of selected news stories
  * Identifying various client needs

The processing power of a database allows it to manipulate the data it houses, so it can:
  * Sort
  * Match
  * Link
  * Aggregate
  * Skip fields
  * Calculate
  * Arrange

Because of the versatility of databases, we find them powering all sorts of projects. A database can be linked to:
  * A website that is capturing registered users
  * A client-tracking application for social service organizations
  * A medical record system for a health care facility
  * Your personal address book in your email client
  * A collection of word-processed documents
  * A system that issues airline reservations

There are a number of characteristics that distinguish the database approach from the file-based system or approach. This chapter describes the benefits (and features) of the database system.

#### Self-describing nature of a database system

A database system is referred to as self-describing because it not only contains the database itself, but also metadata which defines and describes the data and relationships between tables in the database. This information is used by the DBMS software or database users if needed. This separation of data and information about the data makes a database system totally different from the traditional file-based system in which the data definition is part of the application programs.

#### Insulation between program and data

In the file-based system, the structure of the data files is defined in the application programs so if a user wants to change the structure of a file, all the programs that access that file might need to be changed as well.
On the other hand, in the database approach, the data structure is stored in the system catalogue and not in the programs. Therefore, one change is all that is needed to change the structure of a file. This insulation between the programs and data is also called program-data independence.

#### Support for multiple views of data

A database supports multiple views of data.  A view is a subset of the database, which is defined and dedicated for particular users of the system. Multiple users in the system might have different views of the system. Each view might contain only the data of interest to a user or group of users.

#### Sharing of data and multiuser system

Current database systems are designed for multiple users. That is, they allow many users to access the same database at the same time. This access is achieved through features called concurrency control strategies. These strategies ensure that the data accessed are always correct and that data integrity is maintained. 
The design of modern multiuser database systems is a great improvement from those in the past which restricted usage to one person at a time.

#### Control of data redundancy

In the database approach, ideally, each data item is stored in only one place in the database. In some cases, data redundancy still exists to improve system performance, but such redundancy is controlled by application programming and kept to minimum by introducing as little redudancy as possible when designing the database.

#### Data sharing

The integration of all the data, for an organization, within a database system has many advantages. First, it allows for data sharing among employees and others who have access to the system. Second, it gives users the ability to generate more information from a given amount of data than would be possible without the integration.

#### Enforcement of integrity constraints

Database management systems must provide the ability to define and enforce certain constraints to ensure that users enter valid information and maintain data integrity. A database constraint is a restriction or rule that dictates what can be entered or edited in a table such as a postal code using a certain format or adding a valid city in the City field.
There are many types of database constraints. Data type, for example, determines the sort of data permitted in a field, for example numbers only. Data uniqueness such as the primary key ensures that no duplicates are entered. Constraints can be simple (field based) or complex (programming).

#### Restriction of unauthorized access

Not all users of a database system will have the same accessing privileges. For example, one user might have read-only access (i.e., the ability to read a file but not make changes), while another might have read and write privileges, which is the ability to both read and modify a file. For this reason, a database management system should provide a security subsystem to create and control different types of user accounts and restrict unauthorized access.

#### Data independence

Another advantage of a database management system is how it allows for data independence. In other words, the system data descriptions or data describing data (metadata) are separated from the application programs. This is possible because changes to the data structure are handled by the database management system and  are not embedded in the program itself.

#### Transaction processing

A database management system must include concurrency control subsystems. This feature ensures that data remains consistent and valid during transaction processing even if several users update the same information.

#### Provision for multiple views of data

By its very nature, a DBMS permits many users to have access to its database either individually or simultaneously. It is not important for users to be aware of how and where the data they access is stored

#### Backup and recovery facilities

Backup and recovery are methods that allow you to protect your data from loss.  The database system provides a separate process, from that of a network backup, for backing up and recovering data. If a hard drive fails and the database stored on the hard drive is not accessible, the only way to recover the database is from a backup.

If a computer system fails in the middle of a complex update process, the recovery subsystem is responsible for making sure that the database is restored to its original state. These are two more benefits of a database management system.

Key Terms
  * concurrency control strategies: features of a database that allow several users access to the same data item at the same time
  * data type: determines the sort of data permitted in a field, for example numbers only
  * data uniqueness: ensures that no duplicates are entered
  * database constraint: a restriction that determines what is allowed to be entered or edited in a table
  * metadata: defines and describes the data and relationships between tables in the database
  * read and write privileges: the ability to both read and modify a file
  * read-only access: the ability to read a file but not make changes
  * self-describing: a database system is referred to as self-describing because it not only contains the database itself, but also metadata which defines and describes the data and relationships between tables in the database
  * view: a subset of the database

------

#### Relational Databases

The relational data model was introduced by C. F. Codd in 1970. Currently, it is the most widely used data model.

The relational model has provided the basis for:
  * Research on the theory of data/relationship/constraint
  * Numerous database design methodologies
  * The standard database access language called structured query language (SQL)
  * Almost all modern commercial database management systems

The relational data model describes the world as “a collection of inter-related relations (or tables).”

------

Fundamental Concepts in the Relational Data Model

#### Relation

A relation, also known as a table or file, is a subset of the Cartesian product of a list of domains characterized by a name. And within a table, each row represents a group of related data values. A row, or record, is also known as a tuple. The columns in a table is a field and is also referred to as an attribute. You can also think of it this way: an attribute is used to define the record and a record contains a set of attributes.

The steps below outline the logic between a relation and its domains.
1.	Given n domains are denoted by D1, D2, … Dn
2.	And r is a relation defined on these domains
3.	Then r ⊆ D1×D2×…×Dn

#### Table

A database is composed of multiple tables and each table holds the data.

#### Column

A database stores pieces of information or facts in an organized way. Understanding how to use and get the most out of databases requires us to understand that method of organization.

The principal storage units are called columns or fields or attributes. These house the basic components of data into which your content can be broken down. When deciding which fields to create, you need to think generically about your information, for example, drawing out the common components of the information that you will store in the database and avoiding the specifics that distinguish one item from another.

#### Domain

A domain is the original sets of atomic values used to model data. By atomic value, we mean that each value in the domain is indivisible as far as the relational model is concerned. For example:
  * The domain of Marital Status has a set of possibilities: Married, Single, Divorced.
  * The domain of Shift has the set of all possible days: {Mon, Tue, Wed…}.
  * The domain of Salary is the set of all floating-point numbers greater than 0 and less than 200,000.
  * The domain of First Name is the set of character strings that represents names of people.

In summary, a domain is a set of acceptable values that a column is allowed to contain. This is based on various properties and the data type for the column. We will discuss data types in another chapter.

#### Records

Just as the content of any one document or item needs to be broken down into its constituent bits of data for storage in the fields, the link between them also needs to be available so that they can be reconstituted into their whole form. Records allow us to do this. Records contain fields that are related, such as a customer or an employee. As noted earlier, a tuple is another term used for record.

Records and fields form the basis of all databases. A simple table gives us the clearest picture of how records and fields work together in a database storage project.

#### Degree

The degree is the number of attributes in a table.

------

#### Properties of a Table

  * A table has a name that is distinct from all other tables in the database.
  * There are no duplicate rows; each row is distinct.
  * Entries in columns are atomic. The table does not contain repeating groups or multivalued attributes.
  * Entries from columns are from the same domain based on their data type including: 
  * number (numeric, integer, float, smallint,…)
  * character (string)
  * date
  * logical (true or false)
  * Operations combining different data types are disallowed.
  * Each attribute has a distinct name.
  * The sequence of columns is insignificant.
  * The sequence of rows is insignificant.

Key Terms
  * atomic value: each value in the domain is indivisible as far as the relational model is concerned
  * attribute: principle storage unit in a database
  * column: see attribute 
  * degree: number of attributes in a table
  * domain: the original sets of atomic values used to model data; a set of acceptable values that a column is allowed to contain
  * field: see attribute 
  * file: see relation 
  * record: contains fields that are related; see tuple 
  * relation: a subset of the Cartesian product of a list of domains characterized by a name; the technical term for table or file
  * row: see tuple 
  * structured query language (SQL): the standard database access language
  * table: see relation 
  * tuple: a technical term for row or record

Several of the terms used in this chapter are synonymous. In addition to the Key Terms above, please refer to Table below. The terms in the Alternative 1 column are most commonly used.

Terminology Key
|Formal Terms (Codd)|Alternative 1|Alternative 2|
|---|---|---|
|Relation|Table|File|
|Tuple|Row|Record|
|Attribute|Column|Field|

------

#### Non-relational Databases

In the year 1970’s when relational database came into picture, data schema to be worked upon were reasonably elemental and simple wherein the data items were to be arranged as a set of formally described tables with rows and columns. But with the need to store volumes and variety of data (unstructured) in recent years, non-relational database technologies have emerged to address the requirement that allow data to be grouped together more naturally and logically.

Examples of non-relational databases include:
  * Document-oriented
  * Graph based
  * Column based
  * Key-value
  * Hybrid

One of the most popular ways of storing data is a document-oriented database, basically employed for storing, managing and retrieval of semi-structured data where each record and its associated data is considered of as a “document”. A document-oriented database is also termed as a document store or simple document, is one of the kind of NoSQL database.

------

#### What is NoSQL?

NoSQL is an approach to databases that represents a shift away from traditional relational database management systems (RDBMS). To define NoSQL, it is helpful to start by describing SQL, which is a query language used by RDBMS. Relational databases rely on tables, columns, rows, or schemas to organize and retrieve data. In contrast, NoSQL databases do not rely on these structures and use more flexible data models. NoSQL can mean “not SQL” or “not only SQL.” As RDBMS have increasingly failed to meet the performance, scalability, and flexibility needs that next-generation, data-intensive applications require, NoSQL databases have been adopted by mainstream enterprises. NoSQL is particularly useful for storing unstructured data, which is growing far more rapidly than structured data and does not fit the relational schemas of RDBMS. Common types of unstructured data include: user and session data; chat, messaging, and log data; time series data such as IoT and device data; and large objects such as video and images.

#### TYPES OF NOSQL DATABASES

Several different varieties of NoSQL databases have been created to support specific needs and use cases. These fall into four main categories:
  * Key-value data stores: Key-value NoSQL databases (Links to an external site.) emphasize simplicity and are very useful in accelerating an application to support high-speed read and write processing of non-transactional data. Stored values can be any type of binary object (text, video, JSON document, etc.) and are accessed via a key. The application has complete control over what is stored in the value, making this the most flexible NoSQL model. Data is partitioned and replicated across a cluster to get scalability and availability. For this reason, key value stores often do not support transactions. However, they are highly effective at scaling applications that deal with high-velocity, non-transactional data.
  * Document stores: Document databases typically store self-describing JSON, XML, and BSON documents. They are similar to key-value stores, but in this case, a value is a single document that stores all data related to a specific key. Popular fields in the document can be indexed to provide fast retrieval without knowing the key. Each document can have the same or a different structure.
  * Wide-column stores: Wide-column NoSQL databases store data in tables with rows and columns similar to RDBMS, but names and formats of columns can vary from row to row across the table. Wide-column databases group columns of related data together. A query can retrieve related data in a single operation because only the columns associated with the query are retrieved. In an RDBMS, the data would be in different rows stored in different places on disk, requiring multiple disk operations for retrieval.
  * Graph stores: A graph database uses graph structures to store, map, and query relationships. They provide index-free adjacency, so that adjacent elements are linked together without using an index.

Multi-modal databases leverage some combination of the four types described above and therefore can support a wider range of applications.

#### BENEFITS OF NOSQL

NoSQL databases offer enterprises important advantages over traditional RDBMS, including:
  * Scalability: NoSQL databases use a horizontal scale-out methodology that makes it easy to add or reduce capacity quickly and non-disruptively with commodity hardware. This eliminates the tremendous cost and complexity of manual sharding that is necessary when attempting to scale RDBMS.
  * Performance: By simply adding commodity resources, enterprises can increase performance with NoSQL databases. This enables organizations to continue to deliver reliably fast user experiences with a predictable return on investment for adding resources—again, without the overhead associated with manual sharding.
  * High Availability: NoSQL databases are generally designed to ensure high availability and avoid the complexity that comes with a typical RDBMS architecture that relies on primary and secondary nodes. Some “distributed” NoSQL databases use a masterless architecture that automatically distributes data equally among multiple resources so that the application remains available for both read and write operations even when one node fails.
  * Global Availability: By automatically replicating data across multiple servers, data centers, or cloud resources, distributed NoSQL databases can minimize latency and ensure a consistent application experience wherever users are located. An added benefit is a significantly reduced database management burden from manual RDBMS configuration, freeing operations teams to focus on other business priorities.
  * Flexible Data Modeling: NoSQL offers the ability to implement flexible and fluid data models. Application developers can leverage the data types and query options that are the most natural fit to the specific application use case rather than those that fit the database schema. The result is a simpler interaction between the application and the database and faster, more agile development.

------

#### Query for Data

Depending on what type of database you are using, will depend on how you retrieve the data in the database. Retrieval of data from a database is called a query.

The most common language used in relational databases for queries is the Structured Query Language or SQL for short. SQL is a standard language for selecting, inserting, updating, and deleting data in a relational database. It can do more but the majority of the work in a system is done using SELECT, INSERT, UPDATE, and DELETE.

------

#### SQL Table Basics

In a SQL table, you generally have a table that contains columns of fields, also known as columns, with records that contain all the columns in a table. Records contain all the assigned columns for each table, but have different information.

Each column has a specific data type, examples of data type include:
  * Bit –Integer data with either a 1 or 0 value
  * Int –Integer (whole number) data from -2^31 (-2,147,483,648) through 2^31 – 1 (2,147,483,647)
  * Decimal –Fixed precision and scale numeric data from -10^38 -1 through 10^38
  * Timestamp –A database-wide unique number
  * Uniqueidentifier –A globally unique identifier (GUID)
  * Float –Floating precision number data from -1.79E + 308 through 1.79E + 308
  * Real –Floating precision number data from -3.40E + 38 through 3.40E + 38
  * Datetime –Date and time data from January 1, 1753, to December 31, 9999, with an accuracy of one-three-hundredths of a second, or 3.33 milliseconds
  * Char –Fixed-length non-Unicode character data with a maximum length of 8,000 characters
  * Varchar –Variable-length non-Unicode data with a maximum of 8,000 characters
  * Text –Variable-length non-Unicode data with a maximum length of 2^31 – 1 (2,147,483,647) characters

In addition to columns that contain data, you have columns that are used as keys. A key that is used to uniquely identify a record in the database are called primary keys. These keys are used to relate information between two or more tables with foreign keys used to relate against a primary key.

A foreign key is an identical copy of a primary key that is inserted into another table for the purposes of relating information between two tables. Unlike primary keys, you can have many copies of the same key in a table if it is a foreign key. Only the primary key has to be unique.

------

#### SQL Query Commands

The SQL data manipulation language (DML) is used to query and modify database data. In this chapter, we will describe how to use the SELECT, INSERT, UPDATE, and DELETE SQL DML command statements, defined below.
  * SELECT – to query data in the database
  * INSERT – to insert data into a table
  * UPDATE – to update data in a table
  * DELETE – to delete data from a table

In the SQL DML statement:
  * Each clause in a statement should begin on a new line.
  * The beginning of each clause should line up with the beginning of other clauses.
  * If a clause has several parts, they should appear on separate lines and be indented under the start of the clause to show the relationship.
  * Upper case letters are used to represent reserved words.
  * Lower case letters are used to represent user-defined words.

------

#### SELECT statement with WHERE criteria

Sometimes you might want to focus on a portion of the Publishers table, such as only publishers that are in Vancouver. In this situation, you would use the SELECT statement with the WHERE criterion, i.e., WHERE city = ‘Vancouver’.

#### Using wildcards in the LIKE clause

The LIKE keyword selects rows containing fields that match specified portions of character strings. LIKE is used with char, varchar, text, datetime and smalldatetime data. A wildcard allows the user to match fields that contain certain letters. For example, the wildcard province = ‘N%’ would give all provinces that start with the letter ‘N’.

Table four ways to specify wildcards in the SELECT statement in regular express format.

|Symbol|Usage|
|---|---|
|%|Any string of zero or more characters|
|_|Any single character|
|[ ]|Any single character within the specified range (e.g., [a-f]) or set (e.g., [abcdef])|
|[^]|Any single character not within the specified range (e.g., [^a – f]) or set (e.g., [^abcdef])|

#### SELECT statement with ORDER BY clause

You use the ORDER BY clause to sort the records in the resulting list. Use ASC to sort the results in ascending order and DESC to sort the results in descending order.

For example, with ASC:
SELECT *
FROM Employees
ORDER BY HireDate ASC
And with DESC:
SELECT *
FROM Books
ORDER BY type, price DESC

#### SELECT statement with GROUP BY clause

The GROUP BY clause is used to create one output row per each group and produces summary values for the selected columns, as shown below.

SELECT type
FROM Books
GROUP BY type

Here is an example using the above statement.

SELECT type AS ‘Type’, MIN(price) AS ‘Minimum Price’
FROM Books
WHERE royalty > 10
GROUP BY type

If the SELECT statement includes a WHERE criterion where price is not null,

SELECT type, price
FROM Books
WHERE price is not null

then a statement with the GROUP BY clause would look like this:

SELECT type AS ‘Type’, MIN(price) AS ‘Minimum Price’
FROM Books
WHERE price is not null
GROUP BY type

#### Using COUNT with GROUP BY

We can use COUNT to tally how many items are in a container. However, if we want to count different items into separate groups, such as marbles of varying colours, then we would use the COUNT function with the GROUP BY command.

The below SELECT statement illustrates how to count groups of data using the COUNT function with the GROUP BY clause.

SELECT COUNT(*)
FROM Books
GROUP BY type

------

#### INSERT statement

The INSERT statement adds rows to a table. In addition,
  * INSERT specifies the table or view that data will be inserted into.
  * Column_list lists columns that will be affected by the INSERT.
  * If a column is omitted, each value must be provided.
  * If you are including columns, they can be listed in any order.
  * VALUES specifies the data that you want to insert into the table. VALUES is required.
  * Columns with the IDENTITY property should not be explicitly listed in the column_list or values_clause.

The syntax for the INSERT statement is:

INSERT [INTO] Table_name | view name [column_list]
DEFAULT VALUES | values_list | select statement

When inserting rows with the INSERT statement, these rules apply:
  * Inserting an empty string (‘ ‘) into a varchar or text column inserts a single space.
  * All char columns are right-padded to the defined length.
  * All trailing spaces are removed from data inserted into varchar columns, except in strings that contain only spaces. These strings are truncated to a single space.
  * If an INSERT statement violates a constraint, default or rule, or if it is the wrong data type, the statement fails and SQL Server displays an error message.

When you specify values for only some of the columns in the column_list, one of three things can happen to the columns that have no values:
1.	A default value is entered if the column has a DEFAULT constraint, if a default is bound to the column, or if a default is bound to the underlying user-defined data type.
2.	NULL is entered if the column allows NULLs and no default value exists for the column.
3.	An error message is displayed and the row is rejected if the column is defined as NOT NULL and no default exists.

#### Inserting rows with a SELECT statement

We can sometimes create a small temporary table from a large table. For this, we can insert rows with a SELECT statement. When using this command, there is no validation for uniqueness. Consequently, there may be many rows with the same pub_id in the example below.

This example creates a smaller temporary Publishers table using the CREATE TABLE statement. Then the INSERT with a SELECT statement is used to add records to this temporary Publishers table from the publis table.

CREATE TABLE dbo.tmpPublishers (
PubID char (4) NOT NULL ,
PubName varchar (40) NULL ,
city varchar (20) NULL ,
province char (2) NULL ,
country varchar (30) NULL DEFAULT (‘Canada’)
)
INSERT tmpPublishers
SELECT * FROM Publishers

In this example, we’re copying a subset of data.

INSERT tmpPublishers (pub_id, pub_name)
SELECT PubID, PubName
FROM Publishers

In this example, the publishers’ data are copied to the tmpPublishers table and the country column is set to Canada.

INSERT tmpPublishers (PubID, PubName, city, province, country)
SELECT PubID, PubName, city, province, ‘Canada’
FROM Publishers

------

#### UPDATE statement

The UPDATE statement changes data in existing rows either by adding new data or modifying existing data. 

This example uses the UPDATE statement to standardize the country field to be Canada for all records in the Publishers table.

UPDATE Publishers
SET country = ‘Canada’

This example increases the royalty amount by 10% for those royalty amounts between 10 and 20.

UPDATE roysched
SET royalty = royalty + (royalty * .10)
WHERE royalty BETWEEN 10 and 20

#### Including subqueries in an UPDATE statement

The employees from the Employees table who were hired by the publisher in 2010 are given a promotion to the highest job level for their job type. This is what the UPDATE statement would look like.

UPDATE Employees
SET job_lvl =
(SELECT max_lvl FROM jobs
WHERE employee.job_id = jobs.job_id)
WHERE DATEPART(year, employee.hire_date) = 2010

------

#### DELETE statement

The DELETE statement removes rows from a record set. DELETE names the table or view that holds the rows that will be deleted and only one table or row may be listed at a time. WHERE is a standard WHERE clause that limits the deletion to select records.

The DELETE syntax looks like this.

DELETE [FROM] {table_name | view_name }
[WHERE clause]

The rules for the DELETE statement are:
1.	If you omit a WHERE clause, all rows in the table are removed (except for indexes, the table, constraints). 
2.	DELETE cannot be used with a view that has a FROM clause naming more than one table. (Delete can affect only one base table at a time.)

What follows are three different DELETE statements that can be used.
1. Deleting all rows from a table.

DELETE
FROM Discounts

2. Deleting selected rows:

DELETE
FROM Sales
WHERE stor_id = ‘6380’

3. Deleting rows based on a value in a subquery:

DELETE FROM Sales
WHERE title_id IN
(SELECT title_id FROM Books WHERE type = ‘mod_cook’)

------

#### Joining Tables

Joining two or more tables is the process of comparing the data in specified columns and using the comparison results to form a new table from the rows that qualify. A join statement:
  * Specifies a column from each table
  * Compares the values in those columns row by row
  * Combines rows with qualifying values into a new row

Although the comparison is usually for equality – values that match exactly – other types of joins can also be specified. All the different joins such as inner, left (outer), right (outer), and cross join will be described below.

#### Inner join

An inner join connects two tables on a column with the same data type. Only the rows where the column values match are returned; unmatched rows are discarded.

#### Example #1

SELECT jobs.job_id, job_desc
FROM jobs
INNER JOIN Employees ON employee.job_id = jobs.job_id
WHERE jobs.job_id < 7

#### Example #2

SELECT authors.au_fname, authors.au_lname, books.royalty, title
FROM authorsINNER JOIN titleauthor ON authors.au_id=titleauthor.au_id
INNER JOIN books ON titleauthor.title_id=books.title_id
GROUP BY authors.au_lname, authors.au_fname, title, title.royalty
ORDER BY authors.au_lname

#### Left outer join

A left outer join specifies that all left outer rows be returned. All rows from the left table that did not meet the condition specified are included in the results set, and output columns from the other table are set to NULL.

This first example uses the new syntax for a left outer join.

SELECT publishers.pub_name, books.title
FROM Publishers
LEFT OUTER JOIN Books On publishers.pub_id = books.pub_id

This is an example of a left outer join using the old syntax.

SELECT publishers.pub_name, books.title
FROM Publishers, Books
WHERE publishers.pub_id *= books.pub_id

#### Right outer join

A right outer join includes, in its result set, all rows from the right table that did not meet the condition specified. Output columns that correspond to the other table are set to NULL.

Below is an example using the new syntax for a right outer join.

SELECT titleauthor.title_id, authors.au_lname, authors.au_fname
FROM titleauthor
RIGHT OUTER JOIN authors ON titleauthor.au_id = authors.au_id
ORDERY BY au_lname

This second example show the old syntax used for a right outer join.

SELECT titleauthor.title_id, authors.au_lname, authors.au_fname
FROM titleauthor, authors
WHERE titleauthor.au_id =* authors.au_id
ORDERY BY au_lname

#### Full outer join

A full outer join specifies that if a row from either table does not match the selection criteria, the row is included in the result set, and its output columns that correspond to the other table are set to NULL. 

Here is an example of a full outer join.

SELECT books.title, publishers.pub_name, publishers.province
FROM Publishers
FULL OUTER JOIN Books ON books.pub_id = publishers.pub_id
WHERE (publishers.province <> “BC” and publishers.province <> “ON”)
ORDER BY books.title_id

------

#### Key Terms
  * aggregate function: returns summary values
  * ASC: ascending order
  * conversion function: transforms one data type to another
  * cross join: a product combining two tables
  * date function: displays information about dates and times
  * DELETE statement: removes rows from a record set
  * DESC: descending order
  * full outer join: specifies that if a row from either table does not match the selection criteria
  * GROUP BY: used to create one output row per each group and produces summary values for the selected columns
  * inner join: connects two tables on a column with the same data type
  * INSERT statement: adds rows to a table
  * left outer join: specifies that all left outer rows be returned
  * mathematical function: performs operations on numeric data
  * right outer join: includes all rows from the right table that did not meet the condition specified
  * SELECT statement: used to query data in the database
  * string function: performs operations on character strings, binary data or expressions
  * system function: returns a special piece of information from the database
  * text and image functions: performs operations on text and image data
  * UPDATE statement: changes data in existing rows either by adding new data or modifying existing data
  * wildcard: allows the user to match fields that contain certain letters.

------

#### Managed vs Unmanaged

#### Unmanaged Services

Scaling, fault tolerance, and availability are managed by you.

Unmanaged services are typically provisioned in discrete portions as specified by the user. You must manage how the service responds to changes in load, errors, and situations where resources become unavailable.

For example, if you create and launch a web server on an Amazon Elastic Compute Cloud (Amazon EC2) instance. Because Amazon EC2 is an unmanaged solution, that web server will not scale to handle increased traffic load or replace unhealthy instances with healthy ones unless you specify that it use a scaling solution, such as AWS Automatic Scaling.

The benefit to using an unmanaged service is that you have more fine-tuned control over how your solution handles changes in load, errors, and situations where resources become unavailable.

#### Managed Services

Scaling, fault tolerance, and availability are typically built in to the service.

Managed services require the user to configure the service, however, much of the the underlying patching, backups, ensuring availability, and more are managed by the service provider. You must configure how the service responds to changes in load, errors, and situations where resources become unavailable, and the service provider must respond accordingly

For example, you create an Amazon Simple Storage Service (Amazon S3) bucket and then set permissions for it. However, managed services typically require less configuration. Say that you have a static website that you host in a cloud-based storage solution, such as Amazon S3. The static website does not have a web server. However, because Amazon S3 is a managed solution, features such as scaling, fault-tolerance, and availability would be handled automatically and internally by Amazon S3.

------










