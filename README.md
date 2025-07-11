# Protein-Protein Interaction Network Analysis in Breast Cancer

This mini-project explores the protein-protein interaction (PPI) network of breast cancer–associated genes using STRING, Cytoscape, and functional enrichment tools like g:Profiler. The goal is to identify hub genes and understand their roles in cancer-related biological processes and pathways through GO and KEGG enrichment analysis.

## Objectives

- Retrieve breast cancer–associated genes from public databases.
- Construct a PPI network using STRING.
- Identify hub genes based on network topology.
- Perform functional enrichment analysis (GO and KEGG).

## Tools Used

- [GeneCards](https://www.genecards.org) – for gene retrieval  
- [STRING](https://string-db.org) – for PPI network construction  
- [Cytoscape](https://cytoscape.org) – for network visualization and hub identification  
- [g:Profiler](https://biit.cs.ut.ee/gprofiler/) – for GO and KEGG enrichment analysis  

## Methods

### 1. Gene Retrieval
- Collected 100 breast cancer–associated genes from GeneCards.
- Example genes include: `TP53`, `BRCA1`, `BRCA2`, `EGFR`, `ESR1`, etc.

### 2. PPI Network Construction
- Input gene list into STRING (Organism: *Homo sapiens*)
- Interaction score threshold: **0.4** (medium confidence)
- Exported network as `.png` and `.tsv` for downstream analysis

### 3. Hub Gene Identification
- Based on node centrality using Cytoscape
- Top 10 hub genes identified:  
  `TP53`, `BRCA1`, `EGFR`, `PIK3CA`, `PTEN`, `MYC`, `CDH1`, `ESR1`, `CCND1`, `MDM2`

### 4. Functional Enrichment (GO & KEGG)
- Input hub genes into g:Profiler
- Analyzed for:
  - **Biological Processes** (e.g., signal transduction, cell proliferation)
  - **KEGG Pathways** (e.g., PI3K-Akt signaling, Cell cycle, Pathways in cancer)

## Results

### 1. Top Hub Genes
- `TP53`, `BRCA1`, `EGFR`, `PIK3CA`, `PTEN`, `MYC`, `CDH1`, `ESR1`, `CCND1`, `MDM2`

### 2. GO Biological Processes
- Signal transduction  
- Cell proliferation  
- Apoptotic process  

### 3. KEGG Pathways
- PI3K-Akt signaling pathway  
- Cell cycle  
- Pathways in cancer  

## 4. Discussion

The identified hub genes are well-known drivers of breast cancer. Enrichment analysis confirmed their involvement in key oncogenic processes, reinforcing their potential as therapeutic targets or biomarkers.

## 5. Conclusion

This project demonstrates the utility of PPI network analysis in identifying key regulatory genes in breast cancer. The workflow can serve as a foundation for future in-silico or wet lab validation.

## 6. Files Included

- `breast_cancer_genes.txt` – List of 100 breast cancer–related genes  
- `string_network.png` – STRING visual output  
- `ppi_network.tsv` – Tabular network data  
- `hub_genes.txt` – Identified hub genes  
- `go_kegg_enrichment.png` – Enrichment analysis output  

## 7. References

- [STRING](https://string-db.org)  
- [g:Profiler](https://biit.cs.ut.ee/gprofiler/)  
- [GeneCards](https://www.genecards.org)  
- [Cytoscape](https://cytoscape.org)  
