---
title       : Student Performance Prediction (Shiny App)
subtitle    : Data Miners Group Presentation
author      : Yousef Hosny Elsayed (S2141806), Hanani Nurshafira Binti Hamdan (S2150141),                         Jasmeen Bong Kah Ying (S2142739), Loh Cin Ceat (S2141070)
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---


## Introduction

Initial Question

1. What are the characteristics of students who achieve high/low grades?

2. Given a new student, how can we predict the mark of the final grade based on the specific characteristics?

Our product is a shiny app that is powered by regression model and capable for predicting student’s performance in secondary school. The regression model is trained on a data set that predicts the student's final grade.

# Data source

https://archive.ics.uci.edu/ml/datasets/Student+Performance 

P. Cortez and A. Silva. Using Data Mining to Predict Secondary School Student Performance. In A. Brito and J. Teixeira Eds., Proceedings of 5th FUture BUsiness TEChnology Conference (FUBUTEC 2008) pp. 5-12, Porto, Portugal, April, 2008, EUROSIS, ISBN 978-9077381-39-7.

--- .class #id 

## Data Preprocessing
* Removed attributes due to alot of missing values
 - MJob (Mother Job) (40% Missing Value)
 - FJob (Father Job) (35% Missing Value)

<b>Feature Selection according to heatmap</b>

<img src=assets/img/heatmap.png style="width: 400px"> <img src=assets/img/correlated.png style="width: 400px"> 


--- .class #id
## Machine Learning -Linear Regression Model


# Performance of Training Set
MSE:  2.505773 MAE:  0.9221254  RMSE:  1.582963 R2 0.8320791

# Performance of Testing Set
MSE:  2.211841 MAE:  0.9043607  RMSE:  1.487226 R2 0.8320791

# Scatter plot of Training and Testing set
<img src=assets/img/Rplot.png style="width: 450px"> <img src=assets/img/Rplot01.png style="width: 450px"> 

--- .class #id
## Shiny App UI
<img src=assets/img/ui.png style="width: 800px">

# Link to Shiny App
https://jasmeen.shinyapps.io/StudentPerformancePrediction/

# Link to Github
https://github.com/yousefhosny1/student-performance-shiny-app

# Our Experience

