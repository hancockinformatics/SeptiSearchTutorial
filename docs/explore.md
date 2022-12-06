---
title: Explore the Database
layout: default
nav_order: 2
---

This tab allows you to easily browse and search the database, organized by Gene
Set Name

- The first field in the sidebar allows you to enter search terms to filter the
  entries based on the title of study. For example, you could enter
  "endotypes" to look at publications which focus on characterizing sepsis
  endotypes
- With the second field you can filter the gene sets based on the inclusion of 
  COVID patients  
- You may search in the database for specific molecules. This function is
  case-insensitive, and will return partial matches (e.g. "s100" would return 
  gene sets which contain "S100A9", "S100A12", etc.)  
- After entering a number of searches or filter criteria, if you would like to
  return to the original table, click the "Reset this page" button at the
  bottom of the sidebar, which will reset all inputs. In some cases it may also
  help to refresh the page from your browser (CTRL+F5)  

![Select a study from the table to display all associated molecules.](../../assets/images/t2.png)

- The table on the right will display all matching gene sets based on the
  specified filters - initially it includes all studies curated by SeptiSearch.
  Clicking on one or more rows will bring up a second table listing all entries
  (molecules) for the selected gene sets.
- You can search this second table using the small search box above it on the
  right
- If you select a single gene set in the top table, a button is enabled which
  will send that gene set to the "Perform Pathway Enrichment" tab, allowing you
  to easily test a gene set of interest for enriched pathways (see
  [this section](#perform-pathway-enrichment) for more details on performing
  pathway enrichment in SeptiSearch)

![Choosing a single gene set enables the "Test this gene set for enriched pathways" button](../../assets/images/t3.png)

- When you have selected one or more rows from the top table, you can use the
  provided button to download the lower table as a tab-delimited file
