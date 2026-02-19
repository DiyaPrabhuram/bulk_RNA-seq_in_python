# Bulk RNA-seq Analysis in Python
This repository contains all the basic information one needs to conduct bulk RNA-seq analysis in python.

# Basic Differential Expression Analysis
Differential expression analysis is a technique used to idenitfy genes with significant expression profile differences between two or more samples. ( https://pydeseq2.readthedocs.io/en/stable/auto_examples/plot_minimal_pydeseq2_pipeline.html )

# Gene Set Enrichment Analysis (GSEA)
GSEA is a computational method that determines whether an a priori defined set of genes shows statistically significant, concordant differences between two biological states (e.g. phenotypes). ( https://www.gsea-msigdb.org/gsea/index.jsp )

## AMD Dataset (GEO)

Raw counts for differential expression analysis: https://www.ncbi.nlm.nih.gov/geo/download/?type=rnaseq_counts&acc=GSE115828&format=file&file=GSE115828_raw_counts_GRCh38.p13_NCBI.tsv.gz

Gene annotation table: https://www.ncbi.nlm.nih.gov/geo/download/?format=file&type=rnaseq_counts&file=Human.GRCh38.p13.annot.tsv.gz

IMPORTANT NOTES:
Upon discussing with a leading researcher in the field of transcriptomics research, it has been pointed out that there is some controversy surrounding the DESeq2 implemented in R versus the one in python. I think it comes down to the fact that the results across the two implementations are inconsistent. Refer to this discussion thread for more information - https://github.com/TCP-Lab/gene_ranker/issues/6
Most importantly, when the sample size of your dataset is greater than 8, it is recommended that you skip the DESeq2 (or EdgeR) algorithm and run limma-voom or the wilcoxon rank sum test instead. Refer to this article for more information - https://towardsdatascience.com/deseq2-and-edger-should-no-longer-be-the-default-choice-for-large-sample-differential-gene-8fdf008deae9/
