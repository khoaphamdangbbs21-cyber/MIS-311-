# MIS-311-
Cost of Living Analysis
# Cost of Living Analysis | MIS 311

## Data Overview

This project analyzes the *Cost of Living* dataset provided for MIS 311. The original dataset contains 201 observations and five variables covering 2000–2023.

| Variable | Description |
|---|---|
| `Country` | Country associated with the observation |
| `Year` | Year of the observation |
| `Average_Monthly_Income` | Reported average monthly income |
| `Cost_of_Living` | Reported cost of living |
| `Region` | Geographic region |

The analysis compares reported living costs across regions and examines the relationship between monthly income and living costs.

## Data Cleaning

| Issue | Action |
|---|---|
| Two missing `Region` values | Both records were for Mexico. The missing values were filled with `North America`, consistent with the other Mexico records. |
| Two missing `Average_Monthly_Income` values | The cells were left blank. These records were included in the cost-of-living analysis and excluded from calculations that required income. |
| Two exact duplicate rows | Duplicates were identified by comparing all five columns and removed, leaving 199 records. |

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

![Horizontal bar chart comparing average cost of living across six regions](cost-by-region.png)

| Region | Observations | Average Cost of Living |
|---|---:|---:|
| Africa | 18 | 3,963.17 |
| Oceania | 22 | 3,913.40 |
| North America | 51 | 3,750.07 |
| Asia | 47 | 3,645.29 |
| South America | 16 | 3,585.02 |
| Europe | 45 | 3,554.35 |

### Average Monthly Income vs. Cost of Living

![Scatter plot with average monthly income on the horizontal axis and cost of living on the vertical axis](income-vs-cost.png)

The Pearson correlation was **r = −0.0263**, based on the **197 observations** with both income and cost-of-living values.

## Key Insights

1. **Average living costs varied across regions in the dataset.** Africa had the highest reported average (3,963.17), while Europe had the lowest (3,554.35), a difference of 408.82. Since these averages cover multiple years and are based on different numbers of observations, businesses can use them to identify where to check more recent, country-level cost data before setting budgets.

2. **Monthly income showed little linear relationship with living costs.** The Pearson correlation was −0.0263 across 197 complete observations, indicating that higher reported income did not consistently go with higher or lower living costs in this sample. Businesses comparing potential markets should examine local incomes and living costs together when assessing customer purchasing power.

## Files

[Download the Excel analysis](Cost-of-Living-Analysis.xlsx)

## References

*Cost of living* [Data set]. (n.d.). MIS 311 – Introduction to Business Analytics course materials.
