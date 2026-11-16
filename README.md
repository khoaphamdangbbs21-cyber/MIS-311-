# MIS-311-
Cost of Living Analysis
# Cost of Living Analysis | MIS 311

## Data Overview

This project analyzes the *Cost of Living* dataset provided for MIS 311. The original dataset contains 201 observations and five variables covering 2000–2023. The analysis compares reported living costs across regions and examines their relationship with average monthly income.

| Variable | Description |
|---|---|
| `Country` | Country associated with the observation |
| `Year` | Year of the observation |
| `Average_Monthly_Income` | Reported average monthly income |
| `Cost_of_Living` | Reported cost of living |
| `Region` | Geographic region |

## Data Cleaning

| Issue | Action |
|---|---|
| Two missing `Region` values | Both records were for Mexico. The missing values were filled with `North America` based on the other Mexico records. |
| Two missing `Average_Monthly_Income` values | The cells were left blank. These rows were included in the cost-of-living analysis and excluded from calculations that required income. |
| Two exact duplicate rows | All five columns were compared to identify exact duplicates. Removing two duplicate rows left 199 records. |

## Descriptive Statistics

| Statistic | Average Monthly Income | Cost of Living |
|---|---:|---:|
| Count | 197 | 199 |
| Mean | 4,243.97 | 3,705.13 |
| Median | 4,266.46 | 3,688.09 |
| Minimum | 534.74 | 464.49 |
| Maximum | 7,976.56 | 6,981.02 |

## Visualizations

### Average Cost of Living by Region

![Average cost of living by region](Average%20Cost%20of%20Living%20by%20Region.png)

| Region | Observations | Average Cost of Living |
|---|---:|---:|
| Africa | 18 | 3,963.17 |
| Oceania | 22 | 3,913.40 |
| North America | 51 | 3,750.07 |
| Asia | 47 | 3,645.29 |
| South America | 16 | 3,585.02 |
| Europe | 45 | 3,554.35 |

### Average Monthly Income vs. Cost of Living

![Monthly income vs. cost of living](./Monthly%20Income%20Cost%20of%20Living.png)

The scatter plot uses 197 observations with both income and cost-of-living values. The Pearson correlation coefficient is **r = −0.0263**.

## Key Insights

1. **Africa had the highest average cost of living in the dataset.** Its average was 3,963.17, which was 408.82 higher than Europe's average of 3,554.35, the lowest among the six regions. Because the regional averages combine observations from multiple years, businesses can use the comparison to identify where to check more recent, country-level costs before setting budgets.

2. **Average monthly income and cost of living showed little linear association.** The Pearson correlation was −0.0263 across 197 observations, so income alone provided little information about how living costs varied in this sample. Businesses comparing markets can examine both measures when assessing local purchasing power.

## Files

[Open the Excel analysis](./Cost%20of%20Living%20Analysis.xlsx)

## References

*Cost of living* [Data set]. (n.d.). MIS 311 – Introduction to Business Analytics course materials.
