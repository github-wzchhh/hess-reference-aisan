# hess-reference-aisan

Download the 1000 Genomes reference panel from [this link](https://fuma.ctglab.nl/downloadPage).

Then, generate `hess-reference-aisan` with the following script:

```bash
for chr in {1..23}; do \
plink --bfile EAS --chr $chr --make-bed --out EAS_${chr}; \
done
