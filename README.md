# MDD-VTE-TEMR-analysis
# Code for Relationship between Major Depressive Disorder and Venous Thromboembolism: A Five-Ancestry Genetic Analysis 

This repository contains the code used for the trans-ethnic Mendelian randomization (TEMR) analyses performed in our study investigating the bidirectional relationship between major depressive disorder (MDD) and venous thromboembolism (VTE) across multiple ancestries.

## Overview

The main objective of this project was to implement a multi-ancestry TEMR framework to evaluate ancestry-specific heterogeneity in the MDD–VTE relationship. The analyses were conducted using publicly available GWAS summary statistics from European (EUR), East Asian (EAS), African (AFR), Hispanic (HIS), and South Asian (SAS) populations.

The scripts provided here were developed based on the original **TEMR** method and package, with additional reorganization and simplification to facilitate more direct execution, improve workflow clarity, and enhance computational reproducibility for the present study. These scripts should therefore be viewed as a study-specific implementation built upon the original TEMR framework, rather than as a replacement for the original method.

## Original TEMR Method

The present code is based on the TEMR method described in:

**Hou L, Wu S, Yuan Z, Xue F, Li H.** TEMR: Trans-ethnic mendelian randomization method using large-scale GWAS summary datasets. *The American Journal of Human Genetics*. 2025;112(1):28-43.

Users interested in the methodological details are strongly encouraged to consult the original publication and the official TEMR package documentation.

## Repository Contents

- `forward_TEMR.R`  
  Forward-direction TEMR analysis (`MDD -> VTE`)

- `reverse_TEMR.R`  
  Reverse-direction TEMR analysis (`VTE -> MDD`)

## Software Environment

The analyses were performed in **R** and rely primarily on the following packages:

- `TEMR`
- `data.table`
- `dplyr`

Additional packages may be required depending on local environments and downstream extensions.

## Data Availability

This repository provides the analysis scripts only.

The GWAS summary statistics used in this study were obtained from publicly available sources described in the manuscript. Because some datasets are subject to access restrictions, licensing terms, or source-specific redistribution policies, the raw input summary statistics are not fully redistributed in this repository. Users should obtain the original GWAS datasets directly from the corresponding data providers.

## Notes on Implementation

To improve usability in the context of the present study, the code has been organized into a more streamlined workflow with standardized input handling, quality-control steps, and output generation. These adjustments were made solely to facilitate execution and reproducibility of the current analyses and do not alter the core methodological basis of the TEMR framework.

## Reproducibility

To reproduce the main analyses, users may run:

1. `forward_TEMR.R`
2. `reverse_TEMR.R`

Before running the scripts, please make sure that:

- all required R packages are installed;
- the input GWAS summary files are available locally;
- the file names and paths in the scripts are updated to match your working environment.

## Disclaimer

This repository is intended to support transparency and computational reproducibility of the analyses reported in our study. The code is provided for research purposes. Users should interpret and adapt the scripts in conjunction with the original TEMR publication, the official package, and the specific characteristics of their own datasets.

## Citation

If you use the TEMR method, please cite the original publication:

Hou L, Wu S, Yuan Z, Xue F, Li H. TEMR: Trans-ethnic mendelian randomization method using large-scale GWAS summary datasets. *The American Journal of Human Genetics*. 2025;112(1):28-43.
