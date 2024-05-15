## Data

- mRNA: https://zenodo.org/records/11094170/files/mRNA.csv
- miRNA: https://zenodo.org/records/11094170/files/miRNA.csv
- circRNA : https://zenodo.org/records/11094170/files/circRNA.csv
- Methylation: https://zenodo.org/records/11094170/files/Methylation.csv
- Proteomics: http://proteomecentral.proteomexchange.org/cgi/GetDataset?ID=PXD007666

## GEO Platforms

| | GEO Platform |Array name  | 
|---------------|----------------|-----------------|
|circRNA|[GPL21825](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GPL21825) | Arraystar Human CircRNA microarray V2 | 
|methylation|[GPL21145](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GPL21145) |Infinium MethylationEPIC|
|microRNA|[GPL19322](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GPL19322)|miRCURY LNA microRNA Array, 7th gen|
|mRNA|[GPL21185](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GPL21185)|Agilent-072363 SurePrint G3 Human GE v3 8x60K |

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
