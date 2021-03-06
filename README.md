## Installation Guide

#### Run the following to install slidify
```r
install.packages("devtools")
library(devtools)
install_github('ramnathv/slidify')
install_github('ramnathv/slidifyLibraries')
library(slidify)
```

#### Run the following to display the presentation slides
```r
slidify('index.Rmd')
browseURL('index.html')
```

#### Modify your slides in 'index.Rmd'
```r
---
title       : Student Performance Prediction (Shiny App)
subtitle    : Data Miners Group Presentation
author      : Yousef (S2141806), Hanani (S2150141), Jasmeen (S2142739), Loh Cin (S2141070)
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Introduction

1. Brief
2. Questions
3. Data source

--- .class #id 

## Data Preprocessing
<b> Removed attributes due to alot of missing values </b>
 - MJob (Mother Job) (40% Missing Value)
 - FJob (Father Job) (35% Missing Value)

<b>Feature Selection according to heatmap</b>

<img src=assets/img/heatmap.png style="width: 400px"> <img src=assets/img/correlated.png style="width: 400px"> 

--- .class #id
## Machine Learning



--- .class #id
## Shiny App UI
```

#### To display images in your slides 
1. Put your .png/.jpg files in assets/img then include the following (i.e)

```r
## Machine Learning (Machine Learning Slide)
<img src=assets/img/image.png style="width: 400px">  (Image)
```
