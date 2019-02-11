---
layout: post
title: Week Five- Matrix Math with R
---


This week we were introduced to a lot of the built in mathematic functions within R such as

Our assignment for this week was to take two matrices (A and B) and find the inverse of them and the determinant of each. First we have to create the matrices, which was achieved using the code below:

`A <-matrix(c(11:13,5:7,46,22,97),nrow=3)`

Before we get started with the rest of this assignment, let's review some information about matrices.

+ The inverse of matrix A is defined as the matrix A^-1 which can be multiplied by A to give the identify matrix (a square matrix in which all the elements of the principal diagonal are ones).
+ One way to determine if a matrix has an inverse is by calculating the determinant.
+ The determinant is a value that can be computed **only on square matrices** and provides information on the linear transformation described by the matrix.
+ If the **determinant of the matrix is equal to 0 then you would be unable to find the inverse** of the matrix.

Lucky for us, R has built in functions that can compute both the inverse of a matrix and the determinant of a matrix. Let's start by first checking that these matrices are square. To do so, I just wrote a quick function that compares the number of rows to the number of columns of the input matrix.

`squarematrix <- function(m) {
  x <- nrow(m)
  y <- ncol(m)
  if (x == y) {
    message("This is a square matrix.")
}  else {
    message("This is not a square matrix.")
}
}`

Alright, now that we know our matrix is square, let's find the determinant. R makes this easy with the function det(). Keep in mind, in order to find the inverse, the determinant should not be equal to zero.

![](http://gdurl.com/Ccgq)

Once we have R calculate the determinant, we can now find the inverse of the matrix. R also has a function to do this, solve().

![](http://gdurl.com/vcqI)

As usual, all the code I wrote for this project can be found on my GitHub [here](https://github.com/jessicalynnrose/Intro_to_R_Spring_2019/blob/master/week5.R).
