# TCGA Biolinks Data Processing

This repository contains R scripts for downloading, processing, and analyzing TCGA (The Cancer Genome Atlas) data using the TCGAbiolinks package.

## Overview

The main script `run_tcga_biolinks.Rmd` performs the following tasks:

1. Downloads RNA-seq data for a specific TCGA project (default: TCGA-BRCA)
2. Processes and prepares the data
3. Extracts gene expression data (FPKM-UQ, raw counts, and TPM)
4. Retrieves and processes clinical data
5. Filters and processes the RNA-seq data
6. Outputs various CSV files with processed data

## Requirements

- R (version 4.0.0 or higher recommended)
- RStudio (for running the .Rmd file)

### Required R packages:

- BiocManager
- TCGAbiolinks
- dplyr
- tidyr
- styler
- data.table
- stringr
- SummarizedExperiment

## Usage

1. Open the `run_tcga_biolinks.Rmd` file in RStudio.
2. Install the required packages if not already installed.
3. Run the script chunks sequentially.
4. The script will download data, process it, and create several output CSV files.

## Output Files

The script generates several CSV files:

- `gene_id_hgnc_id_mapping.csv`: Mapping between gene IDs and HGNC IDs
- `all_fpkm_uq_data_with_clinical.csv`: FPKM-UQ data with clinical information
- `all_raw_counts_data_with_clinical.csv`: Raw counts data with clinical information
- `all_tpm_data_with_clinical.csv`: TPM data with clinical information
- `feature_data.csv`: Feature data for genes
- `sample_data.csv`: Sample data with clinical information
- `metadata.csv`: Metadata information
- `treatment_data.csv`: Treatment-related data
- Filtered RNA-seq data files for different sample types and data types

## Customization

To analyze a different TCGA project, modify the `project_name` variable in the script.

## License

None

## Contact

Devaki Kelkar 
devaki.kelkar@outlook.com