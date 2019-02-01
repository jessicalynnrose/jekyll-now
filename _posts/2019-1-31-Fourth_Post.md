---
layout: post
title: Week Four- Getting Graphic
---



Defining patient data
```
freq <- c(0.6,0.3,0.4,0.4,0.2,0.6,0.3,0.4,0.9,0.2)
bp <- c(103,87,32,42,59,109,78,205,135,176)
first <- c("bad", "bad", "bad", "bad", "good", "good", "good", "good", "NA", "bad")
second <- c("low", "low", "high", "high", "low", "low", "high", "high", "high", "high")
final <- c("low", "high", "low", "high", "low", "high", "low", "high", "high", "high")
```

Making the side-by-side boxplots
```
par(mfrow=c(3,1))
boxplot(firstgood$bp,firstbad$bp,horizontal=TRUE,main="BP of Patients (First Doctor Evaluation)",xlab="BP",names=firstnames)
boxplot(secondlow$bp,secondhigh$bp,horizontal=TRUE,main="BP of Patients (Second Doctor Evaluation)",xlab="BP",names=secondandfinalnames)
boxplot(finallow$bp,finalhigh$bp,horizontal=TRUE,main="BP of Patients (Final Doctor Evaluation)",xlab="BP",names=secondandfinalnames)
```

Making the histograms
```
par(mfrow=c(2,2))
hist(patientdata$freq,main="All Patients",xlab="Frequency of Hospital Visits",ylab="Number of Patients",sub="(over the last twelve months)")
hist(firstgood$freq,main="Good Condition Patients (First Doctor)",xlab="Frequency of Hospital Visists",ylab="Number of Patients",sub="(over the last twelve months)")
hist(secondlow$freq,main="Low Priority Patients (Second Doctor)",xlab="Frequency of Hospital Visists",ylab="Number of Patients",sub="(over the last twelve months)")
hist(finallow$freq,main="Low Priority Patients (Final Doctor)",xlab="Frequency of Hospital Visists",ylab="Number of Patients",sub="(over the last twelve months)")
```
