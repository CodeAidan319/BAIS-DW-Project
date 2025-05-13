### `/data/`
The file `NFL_Combined_2022_2024.xls` contains the final cleaned and merged dataset used in this project. Each row represents a single NFL player-season from the years 2022 through 2024. 

The dataset includes:
- Player names, teams, positions, and year
- Salary data scraped from OverTheCap
- Performance statistics from Pro Football Reference (passing, rushing, and receiving)
- Custom engineered metrics such as:
  - `Stat_Total`: a weighted performance score combining yards and touchdowns
  - `Normalized_Stat` and `Normalized_Salary`: min-max scaled values for comparison
  - `Value_Index`: difference between performance and salary on a normalized scale
  - `Normalized_Yards_per_Million`: a ratio indicating production per unit of salary

This dataset serves as the foundation for all analysis, visualizations, and machine learning models in the notebook and report.
