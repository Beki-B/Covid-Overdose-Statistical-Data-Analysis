# Choose Your Own Hypothesis Project: U.S. Drug Overdose Deaths

## Project Overview

| Element | Description |
|---------|-------------|
| **Project Title** | COVID-19 and U.S. Drug Overdose Mortality Trends |
| **Research Question** | Did the rate of drug overdose deaths in the United States increase significantly after the start of COVID-19 (March 2020) compared to before COVID? |
| **Significance** | Overdose mortality surged during the pandemic, and understanding this change helps explain public-health challenges influenced by lockdowns, mental-health stress, and drug supply disruptions. |
| **Hypothesis (H1)** | The average monthly overdose mortality rate of overdose deaths were higher after COVID-19 than before COVID-19. |
| **Null Hypothesis (H0)** | There is **no difference** in the average monthly mortality rate before vs. after COVID-19. |
| **Primary Outcome Metrics** | 1. **Mean overdose deaths per month** (before vs. after COVID)<br>  |
| **Unit of Analysis** | One month of U.S. overdose mortality data |
| **Data Source** | CDC NCHS Monthly Provisional Overdose Death Counts (`VSRR_Provisional_Drug_Overdose_Death_Counts.csv`) ***Dataset URL:** https://www.cdc.gov/nchs/nvss/vsrr/drug-overdose-data.htm |
| **Time Period** | 2015–2025 (monthly data) |
| **Why This Data Works** | - Monthly overdose deaths are ideal for comparing pre- and post-COVID trends<br>- National coverage ensures consistency<br>- Monthly frequency allows testing mean changes<br>- Sufficient temporal coverage (2015–2025)|
| **Statistical Methods** | - **Bootstrap confidence intervals** for the difference in mean overdose deaths per month (after – before)<br>- **Permutation test** to determine if observed differences could occur by chance |
| **Null Hypothesis Interpretation** | "COVID-19 had no real effect on overdose mortality—the difference we see before and after COVID is just random chance." |

## Project Structure
- **Data Cleaning**: Filtered national overdose death indicators, converted data values to numeric format, handled missing values, and created monthly date features.
- **Exploratory Analysis**: Visualized monthly overdose deaths over time, identified pre- and post-COVID periods, and examined overall level changes.
- **Statistical Testing**: Comparison of means  using bootstrap and permutation methods and Used bootstrap resampling to estimate uncertainty in mean permutation testing to assess statistical significance of the mean change.
- **Results**: Evaluated whether overdose death levels  changed significantly after the start of COVID-19.

## Key Findings

-   Monthly overdose deaths increased sharply after March 2020, indicating a clear level shift following COVID-19.
-   The bootstrap confidence interval for the difference in mean monthly overdose deaths (After − Before) lies entirely above zero, providing strong evidence of a statistically significant increase.
-   The permutation test produced a p-value effectively equal to 0.0000, indicating that the observed increase in overdose deaths is highly unlikely to be due to random chance.
-   Overall, the evidence supports an upward shift in overdose mortality levels.



## Conclusion

-   COVID-19 caused a major jump in overdose deaths rather than a change driven by random fluctuation. After the pandemic began, the average number of overdose deaths per month increased sharply, and this increase is strongly supported by statistical evidence. However, COVID-19 did not permanently increase the month-to-month growth rate of overdose deaths; instead, deaths rose quickly and then remained elevated, later flattening or declining.Overall, the pandemic significantly worsened the overdose crisis through a one-time structural shock, and the analysis highlights the value of statistical methods in distinguishing between changes in level.


## Repository Contents
- `CYOH.ipynb`: Main analysis notebook
- `README.md`: Project documentation (this file)
- Data analysis outputs and visualizations

## Tools & Technologies
- Python (pandas, numpy, matplotlib, seaborn)
- Jupyter Notebook
- Statistical methods: Bootstrap resampling, permutation testing

