
<!-- README.md is generated from README.Rmd. Please edit that file -->

# hagis

[![Project Status: Active – The project has reached a stable, usable
state and is being actively
developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
[![Travis Build
Status](https://travis-ci.org/openplantpathology/hagis.svg?branch=master)](https://travis-ci.org/openplantpathology/hagis)
[![Appveyor Build
Status](https://ci.appveyor.com/api/projects/status/qhkacm5n9twor80c/branch/master?svg=true)](https://ci.appveyor.com/project/adamhsparks/hagis/branch/master)
[![codecov](https://codecov.io/gh/openplantpathology/hagis/branch/master/graph/badge.svg)](https://codecov.io/gh/openplantpathology/hagis)
[![DOI](https://zenodo.org/badge/164751172.svg)](https://zenodo.org/badge/latestdoi/164751172)

## Introduction

The goal of *hagis* is to provide analysis tools for plant pathogens
with gene-for-gene interactions in the R programming language that the
original [Habgood-Gilmour Spreadsheet,
HaGiS](https://onlinelibrary.wiley.com/doi/full/10.1046/j.1365-3059.1999.00325.x),
(Herrmann, Löwer and Schachtel) provided.

## Overview

`hagis` was initially created for *Phytophthora sojae* surveys by Austin
McCoy and Zachary Noel at Michigan State University in the US where the
disease has been managed primarily via deployment of resistance genes
(*Rps* genes, resistance to *P. sojae*) in commercial soybean cultivars
and by the application of fungicide seed treatments. However, repeated
use of resistance genes can cause populations to adapt over time
rendering these resistance genes ineffective. To determine current
effectiveness of resistance genes for managing *P. sojae*, state-wide
surveys (in the US) are conducted to determine the pathotype (previously
referred to as “race”) structure within sampled population of *P.
sojae*.

However, the package is not only useful for *P. sojae* work. It was
built to be useful for other plant pathogen gene-for-gene interaction
systems, *e.g.* rusts or canola blackleg, *Leptosphaeria maculans*. The
goal of this package is to provide all the necessary analyses needed
when conducting a pathotype surveys, including: distribution of
susceptibilities (effective and non-effective resistance genes),
distribution of pathotype complexities with statistics, pathotype
frequency distribution, as well as diversity indices for pathotypes in
an efficient and reproducible manner.

New users are encouraged to visit the documentation,
<https://openplantpathology.github.io/hagis/articles/hagis.html>, for
detailed information on how to use *hagis* along with working examples
using a built-in data set.

## Quick Start Install

### Stable Version

A stable version of *hagis* is available from CRAN.

``` r
install.packages("hagis")
```

### Development Version

A development version is available from from GitHub. If you wish to
install the development version that may have new features or bug fixes
before the CRAN version does (but also may not work properly), please
install the remotes package, available from CRAN. We strive to keep the
master branch on GitHub functional and working properly.

``` r
if (!require("remotes")) {
  install.packages("remotes", repos = "http://cran.rstudio.com/")
  library("remotes")
}

install_github("openplantpathology/hagis", build_vignettes = TRUE)
```

## Meta

### Citation

When you use *hagis*, please cite by using:

``` r
citation("hagis")
#> 
#> McCoy AG, Noel Z, Sparks AH, Chilvers M (2019). _hagis: Analysis
#> of Plant Pathogen Pathotype Complexities, Distributions and
#> Diversity_. doi: 10.5281/zenodo.2619820 (URL:
#> https://doi.org/10.5281/zenodo.2619820), R package version 2.0.0,
#> <URL: https://openplantpathology.github.io/hagis/>.
#> 
#> A BibTeX entry for LaTeX users is
#> 
#>   @Manual{,
#>     title = {{hagis}: Analysis of Plant Pathogen Pathotype Complexities, Distributions and Diversity},
#>     author = {Austin G. McCoy and Zachary Noel and Adam H. Sparks and Martin Chilvers},
#>     year = {2019},
#>     note = {R package version 2.0.0},
#>     url = {https://openplantpathology.github.io/hagis/},
#>     doi = {10.5281/zenodo.2619820},
#>   }
```

Please note that the *hagis* project is released with a [Contributor
Code of
Conduct](https://github.com/openplantpathology/hagis/blob/master/CODE_OF_CONDUCT.md).
By contributing to this project, you agree to abide by its terms.

## References

> Herrmann, , Löwer, and Schachtel, (1999), A new tool for entry and
> analysis of virulence data for plant pathogens. Plant Pathology, 48:
> 154-158. DOI:
> [10.1046/j.1365-3059.1999.00325.x](https://doi.org/10.1046/j.1365-3059.1999.00325.x)
