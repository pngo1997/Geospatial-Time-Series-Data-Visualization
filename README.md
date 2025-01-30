# 🏗️ Geospatial & Time Series Data Visualization Project  

## 📜 Overview  
This project involves **geospatial analysis and time series visualization** using **R and Tableau**. It includes visualizations of **food service availability across U.S. counties**, **Chicago traffic crashes**, and **Portland water levels**, leveraging **mapping, time series smoothing, and custom color scales**.  

## 🎯 Problem Explanation  

### **1. U.S. Food Service Availability Analysis**
📌 Dataset: **FoodSrvcByCounty.txt**  
- **State-Level Food Services Visualization:**  
  - **Choropleth Map** displaying **food service availability** by state.  
  - Color scheme highlights states with **high vs. low food access**.  
  - **Patterns identified** in food service density.  
- **County-Level Food Services Visualization:**  
  - **Choropleth Map** at the **county level** for more granularity.  
  - Identifies **local disparities** in food availability.  
- **Extra Credit:**  
  - Implement a **cartogram visualization** to show state-level data **with area distortions**.  

📊 **Tools Used:** R, Tableau

### **2. Chicago Traffic Crashes**
📌 Dataset: **Chicago_crashes.csv**  
- **Crash Location Map:**  
  - **Geospatial scatter plot** of crash locations in Chicago.  
  - Uses **latitude & longitude data**.  
- **Crash Frequency by Time of Day:**  
  - **Visualization approach chosen:**  
    - **Heatmap**, **boxplot**, or **density plot** for **time-based trends**.  
  - **Findings explained:** What time of day sees the most crashes?  
  - Compares **daytime vs. nighttime crash density**.  

📊 **Tools Used:** Tableau, R  

### **3. Portland Water Level Time Series Analysis**
📌 Dataset: **Portland Water Level Data**  
- **Moving Average Smoothing:**  
  - Computes **moving average** to smooth hourly water level data (365×24 points).  
  - Experiments with different **window sizes**.  
- **Tidal Cycles Visualization:**  
  - **Overlapping time series plot, level plot, or horizon graph**.  
  - Captures **daily tidal fluctuations**.  
  - Identifies **cyclical tide behavior** without excessive clutter.  
- **Comparing Graphs:**  
  - **Single-paragraph analysis** of how each graph conveys information differently.  

📊 **Tools Used:** R, Tableau  

### **4. Custom Color Scale for Portland Water Level Data**
📌 Dataset: **Portland Water Level Data**  
- **Divergent Color Scale:**  
  - **Custom color gradient** for water levels:  
    - **Midpoint (average water level)** = Neutral color  
    - **High water levels** = Distinctive color 1  
    - **Low water levels** = Distinctive color 2  
  - Uses **HSV color space** for precise color selection.  
- **Color Scale Justification:**  
  - Explanation of why the chosen colors **enhance interpretation**.  

📊 **Tools Used:** R (ggplot2)  

---

## 🚀 Technologies Used  
- **R (ggplot2, sf, tmap)** – Mapping, time series analysis, color scales.  
- **Tableau** – Geospatial & time series visualization.  
- **D3.js (Extra Credit)** – Cartogram visualization.  

## 📊 Example Output  

### **1. Food Service Availability (Cartogram)**
🗺 **State-Level Food Service Availability**  
- This cartogram aims to emphasize the higher food services availability, the larger area of the states.
![Food Services Map](https://github.com/pngo1997/Images/blob/main/VS2%20-%20Cartogram%20food%20availability.png)  

---

### **2. Chicago Traffic Crashes (Scatterplot)**
🚗 **Crash Frequency by Time of Day**  
- Six plots side-by-side given each plot represents reported traffic incidents through different times of the date based on brightness level.
- Using attribute Lightning Condition - light condition at time of crash as determined by reporting officer for grouping, the visual allows viewers to decoded the data message following the graph's objective, common crashes in different parts of the city
 based on time of day. With this, the big graph is able to convey the data story, also clear enough that viewers can observe and analyze the data differences. If all data points were all in one graph and separated by colors, then it will create confusion due to high points
 density. 
- Overall, same pattern across all six maps which is downtown Chicago has the most traffic accidents, then scattered around surrounding areas. Noticeably, majority of incidents happened during the day (Daylight), followed by Darkness, lighted road lightning condition. These are rush hours, high-traffic time frame when people commute to and back from work.
![Crash Heatmap](https://github.com/pngo1997/Images/blob/main/VS2%20-%20Heatmap%20chicago%20traffic.png)  

---

### **3. Portland Water Levels (Smoothed Time Series - Line Chart)**
🌊 **Monthly Moving Average (including current month) of Water Levels** 
- The graph represents Monthly Moving Average of Water Level in Portland (2003) including current month data in moving average calculation.
- The black line represent average water level of every month, considering water level were re-calculated as moving average with previous two hours.
- Three smoothing lines represents different moving average methods. Overall, moving average includes all previous months yields the most smoothed line. While moving average consider the previous 2-3 months shows a light increase in September.
- The graph holds expectation that there is a light drop in December due to insufficient data of the month.
![Water Level Graph](https://github.com/pngo1997/Images/blob/main/VS2%20-%20Line%20chart%20monthly%20water%20moving.png)  

---

### **4. Custom Color Scale (Divergent Gradient - Horizon Graph)**
🎨 **Water Level Divergent Color Scale**  
- The diverge in color indicates which days have higher or lower average water levels compared to other days across the months.
- Overall, the graph shows that period between 18th and 21st has much lower water level compared to the rest of the dates, slight drop in the 5th date as well. On the other hand, higher water level at mid-month during 13rd to 16th. There are still tidal signs shown in these dates. The general trend is that the water level gradually decreases from the beginning of the month to the
 12th, fluctuates slightly from the 8th to the 11th, then increases sharply from the 12th to the 10th, then gradually decreases until the end of the month.
![Color Scale](https://github.com/pngo1997/Images/blob/main/VS2%20-%20Divergent%20color%20scale%20water%20level.png)  
