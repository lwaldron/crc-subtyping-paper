Analysis repository for datasets included in the [CRC subtyping paper](https://www.ncbi.nlm.nih.gov/pubmed/30253799).

* `src/`: analysis scripts, ordered in sequence by the tasks performed. The `manuscript/` and `response_letter/` subdirectories contain scripts used to generate display items for the manuscript and response letters.
* `data/`: most importantly, the [*ExpressionSets*](https://www.bioconductor.org/packages/devel/bioc/vignettes/Biobase/inst/doc/ExpressionSetIntroduction.pdf) for each dataset (gene expression + metadata) used in the analyses, as well as the necessary data for analyzing the [CMS](https://www.ncbi.nlm.nih.gov/pubmed/26457759) and [CRIS](https://www.ncbi.nlm.nih.gov/pubmed/28561063) subtypes.

# Frequently (at least once) asked questions:

> How/where can I get the contents for results/discrete_evaluation/additional/?

These are generated CRIS (28561063) classification results for GSE59857, an external validation set. Scripts generating these files are in “4.5-additional_sets.R”, and the output is also provided in this file from issue [#1](https://github.com/biobakery/crc-subtyping-paper/issues/1), [additional.zip](https://github.com/biobakery/crc-subtyping-paper/files/5688429/additional.zip).

> What is the different between Supplementary Table 1 and `data/loadings/avg_loadings.csv`?

They should be exactly the same; supplementary table 1 is just average loadings used to assign continuous scores.
