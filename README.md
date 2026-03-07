
---

# ICC T20 Match Data Analysis

## Project Overview

This project analyzes T20 cricket match data from the International Cricket Council (ICC). The dataset contains **1417 T20 matches**, where each row represents a single match.

As part of the ICC Analytics Team, the objective of this assignment is to explore the dataset, verify its integrity, and perform analytical tasks that can support **pre-match, live-match, and post-match insights**.

The project focuses on **data exploration, cleaning, and analytical insights** derived from historical T20 match records.

---

# Dataset Information

* **Total Matches:** 1417
* **Format:** T20 Cricket
* **Structure:** Each row corresponds to a single match

The dataset includes information such as:

* Match metadata
* Teams participating
* Venue details
* Match results
* Innings data
* Player performances

---

# Objectives

## 1. Data Cleaning

Rename column names to more appropriate and readable formats.

Example:

```
meta.created → created_date
```

---

## 2. Venue Analysis

Identify the **top three venues** that hosted the highest number of T20 matches.

---

## 3. Team Rivalry Analysis

Determine the **pair of teams that have played the most T20 matches against each other**.

---

## 4. Win Percentage Analysis

Calculate the **top five teams based on win percentage**.

The win percentage is calculated as:

[
Win\ Percentage = \left(\frac{\text{Matches Won}}{\text{Matches Played}}\right) \times 100
]

---

## 5. Scorecard Generation

Develop a function that generates scorecards for each match.

### Function Input

```
innings
```

### Function Output

The function returns **two DataFrames**:

**First DataFrame**

* Top 4 scorers from the team batting first
* Top 4 bowlers from the opposing team

**Second DataFrame**

* Top 4 scorers from the team batting second
* Top 4 bowlers from the opposing team

---

# Technologies Used

* Python
* Pandas
* NumPy
* Jupyter Notebook / Google Colab

(Optional if used)

* Matplotlib
* Seaborn

---

# Analysis Workflow

The project follows these steps:

1. Load the dataset
2. Inspect the data structure
3. Rename columns for clarity
4. Perform data validation and sanity checks
5. Conduct exploratory data analysis
6. Compute statistical insights
7. Implement the scorecard generation function

---

# How to Run the Project

### Clone the Repository

```
git clone https://github.com/yourusername/icc-t20-analysis.git
```

### Install Required Libraries

```
pip install pandas numpy matplotlib seaborn
```

### Run the Notebook

Open the notebook using:

* Jupyter Notebook, or
* Google Colab

---

# Author

Abhinav

