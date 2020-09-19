# Commands for combining results

Collecting overlapping genes from at Gröbner and Worst et al. and Ma et al.:

```shell script
cd ../data/
cat grobner_worst_pediatric_smgs.txt ma_smgs.txt| grep -v -e '^[[:space:]]*$' | sort | uniq -d > overlapping_genes.srt.txt
```

Merging with CIViC pediatric genes

```shell script
cat overlapping_genes.srt.txt civic_pediatric_genes.txt | sort -u > merged_genes.srt.txt
```

Removing adult cancer SMGs:

```shell script
sort kandoth_adult_smgs.txt > kandoth_adult_smgs.srt.txt
comm -23 merged_genes.srt.txt kandoth_adult_smgs.srt.txt > merged_minus_adult.srt.txt
```