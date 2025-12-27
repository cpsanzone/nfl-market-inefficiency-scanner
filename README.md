# Cross-Sport Market Efficiency Analyzer

### Project Overview
A comprehensive data analysis framework designed to audit historical NFL and NBA market lines (Totals and Spreads) against actual game results. The tool utilizes granular segmentation to identify "Market Inefficiencies"—specific game conditions where the actual outcome consistently deviates from the projected market line, offering a statistically significant Return on Investment (ROI).

### 🔧 Key Technical Competencies
* **Automated Data Pipeline:** Engineered a robust ETL (Extract, Transform, Load) process using the Kaggle API to ingest multi-season datasets, including automated error handling for missing file structures.
* **Granular Segmentation (Binning):** Developed logic to categorize continuous variables (Total Lines, Spreads) into discrete "Performance Buckets" (e.g., 'Total < 40', 'Spread 1.5-3.5') to isolate specific high-yield trends.
* **Sensitivity Analysis:** Performed iterative "Sweet Spot" analysis to determine optimal range parameters (parlay spans), dynamically adjusting payout structures to model real-world profit factors.

### 📊 Methodology & Results
* **Objective:** To identify specific game environments where market variance allows for optimized capital allocation.
* **Analysis:** Processed 3+ seasons of game data, merging weather conditions and granular betting lines.
* **Result:** Uncovered high-value inefficiencies in the NFL market, specifically isolating a **101% ROI** segment in games with '40-45' Total Lines and '7.5+' Spreads, validating the model's ability to find signal in the noise.
