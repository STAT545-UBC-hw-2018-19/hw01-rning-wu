iris
================
ray
September 18, 2018

R Markdown
----------

This is an R Markdown document. Markdown is a simple formatting syntax for authoring HTML, PDF, and MS Word documents. For more details on using R Markdown see <http://rmarkdown.rstudio.com>.

When you click the **Knit** button a document will be generated that includes both content as well as the output of any embedded R code chunks within the document. You can embed an R code chunk like this:

This is exploring the IRIS dataset that comes built-in with R.

``` r
summary(iris)
```

    ##   Sepal.Length    Sepal.Width     Petal.Length    Petal.Width   
    ##  Min.   :4.300   Min.   :2.000   Min.   :1.000   Min.   :0.100  
    ##  1st Qu.:5.100   1st Qu.:2.800   1st Qu.:1.600   1st Qu.:0.300  
    ##  Median :5.800   Median :3.000   Median :4.350   Median :1.300  
    ##  Mean   :5.843   Mean   :3.057   Mean   :3.758   Mean   :1.199  
    ##  3rd Qu.:6.400   3rd Qu.:3.300   3rd Qu.:5.100   3rd Qu.:1.800  
    ##  Max.   :7.900   Max.   :4.400   Max.   :6.900   Max.   :2.500  
    ##        Species  
    ##  setosa    :50  
    ##  versicolor:50  
    ##  virginica :50  
    ##                 
    ##                 
    ## 

So we can see that the we have 150 observations, 50 each from 3 species, and the dimensions of sepal and petals are recorded.

Including Plots
---------------

You can also embed plots, for example:

``` r
plot(iris)
```

![](iris_files/figure-markdown_github/pressure-1.png)

Here we are looking at a two-way correlation table. As expected, petal length and with correlate highly.

Additionally, we see clustering in many of the correlation plots. This could indicate that the cluster may be one distinct species.

We could also compute various statistics manually. For example,

``` r
mean(iris$Petal.Width)
```

    ## [1] 1.199333

outputs 1.199, just like in the summary statistics.

Note that the `echo = FALSE` parameter was added to the code chunk to prevent printing of the R code that generated the plot.
