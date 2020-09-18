# Pediatric Cancer Gene Passlist

## Introduction

This project identifies lists of genes and hotspots that flags variants for review
that would otherwise be filtered by variant calling and annotation pipeline.

Our initial target is a short list (10s of genes) from the following sources:
  - PeCAN ([resource](https://pecan.stjude.cloud/)) ([notes]())
  - CIViC ([resource](https://civicdb.org/home)) ([notes]())
  - Gröbner and Worst, et al. ([paper](https://doi.org/10.1038/nature25480)) ([notes]())
  
## Results
In progress!
  
## Reproducibility

### Directory Structure
To aid in reproducibility, all data and results generated are stored in 
the `data/` and `results/` directories, respectively. Analyses are individually
linked in this README, but also findable in the `analyses/` directory.

### Package Installation
To reproduce the environment for the notebooks provided in this file, you may use the 
[pipenv](https://pypi.org/project/pipenv/) environment management tool:
```shell script
pipenv sync
```