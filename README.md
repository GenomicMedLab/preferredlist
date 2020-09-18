# Pediatric Cancer Gene Passlist

## Introduction

This project identifies lists of genes and hotspots that flags variants for review
that would otherwise be filtered by variant calling and annotation pipeline.

Our initial target is a short list (10s of genes) from the following sources:
-  [CIViC](https://civicdb.org/home)
-  [Gröbner and Worst, et al.](https://doi.org/10.1038/nature25480)
-  [PeCAN](https://pecan.stjude.cloud/)
  
## Results
- CIViC: 5 pediatric clinically-relevant genes with generalized mutations / deletions / loss
  ([notes](analyses/CIViC/notes.md))
- Gröbner and Worst, et al.: 77 pediatric-relevant SMGs (23 are also adult SMGs)
  ([notes](analyses/Grobner_and_Worst/notes.md))
- PeCAN: Results not available or reproducible from available data
  ([notes](analyses/PeCAN/notes.md))
  
## Reproducibility

### Directory Structure
To aid in reproducibility, all data generated are stored in 
the `data/` directory. Analyses (notes) are individually
linked in this document, but also findable in the `analyses/` directory.
