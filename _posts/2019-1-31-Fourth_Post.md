---
layout: post
title: Week Four-
---
This week was full of loops, functions, Boolean operators, logic and much more!

The lectures we watched for this week's lesson introduced us to how to handle missing values in data sets, the creation of functions, various loop types and using Boolean operators to use in logical statements. The readings this week went in depth on these various loop types, understanding variable environments and how to begin using functions in our code.

The assignment for the week was to display data from a local hospital using a side-by-side boxplot and a histogram. The data consisted of 5 columns of data for ten patients. The data was frequency of the patient's visits to the hospital over the last twelve months, blood pressure, assessment from the first doctor, assessment from the second doctor in terms and assessment from the head of the emergency unit. The first doctor's assessments are in terms of good or bad condition. Then the second and third doctors assessment is using low and high priority. The data frame containing all of this data is shown below:

![](http://gdurl.com/SuIp) #patientdata dataframe

The first objective is to create side-by-side boxplots. I decided it would be of interest to compare the patient statistics between patients determined to be in good condition or of low priority and those in bad condition or high priority as determined by the three doctors. Since some doctors ranked the patient good/low and the others could have found the patient to be bad/high, we would need to do three sets of side-by-side boxplots. Additionally, since we are comparing good/low to bad/high we need to separate the patient data by good/low or bad/high for each doctor.

Once I had the data properly organized, I used the boxplot function built into R to create a boxplot showing the range of blood pressure for patients determined good/low and bad/high with using each doctor's evaluation. This could help determine if there are trend between patient status and blood pressure or to compare the three doctor's evaluations to each other. Our final result is shown here:

![](http://gdurl.com/VEdL) #boxplots

Next, we need to create a histogram. Since we have already used side-by-side boxplots to evaluate the blood pressure data, we will create histograms to evaluate patient frequency of visiting a hospital in the last twelve months. We need the data separated by each doctor's evaluation along with whether they were evaluated as good/low or bad/high. After we have done this, we can use the histogram function in R to create the histograms.

I created two different images, the first four histograms below have the frequency of patient hospital visits for all patients determined good/low by each doctor. The histogram in the top left is the data for all patients, for comparison purposes.

![](http://gdurl.com/N0vb) #goodhistograms

The image below contains a similar histogram for the top left and the rest are frequency of patient hospital visists for all patients determined bad/high by each doctor.

![](http://gdurl.com/WotR) #badhistograms

The code for all of this can be found on [my github.](https://github.com/jessicalynnrose/Intro_to_R_Spring_2019/blob/master/week4.R)

I decided to take this evaluation one step further and I am working on writing some code that will evaluate if either or both of the first two doctors evaluations can be used to predict the final doctor's decision and should have that added by the end of the day!
