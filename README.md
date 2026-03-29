# Data-Science-Assignment2: Movie Insights for Production & Casting

This project provides a data-driven analysis for a rookie movie producer to help them make informed decisions regarding movie production and casting choices. The analysis is based on a dataset of 3,000 movies.

---

## 🔍 Objectives & Questions Addressed
* **Profitability:** Identifying the movie with the highest profit and its key cast/crew.
* **Global ROI:** Finding which language yields the highest average Return on Investment.
* **Market Landscape:** Mapping the unique genres available in the dataset.
* **Stakeholder Performance:** Identifying top producers by ROI and top directors' actor preferences.
* **Star Power:** Deep-diving into the most prolific actor's performance and genre range.

---

## 📊 Key Findings from Analysis

### 1. Highest Profit Movie
* **Title:** *Furious 7*
* **Director:** James Wan
* **Producers:** Vin Diesel, Neal H. Moritz, Michael Fottrell, Brandon Birtell
* **Lead Cast:** Vin Diesel, Paul Walker, Dwayne Johnson, Michelle Rodriguez, etc.

### 2. ROI by Language
The language with the highest average Return on Investment (ROI) is **Korean (ko)**, with an average ROI of approximately **381,794**.

### 3. Unique Genres
The dataset covers a wide variety of genres including:
`Action`, `Adventure`, `Animation`, `Comedy`, `Crime`, `Documentary`, `Drama`, `Family`, `Fantasy`, `Foreign`, `History`, `Horror`, `Music`, `Mystery`, `Romance`, `Science Fiction`, `TV Movie`, `Thriller`, `War`, `Western`.

### 4. Prolific Actor Analysis
**Samuel L. Jackson** is the most frequent actor in this dataset.
* **Total Movies:** 30
* **Avg Profit per Movie:** ~$226,510,055
* **Genre Range:** Spans 15 unique genres including Action, Sci-Fi, and Drama.

### 5. Director Preferences (Top 3)
* **Ron Howard:** Frequently casts Clint Howard and Rance Howard.
* **Steven Spielberg:** Frequently casts Harrison Ford, Tom Hanks, and Pat Roach.
* **Todd Phillips:** Frequently casts Matt Walsh, Bradley Cooper, and Juliette Lewis.

---

## 🛠️ Implementation Details
The analysis was performed using **Python** and **Pandas**. Key steps included:
1. **Profit Calculation:** `df['revenue'] - df['budget']`
2. **ROI Calculation:** `df['profit'] / df['budget']`
3. **Data Parsing:** Used `ast.literal_eval` to extract names from JSON-like strings in the `cast`, `crew`, and `genres` columns.
4. **Aggregation:** Grouped data by language, producer, and director to find top performers.

---

## 📁 Repository Structure
* `imdb_data.csv`: The primary dataset.
* `Assignment2.ipynb`: The Jupyter Notebook containing the Python code and logic.
