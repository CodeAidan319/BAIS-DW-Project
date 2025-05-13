# NFL Player Value Analysis (2022–2024)
### BAIS:3250 – Data Wrangling Final Project  
**Author:** Aidan Terrill

## Project Overview

This project analyzes the relationship between NFL player salaries and on-field performance from 2022 to 2024. NFL teams operate under a salary cap, which makes it important to identify players who deliver high value relative to their compensation. The goal is to measure cost-efficiency by comparing player stats to salary data and determining whether certain positions (e.g., RBs, QBs, WRs) are under- or over-valued.

To do this, I scraped salary data from OverTheCap and performance stats from Pro Football Reference. I merged the two datasets, engineered new performance and value metrics, and used a combination of descriptive visualizations, hypothesis testing, and regression modeling to interpret trends.

## Project Goals

- Evaluate whether player salary is aligned with on-field performance.
- Identify the most underpaid and overpaid NFL players using custom metrics.
- Compare average value by position (QB, RB, WR).
- Use machine learning to predict salary based on performance statistics.
- Apply statistical testing to compare positional value across the league.

## Repository Structure

NFL-Player-Value/
│
├── data/
│   ├── salary_data_2022_2024.csv             # Scraped salary data from OverTheCap  
│   ├── performance_data_2022_2024.csv        # Scraped performance data from Pro Football Reference  
│   └── merged_df_final.csv                   # Final cleaned and merged dataset used in the analysis  
│
├── notebooks/
│   └── Final_NFL_Value_Analysis.ipynb        # Jupyter notebook with scraping, cleaning, analysis, and modeling  
│
├── reports/
│   └── Project_Report_Final.docx             # Final report outlining goals, results, and conclusions  
│
├── docs/
│   └── data_dictionary_final.md              # Full data dictionary describing each field in merged_df  
│
└── README.md                                 # This file

## Repository Walkthrough

### `/data/`
Contains the raw and cleaned data used for analysis. The `merged_df_final.csv` file includes combined salary and performance data for QBs, RBs, and WRs from 2022–2024, along with normalized metrics and calculated value scores.

### `/notebooks/`
This folder includes the Jupyter notebook with all Python code. It contains:
- Web scraping with BeautifulSoup and pandas
- Data cleaning and merging
- Feature engineering (Stat_Total, Value_Index, etc.)
- Visualizations and hypothesis testing
- Machine learning models: Linear, Ridge, and Lasso regression

### `/reports/`
Contains the final written report submitted for the course. The report outlines project goals, methods, key findings, visualizations, and conclusions.

### `/docs/`
Includes the data dictionary used in the report. Each column in the final dataset is clearly defined and labeled with type, source, and description.

### `/README.md/`
The main overview file for the project. Describes the structure of the repository, research goals, and how to run the code.

## How to Run

To run the analysis:
1. Open `Final_NFL_Value_Analysis.ipynb` using Jupyter Notebook or VS Code.
2. Run each cell in order.
3. Ensure the following Python libraries are installed:
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
