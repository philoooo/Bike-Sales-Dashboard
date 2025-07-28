# Bike-Sales-Dashboard
#Created4 Excel sheets. 1. Raw data 2. Working Data 3. Pivot Table 4. Dashboard
#Data cleaning
#Removed 26 duplicates using data tools
#Using find and replace to clarify values in Married Status column from 'M' and 'S' to 'Married' and 'Single'
#Using Find and Replace, claridy values in Gender column from 'F' and 'M" to "Female' and 'Male'
#Insert new column called "Age Brackets" to better quantify age for data analysis. Using nested IF function "=IF(L2>55,"Old",IF(L2>=31,"Middle Age",IF(L2<31,"Adolescent","Invalid")))" using prior Age column "L2"

#Create Pivot Table and charts
#First Pivot table  will  be showing Average Income and Gender of Bike Purchasers. values is the averageo the income column, gender is rows and Bike Purchased(Y/N) is columns. 
#Second Pivot table will be showing the commutes of customers in the bike shop. the vales is the count of purchased bikes, the column is the purchased bikes(No or Yes) and the rows in the commute distance. 
#Third pivot table will be showing the age range of the bike shop customers. the vales is the count of purchased bikes, the column is the purchased bikes(No or Yes) and the rows is the age brackets column

#From first pivot table, creared 2D cluster column chart, adjusted chart elements, add data table. 
#From second pivot table, create line chart, adjusting chart elements. 
#From the third pivot table, i created another line chart, adjusting chart elements. 
#changed chart colors to for colorblindness. 

#Dashboard
#Copied 3 charts
#Removed gridlines
#Create header and dashboard title
#align format of charts from top
#insert slicer analysing married status, education, region. reporting connections for all pivot tables. 



#Report Analysis:
#Married customers are making between ~4-9k more than their single counterparts. The greatest differce is between single and married men who don't purchase a bike, the value being an 9k. This shows that single men are a lot less likley to purchase a bike from the shop, correlating to their income status. 
#Customers in Europe have the smallest wealth disparity between gender as well as marital status, with North America having the greatest. This means that income is less of a factor for a customer in Europe to not purchase a bike. 
#All regions show same trend where middle aged customers are the largest customer base that in the shops that purchase bikes. In Europe, the more often than not a customer will go into a the shop and purchase a bike. 
#In Europe, most customers have a short commute 0-1miles, in north america it is distribute roughly evenly, and in pacific people tend to have a short 0-1 mile or 5-10 mile commute. 
#Customers that aren't home owners tend to have a shorter commute, and also purchase bikes more often then home owners.
#General trend where people with lower education tend to buy buy more bikes then people with higher education. 
# 🚴 Bike Sales Dashboard

This project analyzes customer demographics and purchasing patterns for a bike shop using Excel. It includes **data cleaning**, **pivot table analysis**, and an interactive **dashboard** for visualization.

---

## 📂 Project Structure
The Excel workbook includes four sheets:
1. **Raw Data** – Original dataset.
2. **Working Data** – Cleaned and pre-processed data.
3. **Pivot Tables** – Pivot tables summarizing key insights.
4. **Dashboard** – Visual dashboard built from pivot charts.

---

## 🧹 Data Cleaning
- **Removed 26 duplicates** using Excel Data Tools.
- **Clarified values** in `Married Status` column:
  - `'M' → 'Married'`
  - `'S' → 'Single'`
- **Clarified values** in `Gender` column:
  - `'F' → 'Female'`
  - `'M' → 'Male'`
- **Added new column `Age Brackets`** to group ages:
  ```excel
  =IF(L2>55, "Old", IF(L2>=31, "Middle Age", IF(L2<31, "Adolescent", "Invalid")))
(Here, L2 is the original Age column)

📸 [Insert screenshot of cleaned Working Data here]

📊 Pivot Tables & Charts
1. Average Income by Gender & Bike Purchase
Values: Average of Income.

Rows: Gender.

Columns: Bike Purchased (Y/N).

Chart: 2D Clustered Column with data table and color adjustments.

📸 [Insert screenshot of pivot table & chart]

2. Commute Distance of Customers
Values: Count of Purchased Bikes.

Rows: Commute Distance.

Columns: Bike Purchased (Y/N).

Chart: Line chart with adjusted elements and color-blind-friendly palette.

📸 [Insert screenshot of pivot table & chart]

3. Age Brackets of Customers
Values: Count of Purchased Bikes.

Rows: Age Brackets.

Columns: Bike Purchased (Y/N).

Chart: Line chart with styling adjustments.

📸 [Insert screenshot of pivot table & chart]

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

📸 [Insert screenshot of full dashboard]

📝 Report Analysis
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
