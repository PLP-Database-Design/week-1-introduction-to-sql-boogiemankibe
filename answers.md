# SQL Assignment Week 1


## *What You'll Need*
- A computer with internet access.
- A code editor (e.g., Visual Studio Code).
- MySQL Workbench or another SQL database environment.

---



## *Submission Instructions*
1. Answer every question below and put your responses in a file named `answers.md`
2. Push your completed `answers.md` file to your GitHub repository.
3. Submit the GitHub link for review.

---

## **Assignment Questions**

1. State and Explain the components of a DBMS(Database Management System)
   A Database Management System (DBMS) is a software tool that provides an interface for users to interact with a database. It is designed to store, retrieve, manage, and manipulate data efficiently. A DBMS consists of several key components, each with a specific role in the system's overall operation. These components are as follows:
1. Database Engine

Description: The core service for accessing, managing, and processing data in the database.

    Functions:
        Executes database queries (SQL statements).
        Manages data storage, retrieval, and modification.
        Ensures data integrity and consistency.
    Importance: Serves as the foundation of the DBMS, directly handling user commands and system instructions for data operations.

2. Database Schema

Description: The logical structure or blueprint of the database.

    Functions:
        Defines tables, columns, data types, relationships, indexes, and constraints.
        Provides metadata (data about data), guiding how the data is organized and used.
    Importance: Ensures data organization and supports application requirements.

3. Query Processor

Description: The intermediary between user queries and the database engine.

    Functions:
        Interprets and analyzes SQL queries.
        Optimizes query execution plans for performance.
        Translates user requests into commands that the database engine can execute.
    Importance: Enhances performance and ensures correct query results.

4. Data Manager (or Storage Manager)

Description: Responsible for managing the physical storage of data.

    Functions:
        Handles data files on storage devices.
        Manages data access permissions and recovery mechanisms.
        Coordinates with the operating system for efficient storage utilization.
    Importance: Ensures data is stored securely and is recoverable in case of failures.

5. Transaction Manager

Description: Manages database transactions to ensure they are executed safely and correctly.

    Functions:
        Implements ACID (Atomicity, Consistency, Isolation, Durability) properties.
        Coordinates concurrent transactions to avoid conflicts (e.g., deadlocks or race conditions).
        Ensures data consistency during system failures or errors.
    Importance: Provides reliability and ensures integrity of data in multi-user environments.

6. Metadata Manager

Description: Maintains metadata that describes the database structure and its contents.

    Functions:
        Stores schema definitions and data mappings.
        Tracks indexes, constraints, and relationships.
        Supports the query processor in understanding the database.
    Importance: Facilitates efficient data management and query optimization.

7. User Interface

Description: The means by which users interact with the DBMS.

    Functions:
        Provides a graphical user interface (GUI) or command-line interface (CLI).
        Allows users to execute queries, view reports, and manage data visually.
    Importance: Enhances usability and accessibility for diverse user groups.

8. Security Manager

Description: Manages database security and user access controls.

    Functions:
        Authenticates users and assigns roles/permissions.
        Prevents unauthorized access and protects sensitive data.
        Implements encryption and auditing mechanisms.
    Importance: Ensures data privacy and compliance with security policies.

9. Backup and Recovery Manager

Description: Handles data backup and recovery to ensure data durability.

    Functions:
        Creates periodic backups to prevent data loss.
        Restores data in case of corruption or system failure.
    Importance: Provides disaster recovery and ensures business continuity.

2. What is a relational database? Give 4 examples.
    What is a Relational Database?

A relational database is a type of database that organizes and stores data in a structured format, using tables (also known as relations). Each table consists of rows (records or tuples) and columns (attributes), with each row representing a unique instance of data and each column holding specific types of data about that instance.

The relational database model is based on relational algebra and was first introduced by Edgar F. Codd in the 1970s. It uses keys (primary keys, foreign keys) to establish relationships between tables, enabling users to retrieve and manage data efficiently through Structured Query Language (SQL).
Key Features of a Relational Database

    Data Organization: Data is stored in tabular format for clarity and accessibility.
    Relationships: Tables can be linked using keys to represent real-world relationships.
    SQL Support: SQL is used for querying, inserting, updating, and deleting data.
    Data Integrity: Ensures accuracy and consistency of data through constraints like primary keys, foreign keys, and unique constraints.
    Scalability: Can handle small-scale to large-scale datasets efficiently.

Examples of Relational Databases

Here are four widely used relational database systems:

    MySQL:
        Open-source and highly popular.
        Known for its speed, reliability, and ease of use.
        Commonly used in web applications and small to medium-sized enterprises.

    PostgreSQL:
        Advanced open-source relational database.
        Offers extensive features such as support for complex queries, advanced data types, and full-text search.
        Known for its stability and standards compliance.

    Microsoft SQL Server:
        Developed by Microsoft, a commercial relational database system.
        Provides enterprise-grade features such as business intelligence tools, integration services, and robust security.
        Commonly used in large-scale corporate environments.

    Oracle Database:
        A high-performance commercial relational database system.
        Designed for mission-critical applications with extensive support for scalability, security, and high availability.
        Often used in enterprise-level applications, especially in finance and government.

3. State and Explain three classifications of SQL?
   1. Data Definition Language (DDL)
DDL consists of SQL commands that define, modify, and manage database structures. This includes creating, altering, and deleting tables and other database objects. DDL commands are crucial for establishing the schema of a database.

    Common DDL Commands:
        CREATE: Used to create new database objects such as tables or indexes.
        ALTER: Modifies the structure of existing database objects.
        DROP: Deletes existing database objects from the database.

For example, a command like CREATE TABLE employees (...) defines a new table structure in the database.

2. Data Manipulation Language (DML)
DML includes SQL commands that deal with the manipulation of data within the database. This classification allows users to insert, update, delete, and retrieve data stored in tables.

    Common DML Commands:
        INSERT: Adds new records into a table.
        UPDATE: Modifies existing records in a table.
        DELETE: Removes records from a table.

An example would be INSERT INTO employees (first_name, last_name) VALUES ('John', 'Doe');, which adds a new employee record to the employees table.

3. Data Control Language (DCL)
DCL encompasses SQL commands that control access to data within the database. These commands are essential for managing user permissions and ensuring data security.

    Common DCL Commands:
        GRANT: Provides specific privileges to users or roles.
        REVOKE: Withdraws previously granted privileges from users or roles.

4. What is the difference between a Primary Key and a Foreign Key?
    Primary Key vs. Foreign Key

Key Differences
Aspect	          Primary Key                                         	Foreign Key
Definition	Uniquely identifies a record in its own table.     	References the primary key in another table.
Uniqueness	      Must be unique.	                           Can have duplicates unless otherwise constrained.
NULL values         Cannot be NULL.	                                  Can be NULL if the relationship is optional.
Purpose	   Identifies records uniquely.	                      Links tables to enforce relationships.
Number per Table	  Only one primary key per table.	           Multiple foreign keys are allowed.
Relationship Role	   Defines the unique identity of a row.	     Ensures referential integrity between tables.

5. What is an Entity-Relationship Diagram?
    An Entity-Relationship Diagram (ERD) is a graphical representation of the data model for a database. It visually depicts the entities (objects or concepts), their attributes, and the relationships between them. ERDs are used during the database design process to understand and model the structure and interconnections of data within the system.
6. What are the advantages of relational databases?
     1. Structured and Organized Data

    Data is stored in tables (rows and columns), which provides a clear and logical organization.
    Relationships between tables ensure that data is systematically connected and easily accessible.

  2. Data Integrity

    Constraints such as primary keys, foreign keys, and unique constraints ensure the accuracy and consistency of data.
    ACID properties (Atomicity, Consistency, Isolation, Durability) ensure reliable transactions and data integrity, even in cases of failures.

  3. Ease of Use with SQL

    Relational databases use Structured Query Language (SQL), a standardized language that is intuitive and powerful for querying and manipulating data.
    SQL enables complex queries, joins, and aggregations to extract meaningful information.

  4. Scalability

    Relational databases can handle large amounts of data efficiently.
    They support vertical scalability (adding more resources like CPU and memory to a single server).

  5. Flexibility in Data Relationships

    Tables can be linked using primary and foreign keys, enabling the modeling of complex relationships.
    Supports one-to-one, one-to-many, and many-to-many relationships.

7. State four types of data type used to store data in tables?
    1. Numeric Data Types

    Purpose: Store numeric values for calculations or measurements.
    Examples:
        INTEGER (INT): Whole numbers (e.g., 1, 42, -100).
        FLOAT/REAL/DOUBLE: Numbers with decimal points (e.g., 3.14, -0.99).
        DECIMAL/NUMERIC: Fixed-point numbers with precision, often used in financial data (e.g., 123.45).

2. String (Character) Data Types

    Purpose: Store textual or alphanumeric data.
    Examples:
        CHAR(n): Fixed-length string (e.g., CHAR(5) stores strings like John_).
        VARCHAR(n): Variable-length string, up to n characters (e.g., VARCHAR(50) for names or addresses).
        TEXT: Large amounts of text (e.g., articles, descriptions).

3. Date and Time Data Types

    Purpose: Store date and time information.
    Examples:
        DATE: Stores dates (e.g., 2024-12-01).
        TIME: Stores time (e.g., 14:30:00).
        DATETIME: Combines date and time (e.g., 2024-12-01 14:30:00).
        TIMESTAMP: Stores date and time with time zone information.

4. Boolean Data Type

    Purpose: Store true/false values or binary conditions.
    Examples:
        BOOLEAN: Stores TRUE, FALSE, or NULL.
   
8. What is the purpose of a database management system (DBMS)?
      The purpose of a Database Management System (DBMS) is to efficiently store, retrieve, and manage data while ensuring data consistency, security, and integrity. It provides tools for data organization, user access control, and query execution, enabling multiple users to interact with the database concurrently and reliably.

*How to edit a [markdownfile](https://www.markdownguide.org/basic-syntax/#headings)*

###  NOTE: You should not fork the repository
