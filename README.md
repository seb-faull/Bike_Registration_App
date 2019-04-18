# A Spring Boot Application (Bike Registration App)

Persistence is an important part of any application and you have options when it comes to building your persistence layer.

This application is using Spring Data JPA, which uses the JPA object relational mapping framework, which ultimately runs SQL and communicates with the database, which is a SQLite database.

Here's what I did to get all of that set up:

## Sqlite
- Since I'm using SQLite as the actual database, that was the first thing that I had to get up and running.

## Spring Data JPA dependency
- Next I added the Spring Data JPA dependency and the database JDBC drivers to the Maven pom. xml file.

## Configured a JPA entity
- Once the dependencies were in place, I configured the connections and converted the bike plain old java object model to a bike JPA entity.

## Created a JPA repository
- Because Spring Data JPA utilizes a DAO pattern or a data access object pattern, I then created a JPA repository interface to handle that.

## Jackson JSON annotations
- Finally, we annotated the bike entity with some Jackson annotations to help customize the JSON payload that the API will ultimately return.
