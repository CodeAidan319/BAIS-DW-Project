## Data Dictionary

The table below explains the columns included in the final dataset (`NFL_Combined_2022_2024.xls`). It contains salary and performance data for NFL quarterbacks, running backs, and wide receivers from 2022 to 2024. The dataset also includes engineered metrics like Stat_Total and Value_Index, which are used to compare player value across positions and seasons.

| Column                     | Type     | Source                  | Description                                                  |
|----------------------------|----------|--------------------------|--------------------------------------------------------------|
| Player                    | Text     | Both                     | Full name of the player                                      |
| Year                      | Numeric  | Both                     | NFL season year (2022, 2023, or 2024)                        |
| Team                      | Text     | Pro Football Reference   | Team abbreviation (e.g., KC, BUF)                            |
| Position                  | Text     | Both                     | Player position (QB, RB, or WR)                              |
| Salary                    | Numeric  | OverTheCap               | Annual salary in USD                                         |
| Passing_Yards             | Numeric  | Pro Football Reference   | Total passing yards (QBs only)                               |
| Pass_TDs                  | Numeric  | Pro Football Reference   | Total passing touchdowns (QBs only)                          |
| Completion_Pct            | Numeric  | Pro Football Reference   | Pass completion percentage (QBs only)                        |
| Rush_Yards                | Numeric  | Pro Football Reference   | Total rushing yards (RBs only)                               |
| Rush_TDs                  | Numeric  | Pro Football Reference   | Total rushing touchdowns (RBs only)                          |
| Yards_per_Carry           | Numeric  | Pro Football Reference   | Average yards per carry (RBs only)                           |
| Receiving_Yards           | Numeric  | Pro Football Reference   | Total receiving yards (WRs only)                             |
| Receiving_TDs             | Numeric  | Pro Football Reference   | Total receiving touchdowns (WRs only)                        |
| Yards_per_Catch           | Numeric  | Pro Football Reference   | Average yards per reception (WRs only)                       |
| Stat_Total                | Numeric  | Calculated               | Total production = yards + (TDs × 20)                        |
| Normalized_Stat           | Numeric  | Calculated               | Min-max scaled Stat_Total                                    |
| Normalized_Salary         | Numeric  | Calculated               | Min-max scaled Salary                                        |
| Value_Index               | Numeric  | Calculated               | Normalized_Stat – Normalized_Salary                          |
| Normalized_Yards_per_Million | Numeric  | Calculated               | Normalized_Stat / Normalized_Salary                          |
| Player_Year               | Text     | Calculated               | Player name with year (e.g., “Joe Burrow (2023)”)           |
| Position_RB               | Binary   | Calculated               | 1 if player is RB; 0 otherwise (used in ML)                  |
| Position_WR               | Binary   | Calculated               | 1 if player is WR; 0 otherwise (used in ML)                  |
