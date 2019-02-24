---
layout: post
title: Week Seven- Objects!
---

This post marks officially marks half way through the course! I can't believe it's already been seven weeks. I've really enjoyed learning R so far and am so excited to see what the second half of this course has in store for us!

This week we learned about Object-oriented Programming in R as well S3 and S4 classes. To be completely honest, I will probably have to go back and reread the chapter on OOJ in our book at least one more time after I finish this assignment, but that's what I'm in this class for anyway, to learn!

Our assignment this week was to first load data into R. For this, I chose the famous Kaggle dataset, Titanic: Machine Learning from Disaster. (I'm interested in learning about basic machine learning, so that's why I chose this dataset) To load the data into R and get an idea of what the dataset looked like I ran the following code:

`train <- read.csv("train.csv")

str(train)
summary(train)
head(train)`

Now that we have some information on what the dataset contains, we can get started on the rest of this weeks assignment.

////Next, we are asked to determine if a generic function can be assigned to our data set.

////Finally, we need to see if our dataset can be assigned as an S3 or an s4 object.

### 1. How do you tell what OO system (S3 vs S4) an object is associated with?

A quick way to tell what class an object has is by using the `isS4()` function. When an object is given to this function it returns a logical for whether or not the object has the S4 class attribute. Additionally, the `str()` function is helpful for providing information on not only the class of an object but the overall contents and structure of an object.

### 2. How do you determine the base type (i.e. integer or list) of an object?

The easiest way to determine what type any object is in R is to use the generic function typeof(). It takes any R object in put and will return what that object is in R. A few examples can be seen below with our dataset.

////![](www)

### 3. What is a generic function?

Object-oriented programming has four major qualities that describe some of the most important advantages that OOP can provide in a program. These four qualities are encapsulation, abstraction, inheritance and polymorphism.

+ Encapsulation reduces complexity and increases reusability by grouping related variables and functions operating on these objects.
+ Abstraction reduces complexity and isolates the impact of changes.
+ Inheritance eliminates redundant code by allowing a new object inherit properties of a previously created object.
+ Polymorphism allows for a function to lead to different operations for different classes.

With this information, the question can be answered rather simply. Generic functions is how OOP with R is polymorphic. When a generic function is called, R reroutes the call depending on the objects class.

### 4. What are the main differences between S3 and S4?

| S3     | S4     |
|:------:|:------:|
| lacks formal definition | defined using `setClass()` function|
| objects are created by setting the class attribute| objects are created using `new()` function|
| methods below to generic functions| methods belong to generic functions|
