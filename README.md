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
![Raw Data on bike customers](https://github.com/philoooo/Bike-Sales-Dashboard/blob/main/RawData_BikeData.PNG)
## Data Cleaning:
- **Using Excel Data Tools, I removed 26 duplicate rows.**
- **Then I used Find and Replce to clarified values:** In `Married Status` column:
  - `'M' → 'Married'`
  - `'S' → 'Single'`
- **And then:** in `Gender` column:
  - `'F' → 'Female'`
  - `'M' → 'Male'`
- **Next I added a new column called `Age Brackets`** to group ages so they could be better quantified for analysis:
  ```excel
  =IF(L2>55, "Old", IF(L2>=31, "Middle Age", IF(L2<31, "Adolescent", "Invalid")))
(Here, L2 is the original Age column)

![Cleaned Working Data](https://github.com/philoooo/Bike-Sales-Dashboard/blob/main/Working%20Data_BikeData.PNG)

📊 Pivot Tables & Charts
1. Average Income by Gender & Bike Purchase
Values: Average of Income.

Rows: Gender.

Columns: Bike Purchased (Y/N).

Chart: 2D Clustered Column with data table and color adjustments.
![First Pivot Table](https://github.com/philoooo/Bike-Sales-Dashboard/blob/main/PV1.PNG)

2. Commute Distance of Customers
Values: Count of Purchased Bikes.

Rows: Commute Distance.

Columns: Bike Purchased (Y/N).

Chart: Line chart with adjusted elements and color-blind-friendly palette.
![Formatted Pivot Tables](https://github.com/philoooo/Bike-Sales-Dashboard/blob/main/pv2.PNG)

3. Age Brackets of Customers
Values: Count of Purchased Bikes.

Rows: Age Brackets.

Columns: Bike Purchased (Y/N).

Chart: Line chart with styling adjustments.

![Formatted Pivot Tables](https://github.com/philoooo/Bike-Sales-Dashboard/blob/main/pv3.PNG)


## 📈 Dashboard
 First, I copied and arranged all three charts on a dedicated Dashboard sheet. I need to removed gridlines for a cleaner layout and add a header and title for the dashboard.
Once I coped in all 3 pivot tables, I aligned and formatted the charts for consistency. Then, I inserted slicers for filtering by: Married Status, Education, Region, and home ownership. I made sure to connect the slicers to all pivot tables for interactive filtering.

![Finsihed Bike Sales Dashboard](https://github.com/philoooo/Bike-Sales-Dashboard/blob/main/BikeDashboard.PNG)

## Reports and Findings

Income and Marital Status:
Married customers typically earn $4k–$9k more than their single counterparts.
The most significant gap—around $9k—is observed between single and married men who did not purchase a bike.
This suggests that single men are less likely to purchase bikes, potentially due to income differences.

Regional Insights:
Europe shows the smallest wealth gap between genders and marital statuses, while North America has the largest disparity.
This indicates that income is less of a deciding factor for bike purchases in Europe compared to other regions.

Age Trends:
Across all regions, middle-aged customers represent the largest group of bike purchasers.
In Europe, most customers who visit the shop end up buying a bike.

Commute Patterns:

In Europe, most customers have a short commute (0–1 miles).

In North America, commute distances are more evenly distributed.

In the Pacific region, customers typically have either a short (0–1 miles) or medium (5–10 miles) commute.

Homeownership:
Customers who do not own homes tend to have shorter commutes and are more likely to purchase bikes compared to homeowners.

Education Level:
There is a noticeable trend where customers with lower education levels purchase more bikes than those with higher education.
