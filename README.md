# 🚕 Uber NYC Trip Analysis

An exploratory data analysis project on Uber trip data from New York City to understand trip demand patterns across **time, weekdays, hours, dispatching bases, and geographic locations**.

The project uses Python-based data analysis and visualization techniques to identify patterns in Uber activity and visualize high-demand areas across NYC.

---

## 📌 Project Overview

This project analyzes Uber trip data to answer questions such as:

- Which month has the highest number of Uber pickups?
- How does Uber demand vary across weekdays?
- What are the hourly rush patterns in New York City?
- Which dispatching bases have the most active vehicles?
- Which locations in NYC experience the highest concentration of pickups?
- How does trip demand vary across different hours and days?

The analysis follows a complete data-analysis workflow:

**Data Collection → Data Cleaning → Feature Engineering → Exploratory Data Analysis → Visualization → Geographic Analysis**

---

## 🛠️ Technologies Used

- **Python**
- **Pandas** – Data manipulation and analysis
- **NumPy** – Numerical operations
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical visualization
- **Plotly** – Interactive visualizations
- **Folium** – Geographic visualization and heatmaps
- **Jupyter Notebook**

---

## 📂 Dataset

The project uses Uber New York City trip data containing information such as:

- Pickup date/time
- Pickup latitude
- Pickup longitude
- Dispatching base
- Active vehicles

The notebook works with multiple Uber trip-data CSV files and combines them for analysis.

> **Note:** The raw dataset is not included in this repository. Download the dataset separately and place the required CSV files inside the `data/` directory.

---

## 🔍 Analysis Performed

### 1. Data Cleaning

The dataset was inspected for:

- Duplicate records
- Missing values
- Incorrect data types

Duplicate records were removed and timestamp columns were converted into appropriate datetime formats.

---

### 2. Time-Based Analysis

The pickup timestamp was used to create additional features:

- Month
- Weekday
- Day
- Hour
- Minute

These features were then used to analyze Uber demand patterns over different time periods.

---

### 3. Monthly Trip Analysis

The project analyzes the number of Uber pickups across different months to identify periods with higher trip demand.

A bar chart is used to visualize monthly pickup activity.

---

### 4. Weekday Analysis

A month-vs-weekday cross-tabulation is created to examine how Uber pickup activity changes across different days of the week and months.

---

### 5. Hourly Rush Analysis

Hourly trip demand is analyzed across different weekdays.

A Seaborn point plot is used to visualize how Uber activity changes throughout the day and to identify periods of higher demand.

---

### 6. Dispatching Base Analysis

The `Uber-Jan-Feb-FOIL.csv` dataset is analyzed to understand the distribution of active vehicles across different dispatching bases.

An interactive **Plotly box plot** is used to visualize active-vehicle distributions by dispatching base.

---

### 7. NYC Pickup Hotspot Analysis

Pickup coordinates (`Lat`, `Lon`) are grouped to identify locations with higher concentrations of Uber pickups.

A **Folium HeatMap** is then created to visualize geographic pickup hotspots across New York City.

---

### 8. Pairwise Day & Hour Analysis

The project also examines the relationship between:

- Day of the month
- Hour of the day

A pivot table with background gradients is generated to make high-activity periods easier to identify.

---

## 📊 Visualizations

The project includes several types of visualizations:

- 📈 Monthly pickup distribution
- 📊 Month vs. weekday analysis
- ⏰ Hourly rush analysis
- 🚗 Active vehicles by dispatching base
- 🗺️ NYC pickup heatmap
- 📅 Day vs. hour demand analysis

---

## 📁 Project Structure

```text
Uber-Trip-Analysis/
│
├── uber_trip_analysis.ipynb
├── README.md
├── requirements.txt
│
├── data/
│   └── README.md

