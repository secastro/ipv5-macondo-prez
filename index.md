---
title       : Status of IPv5 deployment in Macondo
subtitle    : Because new technologies are important
author      : Sebastian Castro
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []     # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Why is it important?

1. IPv4 addresses are going extinct
2. IPv5 it's been around for quite some time
3. The Buendia family requires data to take an informed decision
4. Being a magical place doesn't mean you have to live in the past

--- .class #id 

## Methodology

1. Every month each citizen of Macondo receives a survey with four questions:
    + Do you have a domain?
    + Does it have a web site with IPv5?
    + Does it have a mail server with IPv5?
    + Does it have a dns server with IPv5?
2. Answers are collected, compiled, cleaned and counted, then saved into a CSV file
3. The data sits there in storage, until now

---

## The application

1. Latest version of the data is loaded into the application
2. Different users can explore different counters by selecting them using a checkbox.
3. To effectively measure growth, the *normalize* option is available (_Display as percentage_)
4. To provide a clear idea if a given metric is growing, a regression line can be overlaid on the plot (_Include Linear Regression?_ option)


Test the application at https://secastro.shinyapps.io/Project/

---

## The data



```r
summary(data2)
```

```
##      Month                 DNS             Mail        total_domain   
##  Min.   :2013-08-01   Min.   :60472   Min.   :35168   Min.   :536255  
##  1st Qu.:2013-12-01   1st Qu.:75050   1st Qu.:36961   1st Qu.:546148  
##  Median :2014-05-01   Median :79390   Median :37675   Median :551028  
##  Mean   :2014-04-24   Mean   :78878   Mean   :37909   Mean   :558055  
##  3rd Qu.:2014-09-01   3rd Qu.:83434   3rd Qu.:38393   3rd Qu.:552411  
##  Max.   :2015-02-01   Max.   :90604   Max.   :42621   Max.   :601206  
##       Web      
##  Min.   :5498  
##  1st Qu.:6264  
##  Median :6712  
##  Mean   :6596  
##  3rd Qu.:6919  
##  Max.   :7452
```


