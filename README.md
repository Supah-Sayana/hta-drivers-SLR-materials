# hta-drivers-SLR-materials

Supplementary Materials — HTA Decision-Drivers Systematic Review
Using Large Language Models to Enhance Systematic Reviews Concerning HTA Decision Drivers

This repository contains every dataset, notebook and methods file needed to reproduce the results in our manuscript.

Repository URL
https://github.com/Supah-Sayana/hta-drivers-SLR-materials

Folder structure

data_and_analysis/

final_extraction_and_synthesis.xlsx

parameters_extracted_python_graphs.xlsx

screening_decisions_performance.xlsx

R-Jupyter CI Graphs.ipynb


methods/

pico_search_strategy_results.docx

llm_prompting_framework.docx


data_and_analysis holds the Excel data files and the R-based Jupyter notebook that regenerates all figures and statistics.
methods holds two Word documents: the PICO search strategy with results and the GPT-4 multi-persona prompt framework used in title-and-abstract screening.

How to reproduce the analysis

Requirements

R ≥ 4.2 with Jupyter + IRkernel or RStudio

R packages: tidyverse, readxl, ggplot2, IRdisplay, here


Steps

1. Clone or download the repo
git clone https://github.com/Supah-Sayana/hta-drivers-SLR-materials.git
cd hta-drivers-SLR-materials


2. Open data_and_analysis/R-Jupyter CI Graphs.ipynb in Jupyter (or RStudio) and run all cells.
The notebook reads the Excel files in the same folder and recreates every plot and summary table.


3. Example of loading a sheet with the here package in R

library(here)
library(readxl)
df <- read_excel(here("data_and_analysis", "final_extraction_and_synthesis.xlsx"))


4. For full search transparency consult the Word files in methods/.



License

Data and documents: CC-BY 4.0
Notebook code: MIT License

Citation

Takatzoglou N, Ken R, Cindy T, Mikhail S, Maureen B (2025).
Supplementary materials for “Using Large Language Models to Enhance Systematic Reviews Concerning HTA Decision Drivers.”
GitHub. https://github.com/Supah-Sayana/hta-drivers-SLR-materials
