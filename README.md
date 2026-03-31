# GWAS VCF Processing Pipeline

## Overview
An end-to-end bioinformatics pipeline demonstrating VCF file processing
using industry-standard tools — bcftools, tabix, and Python.

## Pipeline Steps
1. VCF generation (100 SNPs, VCF 4.2 format)
2. bgzip compression
3. tabix indexing
4. bcftools QC stats
5. Variant filtering (PASS + AF > 0.05)
6. DataFrame parsing & visualization

## Results
- 100 variants processed across Chr1
- 87 PASS variants | 13 LowQual filtered
- 94 common variants (AF > 5%)
- Mean read depth: 51.3x | Mean mapping quality: 46.5

## Visualizations
| Plot | Description |
|---|---|
| plot1 | Allele frequency distribution & PASS vs LowQual |
| plot2 | Quality score, read depth, mapping quality distributions |
| plot3 | Manhattan-style position plot (AF + quality) |
| plot4 | SNP substitution patterns & Ti/Tv ratio |

## Tech Stack
- bcftools 1.19
- tabix (htslib) 1.19
- Python 3.13
- pandas, NumPy, matplotlib, seaborn

## Author
Taimoor Asad — Python & Bioinformatics Developer
