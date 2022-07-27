# What is Spring Data?

## Learning Goals

- Define Spring Data.
- Give an overview of its features and different modules

## Introduction

Spring Data is a project in the Spring ecosystem that provides persistence
technology specific implementations to simplify the persistence layer
development. It provides a unified way of data access. It also offers additional
features for database easier interaction such as:

- **Repository:** Spring Data provides data abstraction through repositories.
  The central interface is called `Repository`. This interface primarily marks a
  class as a Spring Data repository but it doesn’t provide any additional
  methods. There are other interfaces such as `CrudRepository` that extend from
  this interface to provide common methods for database interaction.
- **Repository Method Name Based Query Generation:** automatically generates SQL
  queries based on the method name defined in a repository.
- **Custom Queries:** flexibility to use native queries in case the automatic
  queries are not enough.
- **Simple Configuration:** makes it easy to configure the database.

## Spring Data Subprojects

The Spring Data project contains several subprojects for specific databases
which makes it easy to use across the most common databases. Here are some of
the most common subprojects:

- **Spring Data Commons:** the core module that provides common functionality
  for interacting with databases such as repositories and transactions.
- **Spring Data JDBC:** provides a way to use JDBC (Java DataBase Connectivity)
  API with repositories.
- **Spring Data JPA:** a feature complete implementation of the JPA
  specification with an additional layer on top of it for even more convenient
  functionality.
- **Spring Data REST:** allows using Spring Data repositories as REST services.
  It requires the Spring Web module to work properly.

## Conclusion

We have learned about Spring Data in this module and the several advantages it
provides us for interacting with databases. In the next lessons, we will learn
more about repositories and use them in a sample project.

## References

- [Spring Data Reference Docs](https://docs.spring.io/spring-data/jpa/docs/current/reference/html/)
