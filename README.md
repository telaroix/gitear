
<!-- README.md is generated from README.Rmd. Please edit that file -->

# gitear <a href="url"><img src="gitear.png" align="right" width="30%"></a>

<!-- badges: start -->

[![CRAN
status](https://www.r-pkg.org/badges/version/gitear)](https://cran.r-project.org/package=gitear)
<!-- badges: end -->

The goal of gitear is to request your self-hosted Git service data and
import it to R in a tidy data frame.

`gitear` is a package that communicates with the
[gitea](https://gitea.io/en-us/) API.

## Installation

You can install the development version from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("ixpantia/gitear")
```

## Usage

First go to your gitea self hosted service and grab your API Token. Then
you should be able to the following:

``` r
library(gitear)

## Credentials
api_token <- "gfdsgfd8ba18a866bsdfgsdfgs3a2dc9303453b0c92dcfb19"
url_ixpantia <- "https://secure.ixpantia.com"

## Example function use:
issues <- get_issues(base_url = url_ixpantia,
                       api_key = api_token,
                       owner = "ixpantia",
                       repo = "ixmandash")
```
