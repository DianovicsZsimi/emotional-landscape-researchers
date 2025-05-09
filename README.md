
<!-- README.md is generated from README.Rmd. Please edit that file -->

# Researcher burnout and QRP

<!-- badges: start -->
<!-- badges: end -->

## Folder structure

The `data/raw` folder contains all the datafiles that are needed to
reproduce the results of the project.

The `analysis/` folder contains all the analyses files in quarto
documents.

The `analysis/figures/` folder contains all the figures

## How to Reproduce the Analysis Using `{renv}`

1.  Install R and RStudio (optional):

- [Download R](https://cran.r-project.org/bin/windows/base/)
- [Download RStudio](https://posit.co/download/rstudio-desktop/) (if
  preferred)

2.  Install {renv} (if not already installed):

``` r
install.packages("renv")
```

3.  Clone or Download This Project:

- Clone via Git:

<!-- -->

    git clone https://github.com/DianovicsZsimi/Researcher-burnout-and-QRP.git

- Or download the ZIP file and extract it.

4.  Restore the Project Environment: Open the project in R (or RStudio)
    and run:

``` r
renv::restore()
```

This command will:

- Install the exact versions of all packages listed in `renv.lock`.
- Ensure compatibility with the tested environment.
- Installing the `renv` environment takes about 10 minutes on an average
  computer with Windows 11 64bit.

(If you are using Windows, `renv::restore()` will not work without
RTools. You need RTools to compile some packages. You can install it by
running: )

``` r
install.packages("installr")
installr::install.Rtools()
```

5.  Run the analysis. Execute the scripts in this order:

I. raw_to_clean_data.qmd II. clean_to_processed_data.qmd III.
processed_to_aggregated_data.qmd IV. descriptive_analysis.qmd
