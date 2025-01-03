# hess-reference-aisan

#https://fuma.ctglab.nl/downloadPage
# this is where I download 1000G reference panel
# then generate  hess-reference-aisan
for chr in {1..23}; do \
plink --bfile EAS --chr $chr --make-bed --out EAS_${chr}; \
done
