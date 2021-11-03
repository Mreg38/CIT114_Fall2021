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




