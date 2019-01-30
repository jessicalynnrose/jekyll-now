---
layout: post
title: Week Three- Let's make a data frame
---
This week's lectures and videos focused on learning in depth about matrices, arrays, lists and data frames.


Our assignment for this week was to use some manufactured election poll results and evaluate different statistics analysis used on the data set. First we define the variables, names, ABCpollresults, and CBSpoll results.

![](http://gdurl.com/fTwR)

Next we use cbind which will combine vectors, matrices or data frames by columns to create:

![](http://gdurl.com/XkPzz)

Then we create a data.frame of the results so that we are able to store the columns of this data object as different types.

![](http://gdurl.com/zqiT)

The first statistical analysis we will do with our data is determine the mean of the two columns containing poll results (columns 2 and 3). If we try mean(results.df) it will not work, as it is a summary function and will attempt to take the mean of each column in the data frame. Instead, we could use colMeans and specify the two columns containing the poll result data:

![](http://gdurl.com/5sTZ)

Another helpful function in R, is the ability to convert between matrices and data frames using as.matrix:

![](http://gdurl.com/yGHh)

Similarly, we can convert from data frames back to matrices!

![](http://gdurl.com/S6tH)
