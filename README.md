<!-- README.md is generated from README.Rmd. Please edit that file -->
words2number: Convert English number words into numeric digits [![Build Status](https://travis-ci.org/benmarwick/words2number.svg?branch=master)](https://travis-ci.org/benmarwick/words2number)
================================================================================================================================================================================================

### Installation

``` r
devtools::install_github("benmarwick/words2number")
```

This is a fork of [verajosemanuel/ESmisc](https://github.com/verajosemanuel/ESmisc), which is for Spanish numbers. I've just changed the Spanish to English.

### How to use

The onlny function in this package, `to_number`, is a simple function to translate English words for whole number quantities into their numerical counterparts. Given a numerical quantity spelled in English, `to_number` translates it to integer.

``` r
library(words2number)
to_number("forty two")
```

    ## [1] 42

``` r
to_number("forty-two")
```

    ## [1] 42

``` r
to_number("fortytwo")
```

    ## [1] 42

### Usage notes

-   magrittr must be installed.
-   `to_number` needs clean text. The input must be previously cleaned with extraneous words and symbols removed.
-   Quantities must be written in simple, common English (this function is very simple).
-   The upper limit is up to the millions range.

### Contributing

Please note that this project is released with a [Contributor Code of Conduct](CODE_OF_CONDUCT.md). By participating in this project you agree to abide by its terms.
