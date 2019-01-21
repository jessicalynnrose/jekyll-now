---
layout: post
title: Week Two!
---

----
****

During the first week of class, we were introduced to open source software, the history of R, object oriented programming, R packages and GitHub. Next we started learning about different data types in R and how to write basic functions. This was supplemented with reading about the stages of a package and vectors.

This week's assignment is to evaluate the following function:

'myMean <- function(assignment2) { return(sum(assignment)/length(someData)) }'

The data to evaluate this function can be found below:

'assignment2 <- c(16,18,14,22,27,17,19,17,17,22,20,22)'


Evaluation:

This function appears to find the mean of a vector of data by taking the sum of 'assignment' and divides in by the length of 'someData'. The first thing I did was simply create the function and try to run it with the data set given. I received this error when doing so:

![firsttry] firsttry.PNG

After receiving this error message, I reviewed the function. The first problem I see is that the parameter for the function (argument2) is not referenced later anywhere in the function. Also, there are two variables that are not previously defined anywhere (assignment and someData) that are being manipulated in this function.

Some changes I would make to rewrite this function would be changing the argument of the function from argument2 to argument and defining someData to what the length of sum of argument needs to be divided by. The result of my suggested corrections are shown below:

![correctedfunction] /images/corrected.PNG
