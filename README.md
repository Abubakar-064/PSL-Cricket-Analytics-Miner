# 🏏 PSL Cricket Analytics Miner

**DS-311 Data Mining Semester Project | Fall 2026**  
**BS Artificial Intelligence | National University of Sciences and Technology (NUST)**

## 📌 Project Overview

The **PSL Cricket Analytics Miner** is a data mining project that analyzes ball-by-ball cricket data from the Pakistan Super League (PSL) to discover patterns in team performance, match outcomes, and player playing styles.

The project aims to investigate what separates winning and losing T20 innings and how data mining techniques can identify meaningful cricket performance patterns.

The implementation uses Python, Pandas, NumPy, Matplotlib, Seaborn, and Scikit-learn in Google Colab.

## 🎯 Project Objectives

- Analyze PSL ball-by-ball cricket data.
- Assess data quality by identifying missing values, duplicates, inconsistencies, and potential outliers.
- Explore scoring patterns, wickets, innings phases, venues, and seasons.
- Investigate the relationship between winning the toss and winning the match.
- Develop player profiles based on batting and bowling performance.
- Apply clustering, association rule mining, and classification techniques.
- Develop an interactive cricket analytics dashboard as a future project component.

## 📊 Dataset

**Dataset:** PSL Men's Ball-by-Ball Cricket Data  
**Source:** [Cricsheet](https://cricsheet.org/)  
**Format:** CSV  
**Unit of observation:** Individual ball-level records

The initial dataset contains:

- **83,799 rows**
- **64 columns**
- **357 unique matches**

These figures describe the initial dataset and should be updated if the dataset changes during preprocessing.

The dataset includes information about matches, innings, teams, batters, bowlers, runs, wickets, venues, seasons, toss decisions, and match results.

## 🧹 Week 7 — M1: Data Quality and Exploratory Data Analysis

The first milestone focuses on understanding and validating the dataset before applying data mining techniques.

### Data Quality Assessment

- Dataset structure, dimensions, and data types
- Data dictionary generation
- Missing-value analysis
- Exact duplicate detection
- Repeated delivery-key investigation
- Data consistency checks
- IQR-based potential outlier detection
- Conservative data cleaning and export

### Exploratory Data Analysis (EDA)

- Match counts by season
- Run distributions at delivery level
- Dismissal-type analysis
- Innings-level runs, legal balls, wickets, and run rate
- Powerplay, middle-over, and death-over analysis
- Venue and season comparisons
- Numeric correlation heatmap
- Hypothesis testing for the association between toss victory and match victory

Statistical outliers are investigated rather than automatically removed because unusual scoring events may be legitimate cricket outcomes.

## 💻 Google Colab Notebook

Run and explore the project notebook in Google Colab:

**[Open PSL Cricket Analytics Miner — Google Colab](https://colab.research.google.com/drive/1cmduQEFCmPGodSSK-MfFHuBBVX5SFtip#scrollTo=MdIZFH4Ywmzo)**

### How to Run

1. Open the Google Colab notebook using the link above.
2. Sign in to your Google account.
3. Run the notebook cells sequentially from top to bottom.
4. Upload `psl_male_ball_by_ball.csv` when prompted.
5. Review the generated data-quality reports and EDA visualizations.
6. Download the exported reports and cleaned dataset when the notebook finishes.

The notebook requires the dataset to be uploaded separately unless it is already available in your Google Drive or notebook environment.

## 🛠️ Technologies Used

- **Python** — Main programming language
- **Pandas** — Data manipulation and analysis
- **NumPy** — Numerical operations
- **Matplotlib** — Data visualization
- **Seaborn** — Statistical visualization
- **SciPy** — Statistical hypothesis testing
- **Google Colab** — Cloud-based notebook environment
- **Scikit-learn** — Planned machine learning and data mining workflows

## 🗂️ Expected Project Outputs

The M1 notebook generates CSV reports, including:

- `psl_data_dictionary.csv`
- `psl_missing_values_report.csv`
- `psl_duplicate_report.csv`
- `psl_consistency_report.csv`
- `psl_outlier_report.csv`
- `psl_cleaned_ball_by_ball.csv`
- `psl_innings_statistics.csv`
- `psl_season_eda.csv`
- `psl_correlation_matrix.csv`
- `psl_final_quality_summary.csv`

These files are packaged into `PSL_M1_Data_Quality_and_EDA.zip`.

## 🚀 Planned Future Work

The subsequent stages of the project will focus on the following:

### 1. Player Profiling and Clustering
Create player-performance features and use PCA, K-Means, and hierarchical clustering to identify playing styles.

### 2. Association Rule Mining
Identify match-state patterns associated with winning outcomes using support, confidence, and lift.

### 3. Chase-Success Classification
Compare baseline and machine learning models, including Decision Trees and Random Forests, using a season-based evaluation split.

### 4. Interactive Dashboard
Develop a Streamlit application for match analytics, player profiles, winning patterns, and chase-state analysis.

These components are planned extensions and should be marked complete only when their implementations and evaluations are available.

## 📚 Academic Context

This project is part of the **DS-311 Data Mining** semester project at the National University of Sciences and Technology (NUST), Pakistan.

The work follows the course project's requirements for data acquisition, data-quality assessment, exploratory analysis, data transformation, mining techniques, evaluation, interpretation, and an interactive application.

## 👨‍🎓 Author

**[Your Full Name]**  
BS Artificial Intelligence  
National University of Sciences and Technology (NUST), Pakistan  
Course: DS-311 Data Mining  
Semester: Fall 2026

## 📄 Data Source and Attribution

Cricket data is sourced from [Cricsheet](https://cricsheet.org/). Please consult the source website for applicable attribution and data-use terms.

## ⚠️ Limitations

- Data-quality issues may affect individual analyses.
- Statistical associations do not establish causation.
- Player comparisons depend on sample size, playing role, season, and match conditions.
- Super overs, shortened matches, and no-result matches require special handling.
- Machine learning results must be evaluated using appropriate splits and checks for target leakage.

---

*This repository documents the development of a cricket analytics solution using data mining techniques for academic purposes.*
