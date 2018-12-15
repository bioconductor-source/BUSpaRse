[![Travis build status](https://travis-ci.com/BUStools/BUSpaRse.svg?branch=master)](https://travis-ci.com/BUStools/BUSpaRse)

# BUSpaRse

This package processes files of the `bus` format generated from raw sequencing data, e.g. using [kallisto](http://pachterlab.github.io/kallisto/). The `bus` format is a table with 4 columns: **B**arbode, **U**MI, **S**et, and counts, that represent scRNA-seq datasets. The main goal of this package is to convert the `bus` format into a sparse matrix that can be used for downstream analysis, such as with `Seurat` and `SingleCellExperiment`. See [this paper](https://www.biorxiv.org/content/early/2018/11/21/472571) for more information about the `bus` format.

## Installation

You can install BUSpaRse with:

``` r
if (!require(devtools)) install.packages("devtools")
devtools::install_github("BUStools/BUSpaRse")
```

This is work in progress. I'm trying to get this package to Bioconductor.

## Example
See [the vignettes](https://bustools.github.io/BUS_notebooks_R/index.html) for examples of using `BUSpaRse`. The vignettes will walk you through the complete workflow going from downloading the fastq files to the sparse matrix, with 10x v2 (10x v3, Drop-seq, inDrops, and CEL-seq2 coming soon) datasets. 
