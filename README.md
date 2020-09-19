# Pediatric Cancer Gene Passlist

## Introduction
This project identifies a list of recurrently mutated and clinically-relevant genes for inspecting variants
that would otherwise be filtered by our variant calling and annotation pipeline.

Our initial target was a short list of _pediatric cancer_ genes from the following sources:
-  [CIViC](https://civicdb.org/home)
-  [Gröbner and Worst et al.](https://doi.org/10.1038/nature25480)
-  [PeCAN](https://pecan.stjude.cloud/)
  
## Results
- CIViC ([notes](analyses/CIViC/notes.md)): [5 pediatric clinically-relevant genes](data/civic_pediatric_genes.txt)
  with generalized mutations / deletions / loss.
- Gröbner and Worst, et al. ([notes](analyses/Grobner_and_Worst_2018/notes.md)): 
  [77 pediatric cancer-relevant SMGs](data/grobner_worst_pediatric_smgs.txt) 
  ([23 are also adult SMGs](data/grobner_worst_overlapping_smgs.txt)).
- PeCAN ([notes](analyses/PeCAN/notes.md)): summarized SMGs / hotspots not available or reproducible 
  from provided downloads. However, several published studies from major datasets used by PeCAN are listed on 
  their site:
  - [Gröbner and Worst et al.](https://doi.org/10.1038/nature25480) (already evaluated)
  - [Ma et al.](https://doi.org/10.1038/nature25795)
  - [Rusch et al.](https://doi.org/10.1038/s41467-018-06485-7)
  
  As a first pass, then, we can collect gene lists from these datasets at the time of publication in lieu of 
  recomputing and calling our own.
- Ma, et al. ([notes](analyses/Ma_2018/notes.md)): With some added filtering, 138 pediatric cancer SMGs.
- Rusch et al. ([notes](analyses/Rusch_2018/notes.md)): No SMG / hotspot analysis reported.

After initial evaluation, this leaves us with three sources of genes. Refining the SMGs  to those that appear
in both landscape studies and then merging CIViC genes with this list gives us an initial list of 
[40 genes](data/merged_genes.srt.txt). 
Of these, [20 are not reported](data/merged_minus_adult.srt.txt) as adult SMGs in the 
[Kandoth et al.](https://doi.org/10.1038/nature12634) evaluation of TCGA adult cancers.
([notes](analyses/combining_results.md))

## Reproducibility

### Directory Structure
To aid in reproducibility, all data generated are stored in 
the `data/` directory. Analyses (notes) are individually
linked in this document, but also findable in the `analyses/` directory.
