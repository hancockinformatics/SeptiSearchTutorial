---
title: Test for Enriched Sepsis Gene Sets
layout: default
nav_order: 5
---

- SeptiSearch's implementation of [GSVA](https://github.com/rcastelo/GSVA) will
  examine the expression of the curated sepsis gene sets within expression data
  produced by technologies such as RNA-Seq or microarrays. Each sample within
  your dataset is assigned an enrichment score for each gene set, which can be
  positive or negative depending on the expression level of the genes in a
  given sample.
- To help demonstrate the usefulness of GSVA, we provide an example dataset
  based on microarray data from [GSE65682](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE65682),
  accessible via the "Load example data" button. Then, simply click "Submit 
  expression data for GSVA" at the bottom of the sidebar to run the analysis and
  see the results.

![Successfully loaded user data for GSVA.](../../assets/images/t7.png)

If you'd like to submit your own data for GSVA, the expression component needs
to meet the following criteria:

- Your data must in a plain text, comma-delimited (CSV) file
- The first column must contain Ensembl gene IDs
- The remaining columns should contain samples, with unique names
- Values within the matrix should be transformed/normalized, as is appropriate
  for your data/technology
	- We provide a link to information on the Variance
	Stabilized Transformation (VST) which is often suitable for RNA-Seq data, but
	other methods may also be used, e.g. if you're working with microarrary data

While you can submit only the expression data for GSVA, it's recommended to also
include metadata (e.g. sample groupings) to make the final heatmap more
informative. There are a few requirements for submitted metadata:

- Your metadata must be in a plain text, comma-delimited (CSV) file
- The first column should contain sample names, which must match the sample
  names from your expression data
	- Any missing, extra, or non-matching sample names will cause an error
- All remaining columns will be considered variables/traits (e.g. disease 
  status, severity, mortality, etc.)

Once you've uploaded either the expression data alone, or expression and
metadata, select "Submit expression data for GSVA" to run the analysis and view
the results, which include a summary table and heatmap. Explanations of all the
columns can be viewed by hovering over the column names with your cursor.

![Results from SeptiSearch's GSVA implementation.](../../assets/images/t8.png)

The full results table can be downloaded with the button at the bottom of the
sidebar, and the image can be saved by right-clicking on it and selecting "Save
Image..." from the context menu.
