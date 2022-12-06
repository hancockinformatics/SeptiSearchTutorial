---
title: Peform Pathway Enrichment
layout: default
nav_order: 4
---

SeptiSearch includes the ability to upload a list of your own genes (e.g. those
identified as differentially expressed in an RNA-Seq experiment) and test them
for enriched Reactome pathways using
[ReactomePA](https://bioconductor.org/packages/ReactomePA), as well as MSigDB's
Hallmark gene sets and GO terms via
[enrichR](https://cran.r-project.org/package=enrichR). This functionality is
designed to complement the use of GSVA (the next tab), which tests your data for
the dysregulation of the curated sepsis gene sets.

- You have a few options for submitting data here:
    - Use the "Load example data" button to load a preselected list of genes
    - You can paste your own list of genes as a single column, with one gene per
      line. Submitted genes IDs can be Ensembl, Entrez, or HGNC names.
    - From the Explore the Database (ADD LINK) tab, select a
      single gene set in the top table, then use the "Test this gene set for
      enriched pathways" button to send the genes to the Enrichment tab
- Next, the "1. Perform gene ID mapping" button will be enabled, which will
  complete any necessary mapping steps prior to enrichment testing
- Once the ID mapping is completed, you can hit the "2. Submit genes for pathway
  enrichment" button to run the tests.
- Your results will be displayed in two tables; one containing Reactome pathways
  identified by ReactomePA, and the second containing GO terms and MSigDB
  Hallmark gene sets found by enrichR; use the buttons to switch between the
  two. Hover your cursor over the column names to see a description of each.
  Both tables can be downloaded using the buttons at the bottom of the
  sidebar.

![Table of enrichment results, from ReactomePA.](../../assets/images/t6.png)  
