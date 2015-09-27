---
title       : Travel Expense Computation
subtitle    : A simple data product to calculate travel expenses
author      : Koh M.H.
job         : Analyst
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Background of this presentation

This is a course project for the module on "Developing Data Products".  A shiny application on Travel Expense Computation has been created and deployed on Rstudio's servers. This presentation is a reproducible pitch presentation about the Travel Expense Computation application.

--- .class #id 

## What is the Travel Expense Computation about?

The application is to facilitate the computation of travel expense for travellers in terms of transportation fees, accomodation fees as well as miscellaneous allowance. The user can input the amounts of these components and indicate the number of travellers. The application will then base on these inputs and compute the total travel expense for each traveller as well as the total travel expense for the total number of the travellers. It illustrates the following :

* use of widget inputs such as numeric input (indicate amounts) and slider (indicate number of travellers),
* computation of travel expense related inputs
* reactive output such as total travel expense per traveller as well as for the total number of travellers
* A brief explanation on the purpose and how to make use of the application.

--- .class #id 

## How are the computation done?

Below is an illustration of how the amounts are computed, based on defaulted amounts on the left side of the screen :


```r
transport_fee <- 10; accomodation_fee <- 50; misc_allowance <- 20; Num_of_travellers <- 1
Total_Cost_per_traveller <- transport_fee + accomodation_fee + misc_allowance
Total_Cost_all_travellers <- Total_Cost_per_traveller * Num_of_travellers
```

The results for the above will then be shown on the right side of the screen :

```r
Total_Cost_per_traveller
```

```
## [1] 80
```

```r
Total_Cost_all_travellers
```

```
## [1] 80
```

--- .class #id 

## How to access this application?

The Travel Expense Computation application can be accessed [here](https://kminghui.shinyapps.io/TravelExp)

This is the end of the presentation.

Thank you.
