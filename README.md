# Uber Drive Data Analysis using Python

## 📌 Project Overview

This project focuses on analyzing **Uber Drive trip data using Python** to understand travel patterns and user behavior.

The dataset contains information about:

* Trip dates and times
* Trip categories
* Starting and stopping locations
* Travel distance
* Trip purposes

The project applies **data cleaning, feature engineering, exploratory data analysis (EDA), and data visualization** techniques to transform raw trip data into meaningful insights.

---

## 🎯 Objectives

* Analyze Uber Drive trip data
* Clean and preprocess the dataset
* Identify travel patterns
* Analyze trip distance and duration
* Explore trip purposes and categories
* Identify frequently used routes
* Analyze monthly and time-of-day travel patterns
* Visualize the data
* Generate business-oriented insights

---

## 🛠️ Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Jupyter Notebook**

---

## 📂 Dataset

The dataset contains **1,156 records and 7 columns** in its original form.

### Main Columns

| Column        | Description                                |
| ------------- | ------------------------------------------ |
| `START_DATE*` | Date and time when the trip started        |
| `END_DATE*`   | Date and time when the trip ended          |
| `CATEGORY*`   | Trip category such as Business or Personal |
| `START*`      | Starting location                          |
| `STOP*`       | Destination location                       |
| `MILES*`      | Distance travelled in miles                |
| `PURPOSE*`    | Purpose of the trip                        |

The original dataset also contained a **Totals** row, which was removed during data cleaning.

---

## 🧹 Data Cleaning

The following preprocessing steps were performed:

1. Removed the `Totals` row from the dataset.
2. Corrected the location value `Kar?chi` to `Karachi`.
3. Replaced missing values in `PURPOSE*` with `UNKNOWN`.
4. Removed duplicate records.
5. Converted `START_DATE*` and `END_DATE*` into datetime format.
6. Prepared the dataset for further analysis.

After removing the totals row, the dataset contained **1,155 trip records**.

---

## ⚙️ Feature Engineering

Several new features were created from the existing data:

* **DATE** – Extracted date from the trip start time
* **TIME** – Extracted the hour from the start time
* **DAY-NIGHT** – Classified trips into:

  * Early Morning
  * Morning
  * Afternoon
  * Evening
* **MONTH** – Extracted the month
* **MINUTES** – Calculated trip duration in minutes
* **DAY** – Extracted the day of the week
* **ROUNDTRIP** – Identified whether the starting and stopping locations were the same

---

## 📊 Exploratory Data Analysis

The project performs different types of exploratory analysis to understand trip behavior.

### Univariate Analysis

The analysis examines:

* Trip category
* Trip purpose
* Time-of-day period
* Round-trip status

### Route Analysis

The project identifies the most frequently occurring combinations of starting and stopping locations.

The most frequent combinations included:

* Unknown Location → Unknown Location: **86 trips**
* Morrisville → Cary: **75 trips**
* Cary → Morrisville: **67 trips**

### Trip Duration Analysis

Trip duration was calculated using the difference between the start and end timestamps.

The maximum recorded duration was:

* **Business:** 336 minutes
* **Personal:** 185 minutes

### Monthly Travel Analysis

Monthly travel distance was analyzed to identify changes in travel activity throughout the year.

* **October:** Highest total travel distance — **1,810 miles**
* **May:** Lowest total travel distance — **363.8 miles**

### Round-Trip Analysis

The analysis identified **288 trips** where the starting and stopping locations were the same, with an average distance of approximately **7.74 miles**.

### Time-of-Day Analysis

The average trip distance was highest during the:

* **Early Morning:** approximately 12.35 miles
* **Afternoon:** approximately 11.25 miles

---

## 🔍 Key Insights

### Trip Purpose

Among the identified trip purposes:

* **Meeting:** 187 rides
* **Meal/Entertain:** 160 rides
* **Errand/Supplies:** 128 rides

However, **502 rides had an unknown purpose**, showing that missing purpose information is an important limitation of the dataset.

### Frequently Used Routes

The analysis identified **Morrisville → Cary** and **Cary → Morrisville** as frequently occurring identifiable routes.

### Travel Patterns

October recorded the highest total travel distance, while May recorded the lowest.

### Trip Duration

Business trips showed a wider duration range than Personal trips, with Business trips reaching a maximum recorded duration of 336 minutes.

---

## 💡 Business Insights

The analysis can help identify:

* Frequently used travel routes
* High-travel months
* Common trip purposes
* Travel behavior by time of day
* Differences between Business and Personal trips
* Areas where improved data collection could provide better insights

The presence of a large number of trips with unknown purposes also highlights the importance of improving data collection and recording practices.

---

## 📈 Project Workflow

```text
Raw Dataset
     ↓
Data Understanding
     ↓
Data Cleaning
     ↓
Feature Engineering
     ↓
Exploratory Data Analysis
     ↓
Data Visualization
     ↓
Pattern Identification
     ↓
Business Insights
     ↓
Conclusion
```

---

## 🏁 Conclusion

The Uber Drive dataset contained **1,155 trip records after removing the totals row**.

The analysis explored trip purposes, travel distances, trip durations, routes, time-of-day patterns, monthly travel trends, and round-trip behavior.

The findings showed that Meeting was the most common identified trip purpose, October had the highest total travel distance, and Morrisville ↔ Cary was one of the most frequently used identifiable routes.

Overall, this project demonstrates the use of **Python, Pandas, Matplotlib, and Seaborn** to clean raw data, perform feature engineering, conduct exploratory data analysis, and generate meaningful business-oriented insights.

---

## 📁 Project Structure

```text
Uber-Drive-Data-Analysis/
│
├── UBERDRIVE.ipynb
├── uberdrive.csv
└── README.md
```

---

## ▶️ How to Run the Project

### 1. Clone the repository

```bash
git clone <your-github-repository-url>
```

### 2. Install the required libraries

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 3. Open Jupyter Notebook

```bash
jupyter notebook
```

### 4. Open

```text
UBERDRIVE.ipynb
```

### 5. Run the notebook cells

Make sure the dataset file is placed in the same project directory as the notebook.

---

## 👩‍💻 Author

**Cathrin Prasalya**

Data Analytics / Data Science Enthusiast

**Skills demonstrated in this project:**
Python • Pandas • NumPy • Matplotlib • Seaborn • Data Cleaning • Feature Engineering • EDA • Data Visualization
