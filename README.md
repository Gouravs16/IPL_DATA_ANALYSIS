# 🏏 IPL Data Analysis — Internship Project

## Bharat Cares × IBM Collaboration 

This project was developed as part of an **internship project with Bharat Cares in collaboration with IBM**.

The project focuses on performing an end-to-end **IPL Data Analysis** using Python and data analytics techniques. The objective is to transform raw IPL match data into meaningful insights through data cleaning, feature engineering, exploratory data analysis, visualization, and an interactive dashboard.

---

## 📌 Project Overview

The project analyzes IPL match-level data to understand patterns related to:

- IPL seasons
- Team participation and performance
- Match outcomes
- Toss decisions
- Venues
- Winning margins
- Player of the Match awards
- Scoring trends
- League and Playoff / Knockout matches

The complete workflow follows:

**Data Collection → Data Cleaning → Data Validation → Feature Engineering → EDA → Visualization → Statistical Analysis → Interactive Dashboard → Insights**

---

## 🎯 Project Objectives

- Understand the structure and quality of IPL match data.
- Perform data cleaning and validation.
- Handle missing values appropriately.
- Preserve meaningful missing `match_number` values.
- Standardize historical team names.
- Analyze season-wise match participation.
- Analyze team wins and win percentages.
- Study toss decisions and match outcomes.
- Analyze IPL venues.
- Study winning margins by runs and wickets.
- Analyze Player of the Match awards.
- Analyze season-wise scoring trends.
- Compare team-wise average scoring.
- Build an interactive IPL analytics dashboard.
- Generate data-driven observations and insights.

---

## 🏢 Internship Information

| Details | Information |
|---|---|
| Project Type | Internship Project |
| Organization | Bharat Cares |
| Collaboration | IBM |
| Project Domain | Data Analytics / Data Science |
| Project Title | IPL Data Analysis |
| Development Environment | Google Colab |
| Data Preparation | Google Sheets |
| Programming Language | Python |

---

## 📊 Dataset

The project uses IPL match-level data.

Important fields include:

- `season`
- `date`
- `city`
- `venue`
- `team1`
- `team2`
- `toss_winner`
- `toss_decision`
- `team1_runs`
- `team2_runs`
- `team1_wickets`
- `team2_wickets`
- `winner`
- `win_by_runs`
- `win_by_wickets`
- `player_of_match`
- `result_type`
- `match_number`
- `event_name`

---

## 🧹 Data Cleaning

The following data-quality steps were performed:

- Cleaned column names.
- Removed unnecessary whitespace from text fields.
- Converted date values into datetime format.
- Checked missing values.
- Investigated missing `winner` values.
- Investigated missing `player_of_match` values.
- Checked duplicate records.
- Validated data types.
- Checked team-name consistency.
- Standardized historical team names.
- Created analytical features.

### Important Handling of `match_number`

Missing `match_number` values were not treated as ordinary missing data.

In this dataset, missing match numbers represent **Playoff / Knockout matches**. Therefore, they were preserved instead of being deleted or artificially filled.

A `match_stage` feature was created:

```text
League
Playoff / Knockout
```

---

## 🔧 Historical Team Name Standardization

Historical names were standardized so that the same franchise was not incorrectly treated as different teams.

| Historical Name | Standardized Name |
|---|---|
| Royal Challengers Bangalore | Royal Challengers Bengaluru |
| Rising Pune Supergiants | Rising Pune Supergiant |
| Kings XI Punjab | Punjab Kings |
| Delhi Daredevils | Delhi Capitals |

This standardization is important for accurate team-level analysis.

---

## ⚙️ Feature Engineering

The project created analytical features including:

- `season_year`
- `team_pair`
- `match_stage`
- `result_category`
- `toss_match_same`
- `win_margin`
- `margin_type`
- `total_match_runs`

### Match Result Categories

Matches were categorized into:

- Win by Runs
- Win by Wickets
- Other / No Result

---

## 📈 Exploratory Data Analysis

### 1. Season Analysis

- Matches by season
- Season-wise team performance
- Season-wise scoring
- Average runs per match

### 2. Team Analysis

- Team participation
- Team wins
- Team win percentage
- Season-wise team performance
- Team-wise scoring performance

### 3. Toss Analysis

- Toss decision distribution
- Toss winner vs match winner
- Batting first vs fielding first

### 4. Venue Analysis

- Matches hosted by venue
- Top IPL venues

### 5. Match Result Analysis

- Wins by runs
- Wins by wickets
- Other / No Result
- Run-margin distribution
- Wicket-margin distribution

### 6. Player Analysis

- Player of the Match awards
- Top Player of the Match award counts
- Season-wise Player of the Match analysis

### 7. Match Stage Analysis

- League matches
- Playoff / Knockout matches
- Stage-wise team performance

---

## 📊 Data Visualizations

Different visualization techniques were used according to the analytical requirement:

- Bar charts
- Horizontal bar charts
- Line charts
- Histograms
- Box plots
- Pie charts
- Donut charts
- Heatmaps
- Grouped bar charts
- Interactive Plotly visualizations

---

## 🖥️ Interactive IPL Dashboard

The final dashboard combines important project findings into a single interactive analytical view.

### Dashboard includes:

- Total Matches
- Total Seasons
- Total Teams
- Total Venues
- Matches by Season
- Average Runs by Season
- Team Wins
- Team Win Percentage
- Toss Decision Distribution
- Match Result Distribution
- Player of the Match Awards
- Top Venues
- Run Margin Distribution
- Wicket Margin Distribution
- League vs Playoff / Knockout
- Team Average Scoring

The interactive dashboard was developed using **Plotly**.

---

## 🛠️ Technology Stack

### Programming Language
- Python

### Data Analysis
- Pandas
- NumPy

### Visualization
- Matplotlib
- Seaborn
- Plotly

### Data Preparation
- Google Sheets
- CSV

### Development
- Google Colab
- Jupyter Notebook

### Version Control
- Git
- GitHub

---

## 📂 Project Structure

```text
IPL_Data_Analysis/
│
├── GouravSolanke_IPL_Data_Analysis.ipynb
├── requirements.txt
├── GouravSolanke_IPL_ProjectReport.docx
├── README.md
│
└── data/
    └── IPL_Dataset.csv
```

---

## ▶️ How to Run the Project

### Step 1 — Clone the repository

```bash
git clone <your-github-repository-url>
```

### Step 2 — Install dependencies

```bash
pip install -r requirements.txt
```

### Step 3 — Open the notebook

Open:

```text
GouravSolanke_IPL_Data_Analysis.ipynb
```

using Google Colab, Jupyter Notebook, or VS Code.

### Step 4 — Run the notebook

Run the notebook cells sequentially:

```text
Load Data
    ↓
Understand Dataset
    ↓
Data Quality Checks
    ↓
Data Cleaning
    ↓
Feature Engineering
    ↓
Exploratory Data Analysis
    ↓
Visualization
    ↓
Statistical Analysis
    ↓
Interactive Dashboard
    ↓
Final Insights
```

---

## 🔍 Key Analytical Questions

The project investigates questions such as:

- How many IPL matches were played in each season?
- How does average scoring change across seasons?
- How many seasons did each team participate in?
- How did team win percentages vary across seasons?
- What toss decisions were most common?
- How often did the toss-winning team also win the match?
- Which venues hosted the most matches?
- How were matches won: by runs or wickets?
- What are the common winning margins?
- Which players received Player of the Match awards most frequently?
- How does team scoring vary?
- How do League and Playoff / Knockout matches differ?

---

## 🧠 Analytical Approach

The project follows a structured data analytics methodology:

### Data Understanding
First, the dataset structure, columns, dimensions, data types, and missing values were inspected.

### Data Cleaning
Data-quality issues were investigated and corrected while preserving meaningful information.

### Feature Engineering
Additional variables were created to support deeper analysis.

### Exploratory Data Analysis
Multiple analytical views were created to understand season, team, toss, venue, player, scoring, and match-result patterns.

### Visualization
Charts were selected according to the type of question being analyzed.

### Dashboard
The most important findings were combined into an interactive dashboard.

---

## ⚠️ Analytical Considerations

The analysis is **descriptive and observational**.

For example, an association between toss decisions and match outcomes does not by itself prove that the toss decision caused the match result.

Similarly:

- Total wins depend on the number of matches played.
- Win percentage can be affected by sample size.
- Venue frequency does not measure venue quality.
- Player of the Match awards are not a complete measure of player performance.
- Historical team-name variations must be standardized before team-level analysis.
- Playoff / Knockout classification is based on the dataset's meaningful missing `match_number` values and should not be used to infer a specific Final, Qualifier, or Eliminator unless those stages are explicitly available in the data.

---

## 🚀 Future Scope

The project can be extended with:

- Player-level batting analysis
- Player-level bowling analysis
- Strike-rate analysis
- Economy-rate analysis
- Powerplay analysis
- Death-over analysis
- Venue-based team performance
- Player performance prediction
- Match outcome prediction
- Machine learning models
- Advanced statistical testing
- Advanced interactive dashboards
- Time-series analysis

---

## 📚 Project Deliverables

The internship project consists of:

```text
1. Jupyter / Google Colab Notebook
2. requirements.txt
3. Project Report
4. README.md
5. IPL Dataset
```

---

## 👨‍💻 Project Author

**Gourav Solanke**

B.Tech — Computer Science & Engineering

Pimpri Chinchwad University, Pune

---

## 🏢 Internship Context

**Developed as an internship project under Bharat Cares in collaboration with IBM.**

The project demonstrates practical application of Python-based data analytics, exploratory data analysis, data visualization, and dashboard development on a real-world sports dataset.

---

## 📜 License

This project is intended for educational and internship purposes.
