Basic Plot
================
Chris
2025-09-14

<span style="color: red">**This is an R Markdown document!**</span>

``` r
set.seed(123)

df_demonstration =
  tibble(
    x = rnorm(n = 1000, mean = 9, sd = 5),
    y = 3 * x + 12 + runif(n = 1000, min = 2, max = 10)
  )
```

``` r
ggplot(df_demonstration, aes(x = x, y = y)) + geom_point()
```

![](template_files/figure-gfm/making_a_plot-1.png)<!-- -->

The mean is 9.0806393.
