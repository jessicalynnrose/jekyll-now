---
layout: post
title: Week Seven- Objects!
---

Hi :)

### 1. How do you tell what OO system (S3 vs S4) an object is associated with?

### 2. How do you determine the base type (i.e. integer or list) of an object?

The easiest way to determine what type any object is in R is to use the generic function typeof(). It takes any R object in put and will return what that object is in R. A few examples can be seen below with our dataset.

![](www)

### 3. What is a generic function?

Object-oriented programming has four major qualities that describe some of the most important advantages that OOP can provide in a program. These four qualities are encapsulation, abstraction, inheritance and polymorphism.

..* Encapsulation reduces complexity and increases reusability by grouping related variables and functions operating on these objects.
..* Abstraction reduces complexity and isolates the impact of changes.
..* Inheritance eliminates redundant code by allowing a new object inherit properties of a previously created object.
..* Polymorphism allows for a function to lead to different operations for different classes.

With this information, the question can be answered rather simply. Generic functions is how OOP with R is polymorphic. When a generic function is called, R reroutes the call depending on the objects class.

### 4. What are the main differences between S3 and S4?

S3
