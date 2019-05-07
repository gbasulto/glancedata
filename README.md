
<!-- README.md is generated from README.Rmd. Please edit that file -->
glancedata
==========

<!-- badges: start -->
[![Travis build status](https://travis-ci.org/gbasulto/glancedata.svg?branch=master)](https://travis-ci.org/gbasulto/glancedata) [![AppVeyor build status](https://ci.appveyor.com/api/projects/status/github/gbasulto/glancedata?branch=master&svg=true)](https://ci.appveyor.com/project/gbasulto/glancedata) [![Codecov test coverage](https://codecov.io/gh/gbasulto/glancedata/branch/master/graph/badge.svg)](https://codecov.io/gh/gbasulto/glancedata?branch=master) <!-- badges: end -->

Whenever I start working on a dataset, I need to take a glance at the data to see how the data are or it the format is the one that I am expecting. I found myself coding similar lines over and over again with each data set I put my hands on. I decided to put that lines together in an R package so I and others can use them. I called it **`glancedata`**.

There are some already cool R packages to summarize information. Two of the best, in my opinion, are `skimr` and `GGally`. In this vignette, I provide examples of the functions in `glancedata` as well as some of the functions in these two packages.

Installation
------------

You can install the released version of glancedata from [CRAN](https://CRAN.R-project.org) with:

``` r
install.packages("glancedata")
```

Functions
---------

Whenever I start working on a dataset, I need to take a glance at the data to see how the data are or it the format is the one that I am expecting. I found myself coding similar lines over and over again with each data set I put my hands on. I decided to put that lines together in an R package so I and others can use them. I called it **`glancedata`**.

There are some already cool R packages to summarize information. Two of the best, in my opinion, are `skimr` and `GGally`. In this vignette, I provide examples of the functions in `glancedata` as well as some of the functions in these two packages.

Below is a table with the functions shown in this vignette.

| Function                  | Description                                                                                                     |
|:--------------------------|:----------------------------------------------------------------------------------------------------------------|
| `glance_data`             | Alternative to `summary`. Emphasizes missing data and binary variables.                                         |
| `glance_data_in_workbook` | Similar to `glance_data`. Creates list of dataframes instead and saves XLSX file.                               |
| `plot_numerical_vars`     | Creates a plot per numerical variable. It might be histogram, density plot, qqplot, violin plot or scatterplot. |
| `plot_discrete_vars`      | Creates a plot per numerical variable. It might be histogram, density plot, qqplot, violin plot or scatterplot. |

Example
-------

This is a basic example which shows you how to solve a common problem:

``` r
library(glancedata)
#> Registered S3 methods overwritten by 'ggplot2':
#>   method         from 
#>   [.quosures     rlang
#>   c.quosures     rlang
#>   print.quosures rlang
#> Registered S3 method overwritten by 'GGally':
#>   method from   
#>   +.gg   ggplot2
## basic example code
```
