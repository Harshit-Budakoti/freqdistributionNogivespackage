
<!-- README.md is generated from README.Rmd. Please edit that file -->

# freqdistributionNogives

<!-- badges: start -->
<!-- badges: end -->

The goal of freqdistributionNogives is to automate the process of
GROUPED FREQUENCY DISTRIBUTION data-framing and cumulative frequency
graph.

## Installation

You can install the development version of freqdistributionNogives like
so:

``` r
# FILL THIS IN! HOW CAN PEOPLE INSTALL YOUR DEV PACKAGE?
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(freqdistributionNogives)
lowerlimits=c(0,5,10,15,20,25)
upperlimits=c(5,10,15,20,25,30)
frequencies=c(124,153,454,234,531,91)
basicfreqdist(lowerlimits,upperlimits,frequencies)
#>   LL UL classmark freq morecf lesscf
#> 1  0  5       2.5  124   1587    124
#> 2  5 10       7.5  153   1463    277
#> 3 10 15      12.5  454   1310    731
#> 4 15 20      17.5  234    856    965
#> 5 20 25      22.5  531    622   1496
#> 6 25 30      27.5   91     91   1587
```

<img src="man/figures/README-example-1.png" width="100%" />

    #> [1] "CLASS WIDTH= 5"
    ## basic example code

\`\`\`

You’ll still need to render `README.Rmd` regularly, to keep `README.md`
up-to-date. `devtools::build_readme()` is handy for this. You could also
use GitHub Actions to re-render `README.Rmd` every time you push. An
example workflow can be found here:
<https://github.com/r-lib/actions/tree/v1/examples>.

You can also embed plots, for example:

<img src="man/figures/README-pressure-1.png" width="100%" />

In that case, don’t forget to commit and push the resulting figure
files, so they display on GitHub and CRAN.
