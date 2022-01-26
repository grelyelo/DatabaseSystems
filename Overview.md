# Database Management Overview
---
## Database Definition

What is a database?
- An integrated collection of related data
- Represents information in the real world 
- Traditional databases use relational model, which organizes data into relations.

---
## DBMS Definition
What is a database management system (DBMS)
---
## Relational Database terminology
**Relation**
- A table with rows (database records) and columns
**Domain**
- The set of possible values for a column
---
## Why use a DBMS?
**Persistence**
- Provide software with the ability to *CREATE* *READ* *UPDATE* and *DELETE* *(CRUD)*
- Backup and recovery

**Performance and Efficiency**
- Provide high speed query processing against large quantities of data
- DBMSs provide query optimizers which determine the best way to satisfy queries. 
  
Example Queries:
- Find each enrollment for student 'abc123' for semester
	- Why is it important for this query to be fast and efficient?
	- We do this fairly often. 
- Determine students who may be a candidate for graduating this semester. 
  
**DBMS Integrated Processing**
- Data can be viewed seperately or as an integrated whole
- Allows more information to be obtained from the data

Example: 
- What sections are both students "abc123" and "bef543" enrolled. 
- What prof teaches courses with average > 3.0?

**Data independance**
- Programs should not have to change because of the following changes to the database:
	- Addition of new fields
	- Addition of new indexes
	- Changes of structure from hashing to indexes
	- Removal of fields which are not referenced by program
- Changes to program should not require changes to the database

**Reduction of Redundancy**
- With proper design we can reduce redundancy 
- Save file space
- Reduce processing requirements (no need to update multiple files)
- Improve integrity

**Centralized Control of Data and Security**
- Centralized group of database administrators (DBAs) are responsible for defining the data and optimizing physical implementation
- DBAs (or security personnel) can define who can access the data and what they can do with it (retrieve, insert, update, delete)
- Enforce integrity constraints

**Concurrent access with integrity**
- provide transactions where all operations in a transaction are done or none of them are allowed
- Since data is i/o intensive, having more users will better utilize the CPU. 
  

---





