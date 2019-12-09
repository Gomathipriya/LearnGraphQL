# LearnGraphQL

## Introduction

* New API standard that proides  more efficient, powerful and fexible alternative to REST
* A client can simply get exactly what data it wants ( from multiple sources) from a single end point
* Not a query language for DB - querylanguage for API
* Works based on strongly typed schemas

REST API
```
/api/students/<id>
/api/students/<id>/classes
```
GraphQL
```
query {
  Student (id:1) {
    firstName
    lastName
    Classes {
      className 
    }
  }
}
```

#### Schemas

How GraphQL defines and structures data it receives

#### Schema Definition Language (SDL)

* Syntax for writing schemas
* queries and mutations - composed to get back the required information from the server
* Completely flexible structure of data returned - query has to be extremely specific in what is required
* If something specified in schema is nt returned , response will contain null for that field it will not throw exception like REST

