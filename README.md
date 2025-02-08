# JPA Finder Methods
Spring Data JPA, a part of the larger Spring Data project, simplifies data access in Java applications by providing powerful features for interacting with databases. One of its key features is the ability to create custom finder methods in repositories.

To begin, Spring Data JPA offers Method Name Query Derivation. By adhering to a specific naming convention like findBy<Property>, we can automatically generate queries based on the method name. For example, findByFirstName(String firstName) generates a query to find entities by their first name.


## Demonstration of Component Mapping through Code
For this I have created one Customer Entity.

One Customer Repository for writing JPA Finder Methods.

Written Test Cases for 3 finder methods.

Customer findByEmailAndName(String email, String name);

Customer findByEmailLike(String email);

Customer findByIdIn(List<Integer> ids);

Use MySql Database for storing customer table.

### Commands Used in MySQL Workbench -

use sys;

CREATE TABLE customer ( id int PRIMARY KEY auto_increment, name varchar(20), city varchar(20), state varchar(20), country varchar(20), zipcode varchar(20) );

select * from customer;
