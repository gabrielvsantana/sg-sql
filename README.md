# SQL and PostgreSQL: The Complete Developer's Guide - Stephen Grider
https://www.udemy.com/course/sql-and-postgresql/

# Table of Contents

1. [Section 1: Simple - But Powerful - SQL Statements](#section-1-simple---but-powerful---sql-statements)
1. [Section 2: Filtering Records](#section-2-filtering-records)
1. [Section 3: Working with Tables](#section-3-working-with-tables)
1. [Section 4: Relating Records with Joins](#section-4-relating-records-with-joins)
1. [Section 5: Aggregation of Records](#section-5-aggregation-of-records)
1. [Section 6: Working with Large Datasets](#section-6-working-with-large-datasets)
1. [Section 7: Sorting Records](#section-7-sorting-records)
1. [Section 8: Unions and Intersections with Sets](#section-8-unions-and-intersections-with-sets)
1. [Section 9: Assembling Queries with SubQueries](#section-9-assembling-queries-with-subqueries)
1. [Section 10: Selecting Distinct Records](#section-10-selecting-distinct-records)
1. [Section 11: Utility Operators, Keywords, and Functions](#section-11-utility-operators-keywords-and-functions)
1. [Section 12: Local PostgreSQL Installation](#section-12-local-postgresql-installation)
1. [Section 13: PostgreSQL Complex Datatypes](#section-13-postgresql-complex-datatypes)
1. [Section 14: Database-Side Validation and Constraints](#section-14-database-side-validation-and-constraints)
1. [Section 15: Database Structure Design Patterns](#section-15-database-structure-design-patterns)
1. [Section 16: How to Build a 'Like' System](#section-16-how-to-build-a-like-system)
1. [Section 17: How to Build a 'Mention' System](#section-17-how-to-build-a-mention-system)
1. [Section 18: How to Build a 'Hashtag' System](#section-18-how-to-build-a-hashtag-system)
1. [Section 19: How to Design a 'Follower' System](#section-19-how-to-design-a-follower-system)
1. [Section 20: Implementing Database Design Patterns](#section-20-implementing-database-design-patterns)
1. [Section 21: Approaching and Writing Complex Queries](#section-21-approaching-and-writing-complex-queries)
1. [Section 22: Understanding the Internals of PostgreSQL](#section-22-understanding-the-internals-of-postgresql)
1. [Section 23: A Look at Indexes for Performance](#section-23-a-look-at-indexes-for-performance)
1. [Section 24: Basic Query Tuning](#section-24-basic-query-tuning)
1. [Section 25: Advanced Query Tuning](#section-25-advanced-query-tuning)
1. [Section 26: Simple Common Table Expressions](#section-26-simple-common-table-expressions)
1. [Section 27: Recursive Common Table Expressions](#section-27-recursive-common-table-expressions)
1. [Section 28: Simplifying Queries with Views](#section-28-simplifying-queries-with-views)
1. [Section 29: Optimizing Queries with Materialized Views](#section-29-optimizing-queries-with-materialized-views)
1. [Section 30: Handling Concurrency and Reversibility with Transactions](#section-30-handling-concurrency-and-reversibility-with-transactions)
1. [Section 31: Managing Database Design with Schema Migrations](#section-31-managing-database-design-with-schema-migrations)
1. [Section 32: Schema vs Data Migrations](#section-32-schema-vs-data-migrations)
1. [Section 33: Accessing PostgreSQL From API's](#section-33-accessing-postgresql-from-apis)
1. [Section 34: Data Access Pattern - Repositories](#section-34-data-access-pattern---repositories)
1. [Section 35: Security Around PostgreSQL](#section-35-security-around-postgresql)
1. [Section 36: Fast Parallel Testing](#section-36-fast-parallel-testing)

<br/>

# Section 1: Simple - But Powerful - SQL Statements

<div align="center"><img src="./diagrams/01-insta/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01-insta/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01-insta/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01-insta/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01-insta/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01-insta/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01-insta/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01-insta/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01-insta/sql-9.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01-insta/sql-10.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01-insta/sql-11.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01-insta/sql-12.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01-insta/sql-13.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01-insta/sql-14.svg" /></div><br/><br/><br/>

<div align="center"><img src="./diagrams/02-insta/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02-insta/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02-insta/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02-insta/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02-insta/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02-insta/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02-insta/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02-insta/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02-insta/sql-9.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02-insta/sql-10.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02-insta/sql-11.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02-insta/sql-12.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02-insta/sql-13.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02-insta/sql-14.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02-insta/sql-15.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02-insta/sql-16.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02-insta/sql-17.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02-insta/sql-18.svg" /></div><br/><br/><br/>

---

<br/>

# Section 2: Filtering Records

<div align="center"><img src="./diagrams/03/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/03/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/03/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/03/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/03/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/03/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/03/sql-7.svg" /></div><br/><br/><br/>

---

<br/>

# Section 3: Working with Tables

<div align="center"><img src="./diagrams/04/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/04/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/04/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/04/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/04/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/04/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/04/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/04/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/04/sql-9.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/04/sql-10.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/04/sql-11.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/04/sql-12.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/04/sql-13.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/04/sql-14.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/04/sql-15.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/04/sql-16.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/04/sql-17.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/04/sql-18.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/04/sql-19.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/04/sql-20.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/04/sql-21.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/04/sql-22.svg" /></div><br/><br/><br/>

<div align="center"><img src="./diagrams/05/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/05/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/05/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/05/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/05/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/05/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/05/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/05/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/05/sql-9.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/05/sql-10.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/05/sql-11.svg" /></div><br/><br/><br/>

---

<br/>

# Section 4: Relating Records with Joins

<div align="center"><img src="./diagrams/06/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/06/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/06/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/06/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/06/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/06/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/06/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/06/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/06/sql-9.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/06/sql-10.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/06/sql-11.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/06/sql-12.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/06/sql-13.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/06/sql-14.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/06/sql-15.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/06/sql-16.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/06/sql-17.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/06/sql-18.svg" /></div><br/><br/><br/>

<div align="center"><img src="./diagrams/07/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/07/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/07/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/07/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/07/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/07/sql-6.svg" /></div><br/><br/><br/>

---

<br/>

# Section 5: Aggregation of Records

<div align="center"><img src="./diagrams/08/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/08/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/08/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/08/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/08/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/08/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/08/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/08/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/08/sql-9.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/08/sql-10.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/08/sql-11.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/08/sql-12.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/08/sql-13.svg" /></div><br/><br/><br/>

---

<br/>

# Section 6: Working with Large Datasets

<div align="center"><img src="./diagrams/09/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-3.svg" /></div><br/><br/><br/>

---

<br/>

# Section 7: Sorting Records

<div align="center"><img src="./diagrams/10/sql-2.svg" /></div><br/><br/><br/>

---

<br/>

# Section 8: Unions and Intersections with Sets

<div align="center"><img src="./diagrams/10/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/10/sql-2.svg" /></div>
<div align="center"><img src="./diagrams/10/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/10/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/10/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/10/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/10/sql-7.svg" /></div><br/><br/><br/>

---

<br/>

# Section 9: Assembling Queries with SubQueries

<div align="center"><img src="./diagrams/09/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-9.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-10.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-11.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-12.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-13.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-14.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-15.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-16.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-17.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-18.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-19.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-20.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-21.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-22.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-23.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-24.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-25.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-26.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-27.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-28.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-29.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/09/sql-30.svg" /></div><br/><br/><br/>

---

<br/>

# Section 10: Selecting Distinct Records

<div align="center"><img src="./diagrams/11/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/11/sql-2.svg" /></div><br/><br/><br/>

---

<br/>

# Section 11: Utility Operators, Keywords, and Functions

<div align="center"><img src="./diagrams/11/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/11/sql-4.svg" /></div><br/><br/><br/>


---

<br/>

# Section 12: Local PostgreSQL Installation


<div align="center"><img src="./diagrams/12/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/12/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/12/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/12/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/12/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/12/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/12/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/12/sql-8.svg" /></div><br/><br/><br/>


---

<br/>

# Section 13: PostgreSQL Complex Datatypes

<div align="center"><img src="./diagrams/13/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/13/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/13/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/13/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/13/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/13/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/13/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/13/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/13/sql-9.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/13/sql-10.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/13/sql-11.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/13/sql-12.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/13/sql-13.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/13/sql-14.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/13/sql-15.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/13/sql-16.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/13/sql-17.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/13/sql-18.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/13/sql-19.svg" /></div><br/><br/><br/>


---

<br/>

# Section 14: Database-Side Validation and Constraints

<div align="center"><img src="./diagrams/14/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/14/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/14/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/14/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/14/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/14/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/14/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/14/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/14/sql-9.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/14/sql-10.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/14/sql-11.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/14/sql-12.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/14/sql-13.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/14/sql-14.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/14/sql-15.svg" /></div><br/><br/><br/>

---

<br/>

# Section 15: Database Structure Design Patterns

<div align="center"><img src="./diagrams/16/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/16/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/16/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/16/sql-4.svg" /></div><br/><br/><br/>

---

<br/>

# Section 16: How to Build a 'Like' System


<div align="center"><img src="./diagrams/16/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/16/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/16/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/16/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/16/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/16/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/16/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/16/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/16/sql-9.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/16/sql-10.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/16/sql-11.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/16/sql-12.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/16/sql-13.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/16/sql-14.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/16/sql-15.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/16/sql-16.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/16/sql-17.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/16/sql-18.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/16/sql-19.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/16/sql-20.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/16/sql-21.svg" /></div><br/><br/><br/>

---

<br/>

# Section 17: How to Build a 'Mention' System

<div align="center"><img src="./diagrams/17/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/17/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/17/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/17/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/17/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/17/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/17/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/17/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/17/sql-9.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/17/sql-10.svg" /></div><br/><br/><br/>

---

<br/>

# Section 18: How to Build a 'Hashtag' System

<div align="center"><img src="./diagrams/18/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/18/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/18/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/18/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/18/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/18/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/18/sql-7.svg" /></div><br/><br/><br/>

---

<br/>

# Section 19: How to Design a 'Follower' System

<div align="center"><img src="./diagrams/19/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/19/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/19/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/19/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/19/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/19/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/19/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/19/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/19/sql-9.svg" /></div><br/><br/><br/>

---

<br/>

# Section 20: Implementing Database Design Patterns

<div align="center"><img src="./diagrams/20/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/20/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/20/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/20/sql-4.svg" /></div><br/><br/><br/>

---

<br/>

# Section 21: Approaching and Writing Complex Queries

## Seeding a Database

<div align="center"><img src="./diagrams/21/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/21/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/21/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/21/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/21/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/21/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/21/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/21/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/21/sql-9.svg" /></div><br/><br/><br/>

## Restoring a Backup

<div align="center"><img src="./diagrams/22/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/22/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/22/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/22/sql-4.svg" /></div><br/><br/><br/>

## Writing Complex Queries

<div align="center"><img src="./diagrams/26/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/26/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/26/sql-3.svg" /></div><br/><br/><br/>

---

<br/>

# Section 22: Understanding the Internals of PostgreSQL

<div align="center"><img src="./diagrams/25/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/25/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/25/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/25/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/25/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/25/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/25/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/25/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/25/sql-9.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/25/sql-10.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/25/sql-11.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/25/sql-12.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/25/sql-13.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/25/sql-14.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/25/sql-15.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/25/sql-16.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/25/sql-17.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/25/sql-18.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/25/sql-19.svg" /></div><br/><br/><br/>

---

<br/>

# Section 23: A Look at Indexes for Performance

<div align="center"><img src="./diagrams/27/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/27/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/27/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/27/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/27/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/27/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/27/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/27/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/27/sql-9.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/27/sql-10.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/27/sql-11.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/27/sql-12.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/27/sql-13.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/27/sql-14.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/27/sql-15.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/27/sql-16.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/27/sql-17.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/27/sql-18.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/27/sql-19.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/27/sql-20.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/27/sql-21.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/27/sql-22.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/27/sql-23.svg" /></div><br/><br/><br/>


<div align="center"><img src="./diagrams/28/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/28/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/28/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/28/sql-4.svg" /></div><br/><br/><br/>

---

<br/>

# Section 24: Basic Query Tuning

<div align="center"><img src="./diagrams/29/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/29/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/29/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/29/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/29/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/29/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/29/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/29/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/29/sql-9.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/29/sql-10.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/29/sql-11.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/29/sql-12.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/29/sql-13.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/29/sql-14.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/29/sql-15.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/29/sql-16.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/29/sql-17.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/29/sql-18.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/29/sql-19.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/29/sql-20.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/29/sql-21.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/29/sql-22.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/29/sql-23.svg" /></div><br/><br/><br/>

---

<br/>

# Section 25: Advanced Query Tuning

<div align="center"><img src="./diagrams/30/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/30/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/30/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/30/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/30/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/30/sql-6.svg" /></div><br/><br/><br/>

---

<br/>

# Section 26: Simple Common Table Expressions

<div align="center"><img src="./diagrams/23/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-3.svg" /></div><br/><br/><br/>

---

<br/>

# Section 27: Recursive Common Table Expressions

<div align="center"><img src="./diagrams/23/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-9.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-10.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-11.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-12.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-13.svg" /></div><br/><br/><br/>


---

<br/>

# Section 28: Simplifying Queries with Views

<div align="center"><img src="./diagrams/24/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/24/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/24/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/24/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/24/sql-9.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/24/sql-10.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/24/sql-11.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/24/sql-12.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/24/sql-13.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/24/sql-14.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/24/sql-15.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/24/sql-16.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/24/sql-17.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/24/sql-18.svg" /></div><br/><br/><br/>

---

<br/>

# Section 29: Optimizing Queries with Materialized Views

<div align="center"><img src="./diagrams/31/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/31/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/31/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/31/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/31/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/31/sql-6.svg" /></div><br/><br/><br/>

---

<br/>

# Section 30: Handling Concurrency and Reversibility with Transactions

<div align="center"><img src="./diagrams/32/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/32/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/32/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/32/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/32/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/32/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/32/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/32/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/32/sql-9.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/32/sql-10.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/32/sql-11.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/32/sql-12.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/32/sql-13.svg" /></div><br/><br/><br/>

---

<br/>

# Section 31: Managing Database Design with Schema Migrations

<div align="center"><img src="./diagrams/33/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/33/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/33/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/33/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/33/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/33/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/33/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/33/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/33/sql-9.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/33/sql-10.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/33/sql-11.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/33/sql-12.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/33/sql-13.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/33/sql-14.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/33/sql-15.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/33/sql-16.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/33/sql-17.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/33/sql-18.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/33/sql-19.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/33/sql-20.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/33/sql-21.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/33/sql-22.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/33/sql-23.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/33/sql-24.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/33/sql-25.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/33/sql-26.svg" /></div><br/><br/><br/>

<div align="center"><img src="./diagrams/34/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/34/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/34/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/34/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/34/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/34/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/34/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/34/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/34/sql-9.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/34/sql-10.svg" /></div><br/><br/><br/>


---

<br/>

# Section 32: Schema vs Data Migrations

<div align="center"><img src="./diagrams/34/sql-11.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/34/sql-12.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/34/sql-13.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/34/sql-14.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/34/sql-15.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/34/sql-16.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/34/sql-17.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/34/sql-18.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/34/sql-19.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/34/sql-20.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/34/sql-21.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/34/sql-22.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/34/sql-23.svg" /></div><br/><br/><br/>

<div align="center"><img src="./diagrams/35/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/35/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/35/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/35/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/35/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/35/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/35/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/35/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/35/sql-9.svg" /></div><br/><br/><br/>

---

<br/>

# Section 33: Accessing PostgreSQL From API's

<div align="center"><img src="./diagrams/36/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/36/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/36/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/36/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/36/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/36/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/36/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/36/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/36/sql-9.svg" /></div><br/><br/><br/>

<div align="center"><img src="./diagrams/37/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/37/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/37/sql-3.svg" /></div><br/><br/><br/>

---

<br/>

# Section 34: Data Access Pattern - Repositories

<div align="center"><img src="./diagrams/37/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/37/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/37/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/37/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/37/sql-8.svg" /></div><br/><br/><br/>

---

<br/>

# Section 35: Security Around PostgreSQL

<div align="center"><img src="./diagrams/37/sql-9.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/37/sql-10.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/37/sql-11.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/37/sql-12.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/37/sql-13.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/37/sql-14.svg" /></div><br/><br/><br/>

---

<br/>

# Section 36: Fast Parallel Testing

<div align="center"><img src="./diagrams/37/sql-15.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/37/sql-16.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/37/sql-17.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/37/sql-18.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/37/sql-19.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/37/sql-20.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/37/sql-21.svg" /></div><br/><br/><br/>


<div align="center"><img src="./diagrams/38/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/38/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/38/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/38/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/38/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/38/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/38/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/38/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/38/sql-9.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/38/sql-10.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/38/sql-11.svg" /></div><br/><br/><br/>

---

<br/>

# Left Over Screenshots!!!




# SEPARATE 1

<div align="center"><img src="./diagrams/01/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01/sql-9.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01/sql-10.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01/sql-11.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01/sql-12.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01/sql-13.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01/sql-14.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01/sql-15.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01/sql-16.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01/sql-17.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01/sql-18.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01/sql-19.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01/sql-20.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01/sql-21.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01/sql-22.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/01/sql-23.svg" /></div><br/><br/><br/>

# SEPARATE 2


<div align="center"><img src="./diagrams/02/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02/sql-9.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02/sql-10.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02/sql-11.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02/sql-12.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02/sql-13.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02/sql-14.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02/sql-15.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02/sql-16.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02/sql-17.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02/sql-18.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02/sql-19.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/02/sql-20.svg" /></div><br/><br/><br/>



# SEPARATE 15
# SEPARATE 21
# SEPARATE 22
# SEPARATE 23

<div align="center"><img src="./diagrams/23/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-5.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-6.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-7.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-8.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-9.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-10.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-11.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-12.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-13.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-14.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-15.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-16.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/23/sql-17.svg" /></div><br/><br/><br/>

# SEPARATE 24

<div align="center"><img src="./diagrams/24/sql-1.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/24/sql-2.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/24/sql-3.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/24/sql-4.svg" /></div><br/><br/><br/>
<div align="center"><img src="./diagrams/24/sql-19.svg" /></div><br/><br/><br/>










