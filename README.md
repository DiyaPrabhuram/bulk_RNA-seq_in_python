# Bulk RNA-seq Analysis in Python
This repository contains all the basic information one needs to conduct bulk RNA-seq analysis in python.

# Basic Differential Expression Analysis
Differential expression analysis is a technique used to idenitfy genes with significant expression profile differences between two or more samples. ( https://pydeseq2.readthedocs.io/en/stable/auto_examples/plot_minimal_pydeseq2_pipeline.html )

# Gene Set Enrichment Analysis (GSEA)
GSEA is a computational method that determines whether an a priori defined set of genes shows statistically significant, concordant differences between two biological states (e.g. phenotypes). ( https://www.gsea-msigdb.org/gsea/index.jsp )

## AMD Dataset (GEO)

Raw counts for differential expression analysis: https://www.ncbi.nlm.nih.gov/geo/download/?type=rnaseq_counts&acc=GSE115828&format=file&file=GSE115828_raw_counts_GRCh38.p13_NCBI.tsv.gz

Gene annotation table: https://www.ncbi.nlm.nih.gov/geo/download/?format=file&type=rnaseq_counts&file=Human.GRCh38.p13.annot.tsv.gz

NOTE: The PyDeseq2_DE_tutorial.ipynb tutorial file is a nice, general example on how to run a basic RNA-seq analysis in python (credits - sanbomics youtube channel). The RNA_seq_with_pyDESeq2.ipynb tutorial file is specific to the AMD dataset.
