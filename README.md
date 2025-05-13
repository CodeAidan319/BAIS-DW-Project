# NFL Player Value Analysis (2022–2024)
### BAIS:3250 – Data Wrangling Final Project  
**Author:** Aidan Terrill

## Project Overview

This project explores whether NFL players are paid fairly based on their performance. It focuses on quarterbacks (QBs), running backs (RBs), and wide receivers (WRs) during the 2022 to 2024 seasons. I scraped salary data from OverTheCap and performance stats from Pro Football Reference, merged and cleaned the datasets, and created metrics to measure player value.

The project includes feature engineering, descriptive visualizations, a statistical comparison of positions, and regression models to test whether performance can help predict salary. The results highlight which players and positions are delivering the most value for their compensation.

## Project Goals

- Compare salary and performance across player positions.
- Build a cleaned, merged dataset using web-scraped data.
- Create metrics like `Stat_Total` and `Value_Index` to measure value.
- Use Welch’s t-test to compare average value between positions.
- Apply linear, ridge, and lasso regression to predict salary from performance.

## Repository Structure
NFL-Player-Value/
│
├── data/
│ └── NFL_Combined_2022_2024.xls # Final dataset with salary, stats, and value metrics
│
├── notebooks/
│ └── Project_DW2025_AidanTerrill.ipynb # Full notebook with scraping, cleaning, analysis, and ML
│
├── reports/
│ └── Project_Report_aterrill.docx # Final report summarizing the project
│
├── docs/
│ └── data_dictionary.md # Definitions of all dataset fields
│
└── README.md # This file


## Repository Walkthrough

### `/data/`
This folder includes `NFL_Combined_2022_2024.xls`, a cleaned dataset containing salary and performance data for QBs, RBs, and WRs from 2022–2024. It also includes normalized columns and custom value metrics used for analysis.

### `/notebooks/`
Contains the full Jupyter notebook used to run the project. It walks through scraping, cleaning, feature engineering (e.g., `Stat_Total`, `Value_Index`), visualization, hypothesis testing, and machine learning (Linear, Ridge, Lasso).

### `/reports/`
Includes the final written report submitted for BAIS:3250. The report covers the project's goals, key methods, insights from the data, and interpretations of results.

### `/docs/`
Contains the data dictionary describing each column in the final dataset. Useful for understanding how the raw and engineered data fields were defined and used.

## How to Run

1. Open `Project_DW2025_AidanTerrill.ipynb` in Jupyter or VS Code.
2. Run the notebook cells from top to bottom.
3. Make sure these libraries are installed:
   - pandas
   - numpy
   - matplotlib
   - seaborn
   - scikit-learn
   - BeautifulSoup4
   - requests

## Data Sources

- [Pro Football Reference](https://www.pro-football-reference.com/)
- [OverTheCap](https://overthecap.com/)
