# 🚖 Uber Drive Data Analysis

## 📌 Project Overview

This project analyzes Uber ride data using Python to uncover travel patterns, ride behavior, customer purposes, and operational insights through Exploratory Data Analysis (EDA).

The project demonstrates data cleaning, feature engineering, visualization, and business insight generation using real-world Uber trip data.

---

## 🎯 Objectives

- Clean and preprocess Uber trip data.
- Perform exploratory data analysis.
- Identify ride trends and travel behavior.
- Generate business insights through visualizations.
- Improve decision-making using data-driven findings.

---

## 📂 Dataset

The dataset contains Uber trip information including:

- Start Date
- End Date
- Category
- Start Location
- Stop Location
- Miles
- Purpose

---

## 🛠 Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## 📊 Data Preprocessing

The following preprocessing steps were performed:

- Removed duplicate records
- Handled missing values
- Converted date columns to datetime format
- Created new features such as:
  - Month
  - Day
  - Hour
  - Weekday
  - Ride Duration
  - Round Trip Indicator

---

## 📈 Exploratory Data Analysis

The analysis answers the following business questions:

- Weekday vs Weekend ride distribution
- Round trip analysis
- Total miles travelled by category
- Monthly ride trends
- Most common starting locations
- Busiest time of the day
- Top ride purposes
- Longest and shortest rides
- Monthly total miles travelled
- Average rides by weekday
- Locations with the highest round trips
- Average distance by time of day
- Rides starting and ending at the same location
- Purpose with the highest average ride distance
- Most common start-stop route combinations
- Average time gap between rides

---

## 📌 Key Insights

- Business trips account for the majority of rides.
- Weekday rides are more frequent than weekend rides.
- Certain locations consistently generate the highest ride volume.
- Morning and evening hours are the busiest periods.
- Business purposes contribute significantly to total travel distance.

---

## 📷 Visualizations

The project includes various visualizations such as:

- Bar Charts
- Count Plots
- Pie Charts
- Histograms
- Line Charts
- Box Plots

---

## 📁 Project Structure

```
Uber-Drive-Data-Analysis/
│
├── Uber_Drive_Data_Analysis.ipynb
├── UberDataset.csv
├── README.md

```

---

## ▶️ How to Run

1. Clone this repository.
2. Install the required libraries.

```bash
pip install pandas numpy matplotlib seaborn
```

3. Open the Jupyter Notebook.

```bash
jupyter notebook
```

4. Run all cells sequentially.

---

## 📚 Skills Demonstrated

- Data Cleaning
- Feature Engineering
- Exploratory Data Analysis
- Data Visualization
- Business Insight Generation
- Python Programming
- Data Analytics

---

## 👩‍💻 Author

**Cathrin**

Aspiring Data Analyst

---

## ⭐ Future Improvements

- Build an interactive Power BI dashboard.
- Create a Streamlit web application.
- Add predictive analytics using Machine Learning.
- Deploy the project online.
