# TikTok Engagement Analytics – Content Performance & Trends
This repository contains my work for the **TikTok capstone project** from the Google Advanced Data Analytics programme.
The goal is to use TikTok post-level data to:
- Explore which content features (e.g. video category, duration, hashtags, posting time) are associated with higher engagement.
- Visualise engagement patterns and trends.
- Provide practical recommendations for improving content performance.
The analysis is implemented in Python using **pandas**, **NumPy**, **Matplotlib**, **Seaborn**, **Plotly**, and **SciPy**.
---
## Repository structure
- `Tik_Tok_Google_Advanced_Data_Analytics.ipynb`  
  Main Jupyter notebook. It includes:
  - Data loading and cleaning for the TikTok dataset.
  - Exploratory data analysis (EDA) with summary statistics.
  - Visualisations of engagement metrics (likes, shares, comments, views).
  - Feature analysis by category/hashtag/posting time/etc.
  - Simple statistical tests and/or correlations to quantify relationships.
- `tiktok_dataset.csv`  
  The TikTok dataset used in the analysis, containing post-level features and engagement metrics.
- `README.md`  
  This file.
---
## How to run the notebook
### 1. Clone the repository
```bash
git clone https://github.com/barbavegeta/Google_Advanced_Data_Analytics-TikTok_Project.git
cd Google_Advanced_Data_Analytics-TikTok_Project
```
### 2. Create and activate an environment
Using **conda** (example):
```bash
conda create -n tiktok_project python=3.10 -y
conda activate tiktok_project
```
### 3. Install dependencies
```bash
pip install   numpy   pandas   matplotlib   seaborn   plotly   scipy   jupyter
```
(If some extra library is used in the notebook and missing, install it when Python complains.)
### 4. Launch Jupyter
```bash
jupyter notebook
```
Open:
```text
Tik_Tok_Google_Advanced_Data_Analytics.ipynb
```
and run the cells from top to bottom.
---
## Analysis outline (high level)
The notebook roughly follows these steps:
1. **Load & inspect data**
   - Read `tiktok_dataset.csv` into a pandas DataFrame.
   - Inspect column names, data types, and basic structure.
   - Check for missing values and obvious data quality issues.
2. **Exploratory data analysis (EDA)**
   - Compute summary statistics for engagement metrics (views, likes, comments, shares).
   - Visualise distributions and identify outliers.
   - Look at engagement broken down by key features (category, content type, etc.).
3. **Feature relationships & statistical checks**
   - Examine correlations between numeric features and engagement.
   - Compare engagement across categories/segments using groupby operations and simple tests where relevant (e.g. t-tests/ANOVA-style checks).
4. **Visualisation**
   - Build static plots (Matplotlib/Seaborn) and, optionally, interactive charts (Plotly) to show:
     - Top-performing content categories.
     - Engagement vs posting time or other relevant features.
     - Relationships between multiple engagement metrics.
5. **Recommendations**
   - Translate the patterns into concrete, data-backed suggestions for optimising TikTok content: e.g. what to post more of, when to post, which metrics to track.
---
## Notes
- This project is a **learning / portfolio piece** based on a teaching dataset, not a production system.
- The emphasis is on:
  - Clean exploratory analysis.
  - Clear visualisations.
  - Direct links from data patterns to practical content strategy recommendations.
