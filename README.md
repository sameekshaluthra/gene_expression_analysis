# Differential Gene Expression Analysis (Simulated)

This project performs a computational simulation of differential gene expression analysis using R. It generates synthetic data to model the expression levels of specific marker genes in **Normal** versus **Cancer** tissue samples, focusing on signatures associated with the **Epithelial-Mesenchymal Transition (EMT)**.

## Project Overview

The script simulates expression values for 6 genes across 6 samples (3 Normal, 3 Cancer).
* **Down-regulated markers (Epithelial):** CDH1, EPCAM
* **Up-regulated markers (Mesenchymal):** VIM, ZEB1, SNAI1, MMP9

The analysis calculates summary statistics (Mean ± SD) and visualizes the results.

## Files

* `gene_expression.R`: The main R script containing the simulation, processing, and plotting logic.
* `gene_expression_summary_plot.png`: The output bar chart visualization.
* `gene_expression_summary_table.csv`: The calculated summary statistics.

## Prerequisites

You must have **R** installed on your system.
* **Download R:** [https://cloud.r-project.org/](https://cloud.r-project.org/)

**Note:** The script automatically checks for and installs the required R packages (`ggplot2`, `dplyr`, `reshape2`) if they are missing.

---

## How to Run

### macOS

1.  Open **Terminal**.
2.  Navigate to the folder containing the script:
    ```bash
    cd /path/to/your/folder
    ```
3.  Run the script using `Rscript`:
    ```bash
    Rscript gene_expression.R
    ```

### Linux

1.  Open your **Terminal**.
2.  Navigate to the directory:
    ```bash
    cd /path/to/your/folder
    ```
3.  Run the script:
    ```bash
    Rscript gene_expression.R
    ```
    *(Note: You may need to install `r-base` via your package manager if you haven't already).*

### Windows

#### Option A: Using Command Prompt (cmd) or PowerShell
1.  Open **Command Prompt** or **PowerShell**.
2.  Navigate to your folder:
    ```cmd
    cd C:\path\to\your\folder
    ```
3.  Run the script.
    * If R is in your system PATH, type:
        ```cmd
        Rscript gene_expression.R
        ```
    * If that command is not found, you need the full path to the executable (example below, version number may vary):
        ```cmd
        "C:\Program Files\R\R-4.x.x\bin\Rscript.exe" gene_expression.R
        ```

#### Option B: Using RStudio (Recommended for beginners)
1.  Open **RStudio**.
2.  Go to `File` > `Open File...` and select `gene_expression.R`.
3.  Click the **Source** button in the top-right corner of the script editor (or press `Ctrl+Shift+S`).

---

## Outputs

After running the script, the following files will appear in the directory:
1.  **`gene_expression_summary_table.csv`**: A spreadsheet showing the Mean Expression and Standard Deviation for each gene per condition.
2.  **`gene_expression_summary_plot.png`**: A bar chart comparing Normal vs Cancer expression with error bars.
![](./ gene_expression_summary_plot.png)
