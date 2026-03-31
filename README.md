
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

---

# IMDB Movie Data Analysis

## Project Overview

This project analyzes **IMDB movie data** to explore profitability, genres, cast, crew, and return on investment (ROI) across 3,000 movies. The dataset contains comprehensive information about movies including budget, revenue, cast, crew, genres, and other metadata.

The objective is to perform **data exploration, cleaning, and financial analysis** to answer key questions about movie profitability, industry trends, and the relationships between cast, directors, producers, and financial performance.

---

# Movie Dataset Information

* **Total Movies:** 3,000
* **Total Features:** 23 columns
* **Structure:** Each row represents a single movie

The dataset includes information such as:

* Budget and Revenue
* Cast and Crew details
* Genres and Keywords
* Release date and runtime
* Production companies and countries
* Movie metadata (title, overview, ratings, etc.)

**Data Location:** `datasets/imdb_data (1).csv`

---

# Movie Project Objectives

## Q1: Highest Profit Movie Analysis

Identify the **movie that made the highest profit** and provide details about:
* Budget and Revenue
* Return on Investment (ROI)
* Director and Producer
* Main Cast (top 5 actors)

**Result:** Furious 7 with $1.32B profit and 692.76% ROI

---

## Q2: Language & ROI Analysis

Determine which **language has the highest average ROI** among movies with at least 5 movies in the dataset.

**Analysis includes:**
* Average ROI by language (filtered for reliability)
* Language distribution (Top 5)
* Bar chart of top 12 languages by ROI
* Pie chart showing language distribution

**Result:** Korean (ko) language has the highest average ROI

---

## Q3: Genre Analysis

Find all **unique genres** in the dataset and analyze their distribution.

**Analysis includes:**
* Count of unique genres
* Complete list of all genres
* Movie count per genre
* Bar chart visualization of genre popularity

**Result:** 20 unique genres identified (Drama, Comedy, Thriller, Action, etc.)

---

## Q4: Producer & ROI Analysis

Identify the **top 3 producers with highest average ROI** (minimum 3 movies produced).

**Analysis includes:**
* Create table of all movies with Director and Producer
* Group by Producer and calculate average ROI
* Filter producers with at least 3 movies
* Top producers ranking and visualization

**Result:** Charlie Chaplin leads as top producer by average ROI

---

## Q5: Prolific Actor Deep Dive

Discover the **actor who appeared in the most number of movies** and perform comprehensive analysis.

**Analysis includes:**
* Actor filmography count
* Top movies by profit (with details)
* Genre breakdown for this actor's films
* Profit distribution histogram
* Charts for genres and top profitable films

**Result:** Samuel L. Jackson (17 movies, primarily in Action/Crime/Adventure genres)

---

## Q6: Director & Actor Preferences

Analyze the **top 3 directors** and identify their **preferred actors**.

**Analysis includes:**
* Identify top 3 most prolific directors
* For each director, find their favorite actors
* Show frequency of collaborations
* Side-by-side bar charts comparing actor preferences

**Result:** 
* Steven Spielberg → Harrison Ford
* Clint Eastwood → Clint Eastwood (himself)
* Ron Howard → Clint Howard

---

# Movie Project Key Metrics & Calculations

### Profit Formula
```
Profit = Revenue - Budget
```

### Return on Investment (ROI)
```
ROI = (Profit / Budget) × 100
```

### Data Cleaning Steps for Movie Analysis
1. Remove rows where Budget = 0 or Revenue = 0
2. Capitalize column names for consistency
3. Parse stringified lists (Cast, Crew, Genres) using `ast.literal_eval()`
4. Filter movies with valid actor information

---

# Movie Notebook Structure

The `movie_assignment.ipynb` notebook contains:
* Data loading and exploration
* Data cleaning and preprocessing
* Helper functions for parsing complex columns
* 6 analytical questions (Q1-Q6) with visualizations
* Summary tables and insights

All cells are executable and dependencies are properly managed.

