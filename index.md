---
layout: main
title: PolyJDBC
---

# PolyJDBC

PolyJDBC is a polyglot, lightweight wrapper around standard JDBC drivers with
schema inspection/creation capabilities.

## Target

PolyJDBC primary target are libraries that need light and cross-platform JDBC
persistence. Hibernate is great, but it leaves little place for end-user customization,
which is important when offering a library. It is also quite heavy. PolyJDBC size is
only 97kB, no dependencies except for slf4j logging API.

## Is anyone using it?

Apart from internal projects, there are two OpenSource projects currently using PolyJDBC:

* [SmartParam](http://smartparam.org)
* [JaVers](http://javers.org)

## Features

* polyglot (or better poly-dialect? multiple DB dialect support, including id generation strategies)
* transaction-oriented
* resources (Statements, ResultSets) are managed inside transaction scope
* intiutive transaction commit/rollback support
* option to leave transaction management to external framework (i.e. Spring)
* DDL operation DSL (CREATE TABLE/INDEX/SEQUENCE with constraints, DROP \*)
* SQL query DSL (INSERT, SELECT, UPDATE, DELETE)
* lightweight
* schema inspection (table/sequence exists?)
* schema alteration

## Supported database engines

* H2
* PostgreSQL
* MySQL

## Documentation

Want to know more? Visit [PolyJDBC GitHub](https://github.com/polyjdbc/polyjdbc).

## License

PolyJDBC is published under [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0).
