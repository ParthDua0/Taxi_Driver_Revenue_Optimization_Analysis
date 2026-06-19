# NYC Taxi Revenue Analytics

## Overview

This project analyzes over 6 million NYC Yellow Taxi trips to identify revenue drivers, demand patterns, customer behavior, tipping trends, and operational insights.

The analysis combines Python-based data cleaning, feature engineering, exploratory data analysis, statistical testing, and Power BI dashboard development to generate actionable business recommendations.

---

## Dataset

Source: NYC TLC Yellow Taxi Trip Records (January 2020)

Raw Dataset Size:

* 6.4+ million records

Final Cleaned Dataset:

* 6.3+ million records after data cleaning and validation

---

## Project Workflow

### 1. Data Cleaning

* Removed duplicate records
* Removed trips with:

  * Zero or negative fare amounts
  * Zero or negative trip distances
  * Zero or negative trip durations
* Handled missing values
* Validated feature consistency

### 2. Feature Engineering

Created:

* Trip Duration
* Pickup Hour
* Pickup Weekday
* Pickup Month
* Pickup Date
* Tip Percentage
* Distance Bucket
* Duration Bucket
* Time Period Categories

### 3. Exploratory Data Analysis

Analyzed:

* Revenue patterns
* Demand patterns
* Distance trends
* Duration trends
* Passenger behavior
* Tipping behavior

### 4. Statistical Testing

#### Independent T-Test

Objective:

Determine whether tipping behavior differs significantly across payment methods.

Result:

* P-value < 0.001
* Reject Null Hypothesis

Conclusion:

Card payments generate significantly higher tips than cash payments.

#### One-Way ANOVA

Objective:

Determine whether revenue differs across time periods.

Result:

* P-value < 0.001
* Reject Null Hypothesis

Conclusion:

Revenue differs significantly across time periods.

---

## Power BI Dashboard Pages

### Page 1 – Executive Overview

* KPI Summary
* Daily Revenue Trend
* Daily Demand Trend
* Revenue by Weekday
* Revenue by Hour
* Revenue by Distance Bucket

### Page 2 – Revenue Optimization

* Revenue by Hour
* Average Revenue by Hour
* Revenue by Distance Bucket
* Average Revenue by Distance Bucket
* Revenue by Duration Bucket
* Average Revenue by Duration Bucket

### Page 3 – Tip Analytics

* Average Tip by Hour
* Average Tip by Payment Type
* Average Tip by Distance Bucket
* Average Tip by Duration Bucket
* Average Tip by Passenger Count

### Page 4 – Passenger & Customer Behavior

* Revenue by Passenger Count
* Average Revenue by Passenger Count
* Trips by Passenger Count

### Page 5 – Statistical Analysis

* Correlation Matrix
* Fare vs Tip Analysis
* Statistical Testing Results

---

## Key Insights

### Revenue

* Peak revenue occurs around 6 PM.
* Friday generates the highest overall revenue.
* Longer trips generate significantly higher average revenue.

### Demand

* Most trips occur during evening hours.
* Short-distance trips dominate demand volume.
* Typical trip duration is between 10 and 20 minutes.

### Tipping

* Card payments generate substantially higher tips.
* Tip amounts increase with trip distance.
* Tip amounts increase with trip duration.

### Customer Behavior

* Single-passenger rides dominate demand.
* Large passenger groups are relatively rare.
* Passenger count has minimal influence on revenue generation.

---

## Business Recommendations

1. Increase driver availability during evening peak hours.

2. Encourage digital payment adoption to improve tipping outcomes.

3. Prioritize service quality for long-distance routes where revenue and tipping potential are highest.

4. Optimize fleet allocation around high-demand operational periods.

5. Focus operational efficiency on short-distance high-volume trips.

---

## Tools Used

### Python

* Pandas
* NumPy
* Matplotlib
* Seaborn
* SciPy

### Business Intelligence

* Power BI

### Development

* Jupyter Notebook
* Git
* GitHub

---

## Project Structure

data/
├── raw/
├── cleaned/

 nyc_taxi_analysis.ipynb

powerbi/
├── NYC_Taxi_Revenue_Analytics.pbix

reports/
├── project_report.txt

README.md
requirements.txt

---

## Author

Parth Dua

Aspiring Data Analyst | SQL | Python | Power BI | Tableau
