---
layout: post
title: Week Eight- Strings, Input and More
---

With everything we've been learning in this class, I've never felt the saying "The more you know, the more you don't know." could be more true. There are a lot of packages available, to do almost anything! Excited to use more as we complete our assignments every week!

This week we've spent some time getting introduced to input/output methods, string manipulation and the plyr package.

For our assignment this week, we are loading a small dataset in R to do some string manipulation and write new files with subsets of the data.

To read in the data, I used read.csv. Then, using lapply, we find the mean of both Age and Grade split by gender.

`studentavg <- ddply(week6data,"Sex",transform,Grade.Average=mean(Grade))`

This will write an additional column to the file, which we use `write.table` to create a new file.

Finally, we want to subset the data to include only names that have a lower or uppercase "I". To accomplish this, we used the subset function.

`subset(x,grepl("[Ii]",x$Name))`

Then, we write this to a separate file as well.

The code for this assignment can be found on my [Github](https://github.com/jessicalynnrose/Intro_to_R_Spring_2019/blob/master/wee8.R).
