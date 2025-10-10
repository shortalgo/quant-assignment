# AlgoDepartment Quantitative Research Assignment

Welcome to the **AlgoDepartment Quantitative Research Assignment**.  
This repository contains the materials and structure for candidates to complete their take-home evaluation.

---

## Overview

This assignment is designed to assess your ability to analyze option data, perform quantitative research, and present your findings clearly using Python and Jupyter.

You are provided with:
- A Jupyter notebook (`newberry_quant_assignment.ipynb`) containing all instructions and code scaffolding.  
- Historical NIFTY option and spot data (split into parts for size limits).  
- Example CSV files showing expected output formats.

All task-specific details are given **inside the notebook** — please read it carefully before starting.

---

## 📂 Repository Contents

| File / Folder | Description |
|----------------|-------------|
| `newberry_quant_assignment.ipynb` | Main assignment notebook |
| `SamplePerformanceStats.csv` | Example of performance metrics output |
| `SampleTradeReport.csv` | Example of trade report output |
| `NIFTY_option_data_split.zip` / `.z01` | Split archives of option data (to be merged) |
| `NIFTY_spot_data.zip` | Spot data archive |

---

## Data Setup

Because the full dataset exceeds GitHub’s file-size limit, the **option data** has been split into smaller parts.  
Follow the steps below to combine and extract the data.

---

### Step 1 — Combine Split Files

Ensure that both files are in the same folder:

NIFTY_option_data_split.zip
NIFTY_option_data_split.z01


####  On Linux / macOS


zip -F NIFTY_option_data_split.zip --out NIFTY_option_data_full.zip
unzip NIFTY_option_data_full.zip 

 On Windows (using 7-Zip or WinRAR)

Keep both parts (.zip and .z01) in the same folder.
Right-click on NIFTY_option_data_split.zip → Extract Here.
The tool will automatically merge and extract the full dataset.

### Step 2 — Extract Spot Data

If NIFTY_spot_data.zip is provided separately (or via external link), extract it similarly:

unzip NIFTY_spot_data.zip

After extraction, your folder should look like this:

quant-assignment/
├── newberry_quant_assignment.ipynb
├── NIFTY_option_data/
├── NIFTY_spot_data/
├── SamplePerformanceStats.csv
└── SampleTradeReport.csv

How to Complete the Assignment
### Step 1 — Fork This Repository

Click the Fork button at the top right to create your own copy.
### Step 2 — Clone Your Fork

git clone https://github.com/<your-username>/quant-assignment.git
cd quant-assignment

### Step 3 — Prepare Data

Follow the instructions above to merge and extract the NIFTY data into this same directory.
### Step 4 — Work on the Notebook

Open newberry_quant_assignment.ipynb in Jupyter Notebook, JupyterLab, or VS Code and complete all tasks.
### Step 5 — Save and Commit Your Work

git add .
git commit -m "Completed quant assignment"
git push

### Step 6 — Submit

Either:

    Share the link to your forked repository, or

    Create a Pull Request to the main repo
    → AlgoDepartment/quant-assignment
