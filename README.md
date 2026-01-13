# Camouflaged Object Detection (COD) Bibliometric & Science‑Mapping Study (2015–2025)

This repository contains the dataset and outputs used in a bibliometric and science‑mapping analysis of **Camouflaged Object Detection (COD)** research. It includes the curated bibliographic corpus (BibTeX) for all analyzed studies and the figures/images used in the manuscript (publication growth, source dynamics, influence, collaboration, and thematic maps).

## Contents

- **BibTeX corpus**: all analyzed COD records (merged and cleaned)
- **Figures / images**: plots and network visualizations used in the paper
- **Tables / exports**: summary tables and network export files (if included)
- **Optional scripts**: analysis and preprocessing scripts (if included)

## Recommended repository structure

If your folder names differ, adjust this section to match your actual layout.

```
.
├── data/
│   ├── bibtex/
│   │   ├── cod_scopus.bib
│   │   ├── cod_wos.bib
│   │   └── cod_merged_cleaned.bib
│   ├── metadata/
│   │   ├── search_strings.md
│   │   ├── inclusion_exclusion.md
│   │   └── prisma_counts.csv
│   └── exports/
│       ├── bibliometrix_export.csv
│       └── vosviewer_export.txt
├── figures/
│   ├── fig01_workflow.png
│   ├── fig02_document_types.png
│   ├── fig03_publication_growth.png
│   ├── fig04_most_relevant_sources.png
│   ├── fig05_source_dynamics.png
│   ├── fig06_top_authors.png
│   ├── fig07_author_production_over_time.png
│   ├── fig08_country_collaboration.png
│   ├── fig09_trending_topics.png
│   ├── fig10_keyword_cooccurrence.png
│   └── fig11_thematic_map.png
├── results/
│   ├── tables/
│   │   ├── table_sources_local_impact.csv
│   │   ├── table_most_cited_documents.csv
│   │   ├── table_productive_countries.csv
│   │   └── table_top_sources.csv
│   └── networks/
│       ├── coauthorship_network.*
│       ├── citation_network.*
│       └── keyword_network.*
├── scripts/ (optional)
│   ├── bibliometrix_analysis.R
│   └── preprocessing_cleaning.R
├── LICENSE
└── README.md
```

## Data sources and scope

- **Databases**: Scopus and Web of Science Core Collection  
- **Time window**: January 2015 to December 2025  
- **Unit of analysis**: peer‑reviewed COD studies using AI techniques (journals and conferences)

## Search strategy and screening

- The search strategy combines COD terms (e.g., “Camouflaged Object Detection”, “Camouflage Object Detection”, “COD”) with common computer‑vision and deep‑learning keywords (e.g., segmentation, CNN, Transformer, boundary/edge‑aware, feature fusion, weak supervision, video/temporal, RGB‑D).
- Screening follows predefined **inclusion** and **exclusion** criteria documented in the metadata files (if provided in this repository).

## How to reproduce the analysis (optional)

If you include scripts/notebooks, this section provides a standard pathway for reproducibility.

### A) Bibliometrix (R)

1. Install R and RStudio (recommended).
2. Install packages:

```r
install.packages(c("bibliometrix", "dplyr", "ggplot2", "readr"))
```

3. Update paths in `scripts/bibliometrix_analysis.R` to point to your merged BibTeX file (e.g., `data/bibtex/cod_merged_cleaned.bib`).
4. Run the script to regenerate performance indicators and descriptive statistics.

### B) VOSviewer

1. Open VOSviewer.
2. Import the relevant export file from `data/exports/`.
3. Generate networks (co‑authorship, citations, keyword co‑occurrence).
4. Export figures and network files into `figures/` and `results/networks/`.

## Outputs

This repository supports:
- Publication growth and source production dynamics
- Core venue identification (most relevant sources)
- Local impact and influence summaries (e.g., citations, h‑index–style indicators)
- Most‑cited documents
- Country collaboration networks
- Trending topics, keyword co‑occurrence, and thematic mapping

## Citation

If you reuse the dataset, figures, or derived outputs, please cite the associated paper (add the final bibliographic details once published).

## License (Open Access)

Open Access This article is licensed under a Creative Commons Attri￾bution 4.0 International License, which permits use, sharing, adapta￾tion, distribution and reproduction in any medium or format, as long 
as you give appropriate credit to the original author(s) and the source, 
provide a link to the Creative Commons licence, and indicate if changes 
were made. The images or other third party material in this article are 
included in the article's Creative Commons licence, unless indicated 
otherwise in a credit line to the material. If material is not included in 
the article's Creative Commons licence and your intended use is not 
permitted by statutory regulation or exceeds the permitted use, you will need to obtain permission directly from the copyright holder. To view a 
copy of this licence, visit http://creativecommons.org/licenses/by/4.0/.

## Contact

**Authors**
- Aminu Bashir Suleiman¹  
- Ahmad Tijjani Garba²  
- Ahmed Ibrahim Mahmud³  

**Affiliations**
1. Department of Cyber Security, Federal University Dutsin‑Ma, Katsina, Nigeria  
2. Department of Information Technology, Bayero University, Kano, Nigeria  
3. Department of Software Engineering, Federal University Dutsin‑Ma, Katsina, Nigeria  

**Email**
- ¹ ameenu.basheer10@gmail.com  
- ² atgarba.it@buk.edu.ng  
- ³ amidot2005@gmail.com
