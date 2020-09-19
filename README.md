# Pediatric Cancer Gene Passlist

## Introduction

This project identifies lists of genes and hotspots that flags variants for review
that would otherwise be filtered by variant calling and annotation pipeline.

Our initial target was a short list of pediatric cancer driver genes from the following sources:
-  [CIViC](https://civicdb.org/home)
-  [Gröbner and Worst, et al.](https://doi.org/10.1038/nature25480)
-  [PeCAN](https://pecan.stjude.cloud/)
  
## Results
- CIViC ([notes](analyses/CIViC/notes.md)): 5 pediatric clinically-relevant genes with 
  generalized mutations / deletions / loss.
- Gröbner and Worst, et al. ([notes](analyses/Grobner_and_Worst_2018/notes.md)): 
  77 pediatric-relevant SMGs (23 are also adult SMGs).
- PeCAN ([notes](analyses/PeCAN/notes.md)): summarized SMGs / hotspots not available or reproducible 
  from available data. However, several published studies from major datasets used by PeCAN are listed on 
  their site:
  - [Gröbner and Worst, et al.](https://doi.org/10.1038/nature25480) (already evaluated)
  - [Ma, et al.](https://doi.org/10.1038/nature25795)
  - [Rusch, et al.](https://doi.org/10.1038/s41467-018-06485-7)
  As a first pass, then, we can collect SMG lists from these publications in lieu of recomputing and 
  calling our own.
- Ma, et al. ([notes](analyses/Ma_2018/notes.md)): 
  
## Reproducibility

### Directory Structure
To aid in reproducibility, all data generated are stored in 
the `data/` directory. Analyses (notes) are individually
linked in this document, but also findable in the `analyses/` directory.
