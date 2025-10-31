# Electric Vehicle Population Data Analysis

This project analyzes the electric vehicle population dataset using Python and various data-visualization tools.  
It covers data cleaning, exploratory data analysis (EDA), and interactive visualizations.

## 📁 Project Overview

- **Dataset**: Electric Vehicle Population Data (CSV)  
- **Tools & Libraries**:  
  - `pandas`, `numpy` for data manipulation  
  - `matplotlib`, `seaborn` for static visualizations  
  - `plotly.express` for interactive charts  
  - `folium` for map visualization (if latitude/longitude available)  
- **Platform**: Executed in a Google Colab notebook  
  - [Notebook link](https://colab.research.google.com/drive/19LkIP0BQaePBzRErdiYhQOL6Tgr4qmxC)  

## ✅ Key Steps in the Analysis

1. **Import libraries** and configure environment (suppressing warnings, etc.)  
2. **Load dataset** into a DataFrame and inspect its basic information (shape, dtypes, head).  
3. **Check unique values** per column to understand dataset composition.  
4. **Missing values analysis** – visualize percentage of missing values and heatmap of null entries.  
5. **Data cleaning** – drop rows where critical fields (`Electric Range`, `Postal Code`) are missing.  
6. **Correlation analysis** – compute correlations among numeric columns and display a heatmap.  
7. **City-wise analysis** – identify top cities by vehicle count; create pie chart and log-scale histogram.  
8. **Model analysis** – identify top EV models and visualize them using bar plots.  
9. **City vs Model Year** – compare latest model years across top cities.  
10. **Base MSRP distribution** – interactive histogram showing pricing distribution (log scale).  
11. **Electric Utility distribution** – interactive histogram of which utilities serve EVs.  
12. **Electric Range vs CAFV eligibility** – histogram showing range by eligibility for clean alternative fuel vehicle programs.  
13. **County-wise distribution** – bar chart of counts by county.  
14. **Interactive scatter plot** – sample of VIN vs legislative district, colored by vehicle type.  
15. **Optional Folium map** – if vehicle location coordinates available, show markers on a map and save as `ev_map.html`.

## 🛠 Getting Started

1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/<your-repo>.git
Open the notebook:

bash
Copy code
electric_vehicle_population_analysis.ipynb
Ensure you have the required libraries installed. You can install via:

bash
Copy code
pip install pandas numpy matplotlib seaborn plotly folium
Run the notebook cell by cell and inspect the visual output.

📊 What You Will Learn
How to handle large datasets (260k+ rows) efficiently

Techniques for cleaning real-world data (missing values, invalid entries)

How to compute and interpret correlations in numeric data

How to use static and interactive visualizations to derive insights

How to map geospatial data (if available) using Folium

How to sample and visualize subsets of data to maintain performance

🔍 Insights & Highlights
There is a strong negative correlation between Model Year and Electric Range (i.e., older model years often have higher range)

The Base MSRP has a wide distribution and is better visualized on a log scale

A few cities dominate the EV population, revealing geographic clustering

Certain electric utilities serve a disproportionate share of EVs

(These are example insights — you should interpret your actual results from the notebook.)

✅ License
This project is released under the MIT License – feel free to use, modify and distribute.

