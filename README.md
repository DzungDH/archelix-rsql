# rsql-querydsl [![Build Status](https://api.travis-ci.org/vineey/archelix-rsql.svg?token%2FkdSmFoN3e8GGHqffx761)](https://travis-ci.org/vineey/archelix-rsql )

This library brings the convenience of SQL declarative nature to restful APIs in the form of RSQL
but without the danger of sql injection by using a typesafe mapping of allowed field paths defined
via integration with querydsl library. Like sql, it supports clauses such as select, filter, pagination 
and sorting that can easily be represented in http request parameters.

It primarily supports JPA model but if possible will strive to handle other kinds of database such as MongoDB.
This is a small project but at its heart is dedicated to maintain highly cohesive and modular components.
Contributions and suggestions are very much welcome and appreciated!


##QueryDSL API
* Filter - uses https://github.com/jirutka/rsql-parser[rsql-parser] library ast to convert filter string into its querydsl predicate equivalent
* Select - converts a simple enumeration of selector separated by comma into its querydsl projection equivalent
* Page - converts page parameters into its querydsl pagination equivalent
* Sort - converts sort parameters into its querydsl sorting equivalent

##Milestones

###M1
Completes filter conversion to querydsl predicate.

###M2
Completes sort and page conversion for rsql querydsl
Tentative : Supports Mongodb filter, sort and page conversion.

###M3
Completes select conversion to  querydsl projections.
Tentative : Supports Mongodb selet conversion.

##MAVEN

```xml
<dependency>
    <groupId>com.archelix</groupId>
    <artifactId>rsql-querydsl</artifactId>
    <version>1.0.0M1</version>
</dependency>
```

##DOCS
To be follow
