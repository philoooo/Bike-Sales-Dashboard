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
## 🧹 Data Cleaning
- **The first thing I did was removed 26 duplicates** using Excel Data Tools.
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


📈 Dashboard
Copied and arranged all three charts on a dedicated Dashboard sheet.

Removed gridlines for a cleaner layout.

Added a header and title.

Aligned and formatted charts for consistency.

Inserted slicers for filtering by:

Married Status

Education

Region

Connected slicers to all pivot tables for interactive filtering.

![Finsihed Bike Sales Dashboard](https://github.com/philoooo/Bike-Sales-Dashboard/blob/main/BikeDashboard.PNG)

## 📝 Report Analysis

Married customers earn between ~$4k–9k more than their single counterparts.
The largest difference is among single vs. married men who did not purchase a bike, with a gap of $9k.
This suggests that single men are less likely to purchase bikes, potentially due to income differences.

Regional Insights:

Europe shows the smallest wealth gap between gender and marital status.
Income is less of a factor in bike purchases compared to North America, which has the greatest disparity.

Age Trends:
Across all regions, middle-aged customers are the largest group purchasing bikes.
In Europe, most customers entering the shop end up buying a bike.

Commute Patterns:

In Europe, most customers have a short commute (0–1 miles).

In North America, commute distances are more evenly distributed.

In the Pacific region, most customers have either a short (0–1 miles) or 5–10 miles commute.

Homeowners vs. Renters:
Customers who aren’t homeowners tend to have shorter commutes and are more likely to purchase bikes.

Education Level:
There’s a trend where customers with lower education levels purchase more bikes compared to those with higher education.
