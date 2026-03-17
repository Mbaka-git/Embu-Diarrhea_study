# Embu-Diarrhea_study
Metagenomic analysis of stool samples from children with diarrhea in Embu, Kenya.


#Description
This repository contains the complete bioinformatics analysis for a metagenomic study of 5 stool samples from children under the age of five years with diarrhea in Embu, Kenya. The study aims to characterize bacterial and viral pathogens using shotgun metagenomics and Kraken2/Bracken analysis


#Samples
- EMBA-14, EMBA-25, EMBA-43, EMBA-49, EMBA-54

#Methods

1. Quality control: `fastp` for read trimming
2. Taxonomic classification: Kraken2 + Bracken (species to phylum levels)
3. Bacterial analysis: Renormalized to 100% within bacteria
4. Viral analysis: Family-to-species level tracking
5. Coinfection analysis: Multiple pathogen detection per sample
6. Alpha diversity: Shannon, Simpson, Chao1, Observed species

#Run analaysis scripts in order
#initial data processing and quality control scripts

01_initial_qc.sh - FastQC initial quality assessment
02_trimming.sh - Read trimming with fastp
03_post_trim_qc.sh - Post-trimming quality control
04_quality_comparison.sh - Compare pre/post trimming quality

#Taxonomy

01_kraken2.sh - Kraken2 classification
02_bracken_commands.sh - Bracken abundance re-estimation

#Visualization

Bar_plot_2026_Mar_10.R - 
heatmap_log_transformed Mar_11_2026.R
Alpha_diversity_11_Mar_2026.R
heatmap_log_transformed Mar_12_2026.R
virus_12_mar_2026.R
