Lecture-02d Notebook
================
Christopher Prener, Ph.D.
(September 06, 2018)

## Introduction

This notebook contains sample code for Lecture-02d - Structuring
Notebooks.

## Dependencies

This notebook requires two packages - `ggplot2` and `dplyr`.

``` r
# tidyverse packages
library(dplyr)       # cleaning data
```

    ## 
    ## Attaching package: 'dplyr'

    ## The following objects are masked from 'package:stats':
    ## 
    ##     filter, lag

    ## The following objects are masked from 'package:base':
    ## 
    ##     intersect, setdiff, setequal, union

``` r
library(ggplot2)     # plotting data
```

## Load Data

For this set of examples, we’ll take the `mpg` data from the `ggplot2`
package and assign it to a new object to work with:

``` r
autoData <- mpg
```

For the rest of the code, we’ll reference `autoData` as a starting
point.

## Part 1

Part 1 of the assignment involves cleaning data from the mpg data frame.

### Question 1

The first question asks to explore the structure of the `autoData`
    data:

``` r
str(autoData)
```

    ## Classes 'tbl_df', 'tbl' and 'data.frame':    234 obs. of  11 variables:
    ##  $ manufacturer: chr  "audi" "audi" "audi" "audi" ...
    ##  $ model       : chr  "a4" "a4" "a4" "a4" ...
    ##  $ displ       : num  1.8 1.8 2 2 2.8 2.8 3.1 1.8 1.8 2 ...
    ##  $ year        : int  1999 1999 2008 2008 1999 1999 2008 1999 1999 2008 ...
    ##  $ cyl         : int  4 4 4 4 6 6 6 4 4 4 ...
    ##  $ trans       : chr  "auto(l5)" "manual(m5)" "manual(m6)" "auto(av)" ...
    ##  $ drv         : chr  "f" "f" "f" "f" ...
    ##  $ cty         : int  18 21 20 21 16 18 18 18 16 20 ...
    ##  $ hwy         : int  29 29 31 30 26 26 27 26 25 28 ...
    ##  $ fl          : chr  "p" "p" "p" "p" ...
    ##  $ class       : chr  "compact" "compact" "compact" "compact" ...
