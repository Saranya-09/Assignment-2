# Assignment 2: Transcript Half-Life Calculation for Yeast Genes

Author
Saranya Guvvala

# Date
[03-01-2024]

# Programming Language & Version
Python 3.8

# Dependencies
pandas
NumPy
SciPy

# Input
DecayTimecourse.txt: Contains the 60-minute time series data for yeast genes, including three sets of time series data for each transcript.

# Script Description:
This Python script is designed to analyze 60-minute time series data of yeast gene transcripts to calculate their half-lives. It employs a meticulous process to handle the data, computing the half-lives for each transcript across three replicates. The script utilizes the curve_fit function from the scipy.optimize module to perform exponential curve fitting, a crucial step in deriving accurate half-life values. Additionally, it identifies genes with significantly high (top 10%) and low (bottom 10%) half-lives, providing insights into the dynamics of gene expression regulation.

# Output Files:
Half_Lives_Calculated.csv: Contains the computed half-lives for each yeast gene transcript.
high_half_life_genes.txt: Lists the identifiers of genes with high half-lives (top 10%).
low_half_life_genes.txt: Lists the identifiers of genes with low half-lives (bottom 10%).

# Further Analysis:
After identifying genes with high and low half-lives, I perform a functional enrichment analysis using online tools such as g:Profiler to explore the biological significance of these genes in yeast. Once the analysis is completed, the following PNG files are generated:

Detailed result of low half-life genes.png: Provides a comprehensive visualization of genes with low half-lives (bottom 10%).

Detailed result of high half-life genes.png: Offers a detailed visualization of genes with high half-lives (top 10%).

Overview of low half-life genes.png: Presents an overview visualization of genes with low half-lives (bottom 10%).

Overview of high half-life genes.png: Offers an overview visualization of genes with high half-lives (top 10%).
