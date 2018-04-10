# Database Systems and Data Thinking

## Questions to Consider When Thinking About Data
* What is my data?
* How is my data structured?
* How can I relate different parts of data?
* How much data will I need to store?
* How frequently will new data be added, existing data be changed and read?
* How frequently and how drastically will the structure of my data change as my product grows?

## Case Studies
* When to use relational DB?
	* Webapps / Websites -  MySQL are the most common versatile dbs good for most projects that involve data storing and querying on the web
	* Embedded Devices - SQLite is great for isolated environments, stores everything in a single file and keeps indexes in memory
	* Analytics - Vertica is one of many databases designed to store large amounts of data with ability to create custom queries. 
* When to use NoSQL DB?
	* Rapid Prototyping - Mongo DB is great for updating schema as project evolves
	* Offline/Online Synching - Pouch DB with Couch DB offers an excellent low-conflict solution for offline implementations
	* Key-Value Store - Redis is super fast and efficient at storing key-value data in-memory for fast performance and quick lookup
	* Large Column & High Performance - Cassandra is great for large column data sets and peforms incredibly fast 
	
## Relational Databases
* Pros
	* Structured
	* ACID-safe
	* Tables can be related to one another
	* Available DBs are fairly consistent and standardized, strengths and weaknesses are somewhat uniform
* Cons
	* Structured nature can cause additional overhead
	* Need to consider normalization forms
* Some Examples - And When to Use Them
	* Oracle - I can pay for the licensing fee! And I want something generally stable and performant
	* MySQL/Maria - I can't pay for the licensing fee! And I want something generally stable and performant
	* PostgreSQL - I need to lots of data sharding and store large formats (blobs, big files)
	* SQLite - I need something simple that I can set up quickly
	* Microsoft SQL - I am using a Microsoft tech stack

## NoSQL Databases
* Pros
	* Fast AF, especially when used in the right situation
	* Able to handle unstructured data
* Cons
	* Need to be able to handle unstructured data
	* Many aren't ACID-safe by default, or require performance hits to do so
	* Can't relate objects to each other
	* Offerings can vary widely, so you need to know what situation calls for what tool
* Some Examples - And When to Use Them
	* MongoDB - TODO: why
	* Cassandra - TODO: why

## Important Considerations
* Don't hand-write your queries in your application code! Use an ORM or other library to interact with your DB(s)
* Databases are incredibly complex; scaled companies hire people (called Database Administrators, DBAs) to do database things full-time
* There are database options in the cloud as well, with companies starting to offer databases as a service

## Resources

### [Upwork (SQL vs NoSQL Databases)](https://www.upwork.com/hiring/data/sql-vs-nosql-databases-whats-the-difference/)
### [Visual guide to DBs)](http://blog.nahurst.com/visual-guide-to-nosql-systems)
