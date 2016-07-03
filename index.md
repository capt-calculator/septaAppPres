---
title       : SEPTA Regional Rail Performance
subtitle    : A Shiny application 
author      : Troy Walters
job         : Data Analyst
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## The Data

* The Southeastern Pennsylvania Transportation Authority (SEPTA) recently made a dataset available on kaggle.com. This dataset contains performance data for SEPTA's regional rail system. 

* Due to the dataset being very large and there being a large number of trains, it made sense to develop a simple app that could show for each train it average runtime, locations, and on-time performance. 

* I first performed some processing of the raw data in which I calculated the run times of each train each day. This resulted in a processed data set that sits underneath the Shiny app. You can find the code that I used to preprocess in the github [repository](https://github.com/capt-calculator/septaApp).

* The data set contains data from March 23, 2016 through May 30, 2016.

---

## Components of the Application

The Shiny application consists of three main parts:

1. Performance information for the selected train
2. A histogram/density plot of the selected train's run times
3. An interactive leaflet map showing the train's measured locations


--- .class #id 

## Train Run Times

A selected train's run times are show as a histsogram and density plot:

<img src="figure/unnamed-chunk-1-1.png" title="plot of chunk unnamed-chunk-1" alt="plot of chunk unnamed-chunk-1" style="display: block; margin: auto;" />

---

## Final Product

A screenshot of the actual Shiny application, which also includes an interactive leaflet map:

![](assets/img/Capture.PNG)

