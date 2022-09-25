---
title: Homework 09/27
author: Tyler J. Anderson
output: github_document
---

# Heading 1

## Subheading


```r
# Some R code
library(dplyr)
```

```
## 
## Attaching package: 'dplyr'
```

```
## The following objects are masked from 'package:stats':
## 
##     filter, lag
```

```
## The following objects are masked from 'package:base':
## 
##     intersect, setdiff, setequal, union
```

```r
library(nycflights13)

flights %>% group_by(carrier) %>%
    summarize(mean_delay = mean(arr_delay, na.rm = T))
```

```
## # A tibble: 16 × 2
##    carrier mean_delay
##    <chr>        <dbl>
##  1 9E           7.38 
##  2 AA           0.364
##  3 AS          -9.93 
##  4 B6           9.46 
##  5 DL           1.64 
##  6 EV          15.8  
##  7 F9          21.9  
##  8 FL          20.1  
##  9 HA          -6.92 
## 10 MQ          10.8  
## 11 OO          11.9  
## 12 UA           3.56 
## 13 US           2.13 
## 14 VX           1.76 
## 15 WN           9.65 
## 16 YV          15.6
```

# Heading 2

Some information.
