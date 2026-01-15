# sa-inflation-price-shock-analysis

# South Africa Inflation vs Global Inflation Shocks (1970–2022)

## Project Overview

This project analyzes how South Africa’s inflation responds to global inflationary pressures between 1970 and 2022. Rather than focusing on predictive modeling, the analysis emphasizes **economic reasoning, data integrity, and contextual interpretation** — mirroring how inflation analysis is approached in policy, finance, and applied data roles.

The core question addressed is:

> **Does South Africa merely follow global inflation trends, or do domestic factors amplify global inflation shocks?**

---

## Why This Project Matters

Inflation affects interest rates, currency stability, household purchasing power, and long-term economic growth. For emerging economies like South Africa, global inflation shocks (e.g. oil crises, global recessions, post-pandemic supply constraints) often interact with **local structural and monetary factors**, producing outcomes that differ from global averages.

Understanding this divergence is critical for:

* Economic policy evaluation
* Risk analysis in emerging markets
* Macro-financial decision-making

---

## Data Sources

Two publicly available macroeconomic datasets were used:

1. **Global Inflation Dataset (1970–2022)**
   Source: IMF / Kaggle
   Description: Annual average headline CPI inflation for countries worldwide.

2. **Consumer Price Index (CPI) Dataset**
   Source: Kaggle
   Description: CPI data used for cross-validation and structural understanding.

---

## Data Preparation & Methodology

### 1. Data Cleaning

* Removed unnamed and metadata-only columns
* Resolved encoding issues during CSV import
* Converted wide-format year columns (1970–2022) into long format

### 2. Handling Multiple Observations per Year

The raw IMF dataset contained **multiple inflation observations per country-year**, originating from different frequency blocks and reporting structures.

To ensure temporal consistency:

* Inflation values were **aggregated using annual averages** per country-year

This approach aligns with standard macroeconomic analysis practices.

### 3. Global Benchmark Construction

A global inflation benchmark was created by:

* Calculating the **mean inflation rate across all reporting countries per year**

This serves as a proxy for **global inflation stress**.

### 4. Inflation Gap Metric

To measure divergence, an **Inflation Gap** was computed:

```
Inflation Gap = South Africa Inflation − Global Average Inflation
```

Positive values indicate South Africa experiencing **higher inflation than global peers**.

---

## Key Findings

### Major Inflation Divergence Periods

South Africa experienced its largest positive inflation gaps in the following years:

| Year | SA Inflation | Global Avg | Gap      |
| ---- | ------------ | ---------- | -------- |
| 2002 | 17.39%       | 5.93%      | +11.46pp |
| 1977 | 25.10%       | 15.12%     | +9.98pp  |
| 1981 | 25.20%       | 17.93%     | +7.27pp  |
| 2022 | 24.37%       | 17.29%     | +7.08pp  |
| 2009 | 9.53%        | 3.33%      | +6.20pp  |

---

## Interpretation

### 1. Domestic Amplification of Global Shocks

In several periods (notably 2002), South Africa’s inflation far exceeded global levels despite moderate global inflation, suggesting **domestic monetary, fiscal, or currency-driven pressures**.

### 2. Structural Vulnerability During Global Stress

During the late 1970s and early 1980s — periods associated with oil shocks and global monetary tightening — South Africa consistently **amplified global inflation trends**.

### 3. Persistent Pattern into Modern Era

The 2022 inflation surge demonstrates that this divergence is **not historical only**, but remains relevant in contemporary macroeconomic conditions.

---

## Conclusion

South Africa does not simply absorb global inflation shocks — it frequently **experiences amplified inflation outcomes** relative to global averages. This suggests that domestic economic dynamics play a significant role in shaping inflation outcomes, especially during periods of global stress.

This finding highlights the importance of country-specific policy responses when managing inflation in emerging markets.

---

## Skills Demonstrated

* Real-world data cleaning and schema inspection
* Wide-to-long data reshaping
* Handling duplicate temporal observations
* Macro-level benchmarking
* Business-focused economic interpretation

---

## Possible Extensions

* Visualizing inflation gaps over time
* Comparing South Africa to peer emerging markets
* Incorporating exchange rate or interest rate data

---

## Author

**Thuto Lefa Motlana**
Data Science & Analytics Portfolio Project
