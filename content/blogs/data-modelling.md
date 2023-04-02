---
title: "Data Modelling"
date: 2023-04-01
slug: data-modelling
tags: ["Data Engineering", "Data Modelling"]
summary: Data modeling is an essential component in designing efficient and effective databases. So, let's dive in and explore the fascinating world of data modeling!
weight: 2
description: Data modeling is an essential component in designing efficient and effective databases. So, let's dive in and explore the fascinating world of data modeling!
cover: 
  image: 
  alt: 
  caption: 
  relative: true
draft: false
---

## Getting Started to Data Modelling
- Data models provide insights into the major data subjects, attributes of the data, relationships between the data, and the business rules for the data.
- These are some terminologies in data modeling:
  - Entity: A thing or concept in the real world that is represented in the database, such as a person, place, thing, or event.
  - Attributes: Characteristics or properties that describe an entity, such as name, age, address, or date.
  - Relationship: An association between two or more entities, which is used to represent how they are related to each other in the database.

## Types of Data Models
- These are the types of data modeling:
  - Conceptual Data Model: Describes what the system contains in terms of entities, attributes, and relationships, without including implementation details. It provides a high-level view of the data requirements of the system.
  - Logical Data Model: Describes how the system should be implemented, in terms of the data structures, constraints, and rules. It defines the logical relationships between entities, attributes, and relationships, and is independent of any specific database management system (DBMS).
  - Physical Data Model: Describes how the system will be implemented using a specific DBMS system, including details such as data types, indexing, partitioning, and storage. It defines the physical storage structures and access methods for the database.
![](https://i.stack.imgur.com/GYDcP.png)

## Cardinality
- Cardinality refers to the number of relationships between two entities, and is often expressed using the minimum and maximum values.
  - The types of cardinality relationships are:
    - One-to-One (1:1): Each entity in the relationship is related to exactly one other entity.
    - One-to-Many (1:N): One entity in the relationship is related to many instances of the other entity, but the reverse is not true.
    - Many-to-Many (M:N): Each instance of each entity can be related to many instances of the other entity.
  - Crow's foot notation is a visual representation used in data modeling to represent cardinality relationships between entities. It uses various symbols such as lines, diamonds, and circles to represent the types of relationships and the cardinality constraints.
  ![](https://www.relationaldbdesign.com/database-design/module7/images/chen-crowsfoot-notation.jpg)

## Normalization & Denormalization
- Normalization  
    A process that involves breaking down complex tables into smaller and more structured tables, following a set of rules or normal forms, such as 1NF, 2NF, and 3NF, to reduce data redundancy and improve data integrity. It can improve query performance, prevent data loss, and increase data storage efficiency, making it suitable for complex database designs that require high data integrity and allow for flexible and efficient data management.
- Denormalization  
    A process that involves combining multiple tables or entities into one larger table or entity, eliminating relationships or connections between tables to improve query performance and simplify database design. Although it makes data reading easier for applications that require fast and easy data access, it can cause data duplication and may be difficult to maintain data integrity if there are changes to the duplicated data. As a result, it is suitable for databases with large volumes of data.

## Dimensional Modelling
- Dimensional modeling is a data warehouse design technique that organizes data into a structure that is easy to understand and efficient for data analysis.
- Fact and dimension are the two key concepts in dimensional modeling. Fact refers to quantitative or numerical data that can be measured, while dimension refers to the categories or attributes used to group and filter data (context).
- The two data schema models used in dimensional modeling are the star schema and the snowflake schema. The star schema is a simple design with one fact table and multiple dimension tables, while the snowflake schema is a more complex design that allows for more detailed analysis.
- Database keys are used to ensure data integrity. Primary keys can be natural or surrogate, while foreign keys are used to create relationships between tables.
- Policies for historical data include overwrite, maintaining unlimited history, or maintaining limited history, depending on the specific needs of the organization.