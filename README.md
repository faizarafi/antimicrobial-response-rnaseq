# Differential Gene Expression Analysis of Antibiotic-Treated *E. coli*

## Overview

RNA-seq differential expression analysis investigating transcriptional responses of Escherichia coli to different antibiotic treatments.

The analysis compares untreated control samples with cultures exposed to novobiocin, rifampicin, and tetracycline, with downstream functional analysis used to identify biological pathways associated with antimicrobial stress response.

## Dataset

The analysis uses publicly available RNA-seq count data from GEO accession GSE215300.

The dataset includes:
- E. coli MG1655
- 36 samples
- 4 treatment conditions:
  - Control
  - Novobiocin
  - Rifampicin
  - Tetracycline
- 3 biological replicates per culture/library-preparation combination
- 4,464 genes

Three library-preparation strategies were represented in the dataset:
- Standard 5′ directional preparation
- VCE enrichment
- Non-enrichment

## Analysis Workflow
RNA-seq counts → normalization → exploratory analysis → differential expression → functional enrichment

### Differential Expression

Differential expression analysis was performed using DESeq2.

The workflow includes:
- Count-data normalization
- Treatment comparisons
- Identification of differentially expressed genes
- PCA to evaluate sample-level variation
- Heatmaps of expression patterns
- Visualization of differential expression results

### Functional Analysis

Differentially expressed genes were further analyzed using:
- Gene Ontology (GO) enrichment
- KEGG pathway enrichment

These analyses were used to investigate biological processes and pathways associated with antibiotic exposure.

## Tools & Technologies
| Category | Tools |
|---|---|
| Differential expression |	`DESeq2` |
| Visualization |	`ggplot2`, `pheatmap`, `EnhancedVolcano` |
| Functional analysis |	`GO enrichment`, `KEGG` |
| Language | `R` |
| Data source | `NCBI GEO` |


## Technical Skills Demonstrated
- RNA-seq count-data analysis
- Differential expression analysis
- Experimental-condition comparison
- PCA and exploratory transcriptomic analysis
- Heatmap and volcano-plot visualization
- Gene Ontology enrichment
- KEGG pathway analysis
- R-based reproducible analysis

## Repository Contents

- `dge_analysis.R`: R Markdown document containing the complete analysis workflow
- `report_ecoli_transcriptomics.pdf`: Written report documenting the analysis and results

## Data

The analysis uses publicly available data from NCBI Gene Expression Omnibus (GEO):

### GSE215300

The original sequencing data are not redistributed in this repository. The analysis is based on the publicly available processed count data associated with the study.

