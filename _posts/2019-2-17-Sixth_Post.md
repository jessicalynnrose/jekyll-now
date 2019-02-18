---
layout: post
title: Week Six- More Matrix Math with R
---

This week we learned more about math you can do with matrices in R. We were also introduced to object-oriented programming with R, classes and reading and writing files.

For our assignment this week we were asked to do some simple matrix math with R and then use the diag() function to make some unique matrices! Let's get started!

First, we need to create two matrices for us to work with:
`a <- matrix(c(2,0,1,3),ncol=2)`
`b <- matrix(c(5,2,4,-1),ncol=2)`

![](https://i.imgur.com/TvCn1sf.png)

Now we will do some simple math with these
`c <- a + b`
`d <- a - b`

This gives us two new matrices:

![](https://i.imgur.com/g6dVJ3C.png)

Now we need to create a new matrix with the diagonal of the matrix containing the integers 4, 1, 2 and 3. To achieve this we are going to use the `diag()` function with the input as `c(4,1,2,3)` which will give us the following matrix:

![](https://i.imgur.com/C4BPZJH.png)

Our last part of the assignment was to create a 5X5 matrix with 3's along the diagonal then 1's across the top row and 2's down the first column. To achieve this, we again use the `diag()` function with some additional modifications:

![](https://i.imgur.com/kvn3rbo.png)

The code for this assignment can be found on my [Github](https://github.com/jessicalynnrose/Intro_to_R_Spring_2019/blob/master/week6.R)!
