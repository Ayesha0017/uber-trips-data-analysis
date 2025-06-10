# 🚕 Uber Trips Data Analysis

This project explores and analyzes Uber trip data to uncover trends and patterns in ride behavior, mileage, and temporal usage. It uses Python, pandas, matplotlib, seaborn, and scikit-learn to preprocess the data, visualize insights, and prepare features for further modeling or reporting.

---

## 📁 Dataset

The dataset contains records of Uber trips with the following columns:
- `START_DATE`: Trip start date and time
- `END_DATE`: Trip end date and time
- `CATEGORY`: Category of trip (e.g., Business, Personal)
- `PURPOSE`: Purpose of the trip (e.g., Meeting, Airport)
- `MILES`: Distance traveled in miles

---

## 🧹 Data Cleaning

- Parsed and converted `START_DATE` and `END_DATE` into `datetime` format using `pd.to_datetime` with error handling.
- Identified and handled missing or unparsable values.
- Extracted the **month** from the `START_DATE` for monthly analysis.

---

## 📊 Visualizations

- Created line plots to compare:
  - Total number of rides per month
  - Maximum miles traveled per month
  - which date has most count of rides
  - Months vs value counts 
  - Count of category, purpose the cabs were used for
  - The time(day-night) when the cabs were most used

- Used `seaborn` for clear, aesthetic plots.
- Handled month labeling using a custom dictionary:
  ```python
  month_label = {
      1: "Jan", 2: "Feb", 3: "Mar", 4: "Apr",
      5: "May", 6: "Jun", 7: "Jul", 8: "Aug",
      9: "Sep", 10: "Oct", 11: "Nov", 12: "Dec"
  }
