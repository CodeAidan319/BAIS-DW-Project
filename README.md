# BAIS-DW-Project
# NFL Salary vs Performance: Data Wrangling Project (BAIS:3250)

## Project Overview

This project analyzes the relationship between NFL player salaries and on-field performance metrics. NFL teams operate under a strict salary cap, making it critical to evaluate whether highly paid players are actually delivering high performance, and whether there are undervalued players contributing significant value.

We aim to combine traditional performance statistics (e.g., touchdowns, yards, sacks) with expert-based grades (Pro Football Focus) to explore cost-efficiency in player compensation. This analysis will help uncover trends in salary allocation, identify potential overpaid/underpaid players, and compare value across player positions.

## Project Goals

- Determine if salary correlates with performance in the NFL.
- Identify which players provide the best and worst return on investment.
- Analyze salary-performance balance by position (e.g., QB, RB, WR).
- Build a merged dataset from multiple sources for comprehensive analysis.

## Repository Structure
BAIS3250-NFL-Project/
│
├── data/
│ └── NFL_2024_Salary_Performance.xlsx # Merged dataset with salary, and stats
│
├── notebooks/
│ └── Project_DW2025.ipynb # Jupyter notebook with all scraping, cleaning, and analysis steps
│
├── docs/
│ └── data_dictionary_final.md # Definitions and descriptions of all fields in the dataset
│
├── README.md # Main project overview and structure (this file)

## Repository Walkthrough

### `/data/`
This folder contains the main dataset: `NFL_2024_Salary_Performance.xlsx`. It includes player salary information, and performance statistics (e.g., passing yards, touchdowns) for the 2024 NFL season. Each row represents an individual player-season.

### `/notebooks/`
The `Project_DW2025.ipynb` notebook contains all the code used for web scraping, cleaning, merging, and analyzing the data. It serves as the main script for the entire project.

### `/docs/`
Includes the `data_dictionary.md` file, which defines and explains each column in the final dataset.

### `README.md`
This file provides an overview of the project, the folder structure, research goals, and relevant data sources.
