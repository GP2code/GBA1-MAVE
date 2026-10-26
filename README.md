# A harmonized functional reference framework for GBA1

`GP2 ❤️ Open Science 😍`

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23654228.svg)](https://doi.org/10.5281/zenodo.23654228)

**Last updated:** September 2026

## Summary

This is the online repository for the manuscript titled **"A harmonized functional reference framework for GBA1"**. This study generated a large-scale functional atlas of *GBA1* variation using a multiplexed assay of variant effect (MAVE), providing quantitative measures of glucocerebrosidase (GCase) function across thousands of variants. These data enable systematic characterization and comparison of the functional consequences of *GBA1* variation.

Data from the Global Parkinson’s Genetics Program (GP2) were used to clinically contextualise these functional findings. Specifically, GCase functional scores were correlated with age at onset (AAO) in *GBA1* variant carriers and with variant-level Parkinson’s disease odds ratios derived from GP2 data.

This repository contains code used for the GP2-based analyses, including single-variant association analyses to estimate *GBA1* variant odds ratios, extraction of *GBA1* variant carriers and corresponding clinical data, and downstream correlation analyses. It also includes code used to generate the associated figures and visualisations. 


## Data statement
Data used in the preparation of this article were obtained from the Global Parkinson’s Genetics Program (GP2; https://gp2.org).

All GP2 data are hosted in collaboration with the Accelerating Medicines Partnership in Parkinson’s disease, and are available via application on the website (https://amp-pd.org/register-for-amp-pd). For up-to-date information on GP2 data acquisition, access, and policies, visit https://gp2.org/. Tier 1 data can be accessed by completing a form on the Accelerating Medicines Partnership in Parkinson’s Disease (AMP®-PD) website (https://amp-pd.org/register-for-amp-pd). Tier 2 data access requires approval and a Data Use Agreement signed by your institution.

In this analysis we used Tier 2 GP2 Release 12 data ([10.5281/zenodo.20932193](https://doi.org/10.5281/zenodo.20932193))


### Helpful Links

- [GP2 Website](https://gp2.org/)
  - [GP2 Cohort Dashboard](https://gp2.org/cohort-dashboard-advanced/)
- [Introduction to GP2](https://movementdisorders.onlinelibrary.wiley.com/doi/10.1002/mds.28494)
  - [Other GP2 Manuscripts (PubMed)](https://pubmed.ncbi.nlm.nih.gov/?term=%22global+parkinson%27s+genetics+program%22)

## Repository Orientation
- The `analysis/` directory includes all analyses discussed in the manuscript.

<pre> THIS_REPO/ 
  ├── analyses/ 
  |     ├── 00_GP2_R12_WGS_GBA1_MAVE_assoc.ipynb
  |     ├── 01_GP2_R12_WGS_GBA1_MAVE_carrier.ipynb
  |     └── 02_GP2_R12_WGS_GBA1_MAVE_plots.ipynb
  ├── LICENSE
  └── README.md 
</pre>

## Analysis Notebooks
### Languages: Python, bash, and R
| Directory | Notebooks   | Description | 
|-----------|----------------|--------|
|`analyses/`| `00_GP2_R12_WGS_GBA1_MAVE_assoc.ipynb`         | Association tests for each variant of interest. |
|`analyses/`| `01_GP2_R12_WGS_GBA1_MAVE_carrier.ipynb`         | Extract variant carriers and perform annotation using GP2 WGS data. |
|`analyses/`| `02_GP2_R12_WGS_GBA1_MAVE_plots.ipynb`         | Correlation plots. |

## Software
| **Software** | **Version(s)** | **Resource URL** | **RRID** | **Notes** |
|--------------|----------------|------------------|----------|-----------|
|ANNOVAR|d.06.08.2020|http://www.openbioinformatics.org/annovar/|RRID:SCR_012821|Used for variant annotation.|
|PLINK|v. 2.0|http://www.nitrc.org/projects/plink|RRID:SCR_001757|Used for genetic analyses.|
|Python Programming Language|3.9, 3.10|http://www.python.org/|RRID:SCR_008394|pandas; numpy; matplotlib; Used for general data wrangling/plotting/analyses|
