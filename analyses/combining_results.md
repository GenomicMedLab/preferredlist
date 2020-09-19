# Commands for combining results

Collecting overlapping genes from at least 2 of CIViC, Gröbner and Worst et al., and Ma et al.:

```shell script
cd ../data/
cat civic_pediatric_genes.txt grobner_worst_pediatric_smgs.txt ma_smgs.txt| grep -v -e '^[[:space:]]*$' | sort | uniq -d > overlapping_genes.txt
```

Removing adult cancer SMGs:

```shell script
sort overlapping_genes.txt > overlapping_genes.srt.txt
sort kandoth_adult_smgs.txt > kandoth_adult_smgs.srt.txt
comm -23 overlapping_genes.srt.txt kandoth_adult_smgs.srt.txt > overlapping_minus_adult.srt.txt
```