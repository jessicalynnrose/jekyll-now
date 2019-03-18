---
layout: post
title: Week Nine- Data Visualization with R
---

This lesson this week was all about different data visualization functions and packages in R. We learned about basic visualization that is built into R, a very common, widely used package called ggplot2 and another package called Lattice. This has been so much fun, there's so much data out there and learning how to create different data visualizations helps the data tell a story.

For this assignment this week, we were to pick a dataset from Vincent Arel Bundock dataset list and create three different visualizations. As a bioinformatics major it seemed fitting to use a melanoma data set that contains the following information:

**Size:** 205 observations of 8 variables

**Variables:**
* X- patient ID
* time- survival in days since operation
* status- 1 = died from melanoma 2 = survived 3 = died from causes unrelated to melanoma
* sex- 1 = male 0 = female
* age- age in years at the time of operation
* year- year of the operation
* thickness- tumor thickness in mm
* ulcer- 1 = ulcer present 0 = ulcer absent

After loading the data into R, the first thing I did was get a glimpse of what the dataset looks like:

`str(week9data)
summary(week9data)
head(week9data)`

Now that I have a good understanding of the values for each observation, we need to think about what relationships would be the most useful to find out. Obviously we are interested in anything that could provide insight on a factor that correlates to a higher than average instance of patient status being 2(survived). The graph below shows the status plotted for all patients.

![](https://i.imgur.com/7KrCyj8.png)

Now that I have all this information, I can start to ask some questions!

1. Could sex of patient impact survival status?

![](https://i.imgur.com/b4MU4oz.png)

2. Could presence of an ulcer impact survival status?

![](https://i.imgur.com/yiBekBM.png)

3. Could the thickness of the tumor impact survival status?

![](https://i.imgur.com/BB2F0wd.png)

These are just a couple of examples of plots we can make with ggplot2 to provide insight on the data set. All my code can be found [here](https://github.com/jessicalynnrose/Intro_to_R_Spring_2019/blob/master/week9.R)!
