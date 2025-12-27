# NFL Market Efficiency Analyzer

### Project Overview
A quantitative analysis framework designed to audit historical NFL market lines (Totals and Spreads) against actual game results. The tool utilizes granular segmentation to identify "Market Inefficiencies"—specific game conditions where the actual outcome consistently deviates from the projected market line, offering a statistically significant Return on Investment (ROI).

### 🔧 Key Technical Competencies
* **Secure Data Pipeline:** Engineered a custom ETL process using `google.colab.userdata` and the Kaggle API to ingest 14,000+ historical records without exposing credentials.
* **Granular Segmentation:** Developed logic to categorize continuous variables into discrete "Performance Buckets" (e.g., 'Total < 40', 'Spread 7.5+') to isolate specific high-yield trends.
* **Interactive Tooling:** Built a self-contained Python application that accepts user inputs (Line/Spread) and instantly queries historical data to generate "Gold Tier" betting recommendations.

### 📊 Methodology & Results
* **Objective:** To identify specific game environments where market variance allows for optimized capital allocation.
* **Findings:**
    * **The "Gold" Segment:** Identified a specific inefficiency in low-total games (<40) with tight spreads, yielding a **10%+ ROI** over a significant sample size.
    * **Market Efficiency:** Verified that the vast majority of NFL lines are highly efficient, requiring precise filtering to find profitable edges.

### 🛠 Tools Used
* **Languages:** Python (Pandas, NumPy)
* **Data Source:** Kaggle API (Toby Crabtree's NFL Dataset)
* **Development:** Google Colab, Model Serialization

### 🔐 How to Run This Project
This project uses **Google Colab Secrets** to securely handle credentials.
1. Open the notebook in Google Colab (click the badge above).
2. Click the **Key Icon** (Secrets) in the left sidebar.
3. Add two new secrets:
   * `KAGGLE_USERNAME`: Your Kaggle username.
   * `KAGGLE_KEY`: Your Kaggle API key.
4. Run all cells to launch the **Interactive Recommendation Tool**.
