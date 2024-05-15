| Discipline        | Target Information                                 | Resources                                                      |
|-------------------|----------------------------------------------------|----------------------------------------------------------------|
| **Genomics**      | **DNA variation data & chromatin structure**       | **ClinVar**<br>**NCBI**<br>**DisGeNET**<br>**OMIM**<br>**TCGA** |
|                   | - WGS and WES                                      |                                                                |
|                   | - Multiple variation types (e.g., SNVs, CHVs, CNVs)|                                                                |
| **Transcriptomics**| **Gene expression**                                | **GEO**<br>**Expression atlas**<br>**GTEx**<br>**GtrNAdb**<br>**miRbase** |
|                   | - RNA-seq & scRNA-seq                              |                                                                |
|                   | - Multiple RNA functionalities:                    |                                                                |
|                   |   - mRNA, miRNA, siRNA, rRNA, tRNA                 |                                                                |
| **Proteomics**    | **Protein dynamics**                               | **UniProt**<br>**HPA**<br>**BioGRID**<br>**IID**<br>**PDB**<br>**AlphaFold** |
|                   | - Mass spectrometry & Protein microarrays          |                                                                |
|                   | - Protein-Protein interaction (PPI)                |                                                                |
|                   | - Structure                                        |                                                                |
|                   | - Cell-specificity & functionality                 |                                                                |
| **Metabolomics**  | **Metabolite dynamics & chemical reactions**       | **KEGG**<br>**Reactome**<br>**VMH**                             |
|                   | - Mass spectrometry                                |                                                                |
|                   | - Metabolite fluxes and levels in cells and tissues|                                                                |
| **Epigenomics**   | **Chemical modifications modulating DNA activity** | **ENCODE**<br>**GTEx**<br>**GEO**                               |
|                   | - ncRNAs                                           |                                                                |
|                   | - DNA methylation and acetylation                  |                                                                |
|                   | - Chromatin accessibility                          |                                                                |
| **Metagenomics**  | **Organisms inhabiting human ecological niches**   | **Human Microbiome Project**<br>**microbioTA**                 |
|                   | - Involvement in normal human physiology (e.g., immune cell maturation) |                                       |
|                   | - Multiple niches (e.g., Oral, gut, skin)          |                                                                |


```mermaid
graph LR
    A[Experimental manipulations] --> B[Gene]
    C[Other sources of biological variability we know about] --> B[Gene]
    D[Biological variability of unknown source] --> B[Gene]
    E[Technical variability of unknown source] --> B[Gene]
    F[Sources of technical variability we know about] --> B[Gene]

    B[Gene] -->|Actual Expression| G[RNA]
    
    H[Sources of technical variability we know about] --> G[RNA]
    I[Technical variability of unknown source] --> G[RNA]
    
    G[RNA] --> J[Measured gene expression]
    
    style A fill:#b3d9ff,stroke:#000000,stroke-width:2px
    style C fill:#b3d9ff,stroke:#000000,stroke-width:2px
    style D fill:#b3ffb3,stroke:#000000,stroke-width:2px
    style E fill:#b3ffb3,stroke:#000000,stroke-width:2px
    style F fill:#b3d9ff,stroke:#000000,stroke-width:2px
    
    style H fill:#b3d9ff,stroke:#000000,stroke-width:2px
    style I fill:#b3ffb3,stroke:#000000,stroke-width:2px
    
    style B fill:#ff9999,stroke:#000000,stroke-width:2px
    style G fill:#ffcc99,stroke:#000000,stroke-width:2px
    style J fill:#ff9999,stroke:#000000,stroke-width:2px
``` 
