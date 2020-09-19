# Gröbner and Worst, et al. Analysis Notes

[The landscape of genomic alterations across childhood cancers](https://doi.org/10.1038/nature25480)
(Gröbner and Worst et al., _Nature_, 2018) examines commonalities and differences of genomic variants
across multiple pediatric cancer types.

## Pediatric pan-cancer SMGs
[Supplementary tables](../../data/41586_2018_BFnature25480_MOESM3_ESM.xlsx) from the paper 
were downloaded.
Supplementary Table 9 contains 77 significantly mutated genes as identified by MuSiC.
These were extracted as a [standalone list](../../data/grober_worst_pediatric_smgs.txt).

Of these, "25" genes were identified in the manuscript as overlapping with adult SMGs. While some of
this list was provided as labels in Extended Data Figure 5c, inspection of this list revealed only 23 
genes. To verify if this list was complete, the [adult SMG list](../../data/kandoth_adult_smgs.txt) 
was extracted from [Table S4](../../data/Supplementary_Table_4.xlsx) of the
[2013 TCGA pan-cancer study](https://doi.org/10.1038/nature12634) and 23 overlapping gene symbols were
identified.

The [overlapping list of 23 genes](../../data/overlapping_smgs.txt) precisely matched the 23 genes 
listed in Figure 5c.
