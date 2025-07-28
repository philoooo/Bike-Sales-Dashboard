# 🚴 Bike Sales Dashboard Using Excel

This project analyzes customer demographics and purchasing patterns for a bike customers using Excel. It includes **data cleaning**, **pivot table analysis**, and an interactive **dashboard** for visualization.

---

## 📂 Project Structure
The Excel workbook includes four sheets:
1. **Raw Data** – Original dataset.
2. **Working Data** – Cleaned and pre-processed data.
3. **Pivot Tables** – Pivot tables summarizing key insights.
4. **Dashboard** – Visual dashboard built from pivot charts.

---
**Raw Data**
![Raw Data on bike customers](https://github.com/philoooo/Bike-Sales-Dashboard/blob/main/RawData_BikeData.PNG)
## Data Cleaning:
1. **Using Excel Data Tools, I removed 26 duplicate rows.**
2. **Used Find and Replce to clarify value names:**
  - **In the `Married Status` column:**
       - `'M' → 'Married'`
       - `'S' → 'Single'`
  - **In the `Gender` column:**
       - `'F' → 'Female'`
       - `'M' → 'Male'`
3. **Added a new column called `Age Brackets` using nested functions** Grouped ages so they could be better quantified for analysis, where L2 is the original Age column.:
  ```excel
  =IF(L2>55, "Old", IF(L2>=31, "Middle Age", IF(L2<31, "Adolescent", "Invalid")))
  ```

**Cleaned Working Data**
![Cleaned Working Data](https://github.com/philoooo/Bike-Sales-Dashboard/blob/main/Working%20Data_BikeData.PNG)

---
## Pivot Tables & Charts
1. First Pivot Table explores the Average Income by Gender & Bike Purchase
Values: Average of Income.
Rows: Gender.
Columns: Bike Purchased (Y/N).

Chart: 2D Clustered Column with data table. (All charts used colorblind-safe palette to ensure accessibility)
![First Pivot Table](https://github.com/philoooo/Bike-Sales-Dashboard/blob/main/PV1.PNG)

2. Second Pivot Table explores the Commute Distance of Customers
Values: Count of Purchased Bikes.
Rows: Commute Distance.
Columns: Bike Purchased (Y/N).

Chart: Line chart with adjusted elements.
![Second Pivot Table](https://github.com/philoooo/Bike-Sales-Dashboard/blob/main/PV1.PNG) 

3. Third Pivot Table explores the Age Brackets of Customers
Values: Count of Purchased Bikes.
Rows: Age Brackets.
Columns: Bike Purchased (Y/N).

Chart: Line chart with styling adjustments.
![Third Pivot Table](https://github.com/philoooo/Bike-Sales-Dashboard/blob/main/pv3.PNG)

---

## Dashboard
To assemble my dashboard, I copied and arranged all three charts on a dedicated Dashboard sheet. I need to removed gridlines for a cleaner layout and add a header and title for the dashboard.
Once I coped in all 3 pivot tables, I aligned and formatted the charts for consistency. Then, I inserted slicers for filtering by: Married Status, Education, Region, and home ownership. I made sure to connect the slicers to all pivot tables for interactive filtering.

![Finsihed Bike Sales Dashboard](https://github.com/philoooo/Bike-Sales-Dashboard/blob/main/BikeDashboard.PNG)

---

## Findings

- **Income & Marital Status**: Married customers typically earn **$4k–$9k more** than single customers. Single men who did not purchase a bike show the largest gap, around **$9k**, indicating income may affect their likelihood of buying a bike.  
- **Regional Insights**: **Europe** has the smallest income gap between genders and marital statuses, while **North America** shows the largest disparities.  
- **Age Trends**: **Middle-aged customers** are the dominant group of bike purchasers across all regions, and in Europe, most customers who enter the store end up purchasing a bike.  
- **Commute Patterns**: Commutes vary by region—**short commutes (0–1 miles)** are common in Europe, while the Pacific region sees a mix of **0–1 miles** and **5–10 miles**.  
- **Homeownership**: Non-homeowners tend to have **shorter commutes** and are **more likely to purchase bikes** compared to homeowners.  
- **Education Level**: Customers with **lower education levels** buy more bikes compared to those with higher education.

---

## Reports

- **Sales Overview**: A breakdown of income, gender, and marital status reveals which groups purchase bikes most often.  
- **Trend Analysis**: Pivot tables highlight age group preferences, commute distances, and regional purchasing patterns.  
- **Customer Insights**: Insights into how factors like homeownership, education level, and income affect bike purchase behavior.

---

## Conclusion

This project demonstrates how Excel can be used for **data cleaning, pivot table analysis, and dashboard building** to uncover customer trends. The findings—like the connection between income, age, and bike purchasing behavior—could help a bike shop better target its marketing and sales strategies. The interactive dashboard and slicers make it easy to explore patterns and gain actionable insights.
