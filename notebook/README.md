# NFL Player Value Analysis – Jupyter Notebook

This notebook is the main script for my BAIS:3250 Data Wrangling final project. It analyzes NFL player salary and performance data from the 2022 to 2024 seasons to evaluate player value. The notebook includes web scraping, data cleaning, merging, normalization, metric creation, visual analysis, hypothesis testing, and machine learning modeling.

## Notebook Sections

### 1. Data Collection (Web Scraping)
Scrapes salary data from OverTheCap and performance stats from Pro Football Reference using BeautifulSoup and pandas.

### 2. Data Cleaning and Merging
Combines the salary and stat datasets by player and year, removes duplicates, handles missing values, and formats columns for analysis.

### 3. Feature Engineering
Creates normalized stats and engineered value metrics such as:
- `Stat_Total`: Yards + (TDs × 20)
- `Value_Index`: Normalized performance – Normalized salary
- `Normalized_Yards_per_Million`: Performance per salary unit

### 4. Value Analysis and Visualization
Includes visualizations showing top and bottom players by Value Index, average value by position, and normalized performance vs. salary.

### 5. Hypothesis Testing
Uses a Welch’s t-test to compare Value Index between QBs and RBs, finding a statistically significant difference.

### 6. Machine Learning
Trains Linear, Ridge, and Lasso regression models to predict salary based on performance. Models are evaluated using R² and MAE, with results showing performance explains about 22% of salary variation.

## How to Run

To run this notebook:
1. Open `Project_DW2025_AidanTerrill.ipynb` in Jupyter or VS Code.
2. Run each cell in order from top to bottom.
3. Make sure the following Python libraries are installed:
   - pandas
   - numpy
   - matplotlib
   - seaborn
   - scikit-learn
   - BeautifulSoup4
   - requests

## Notes

This notebook supports the full analysis presented in the final project report and uses only public web-scraped data. All analysis is reproducible using the notebook and data provided in this repository.
