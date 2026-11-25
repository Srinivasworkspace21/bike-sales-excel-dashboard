# Bike Sales Excel Dashboard

An interactive Excel dashboard that explores which customers buy bikes,
built as a guided project and extended with my own analysis.

## Objective
Find out which customer characteristics (income, commute distance, age,
cars owned, number of children) are linked to buying a bike.

## Dataset
Excel Project Dataset.xlsx from the Excel-Tutorial repository by
Alex The Analyst (guided project):
https://github.com/AlexTheAnalyst/Excel-Tutorial

The raw file had 1,026 rows. After cleaning, 1,000 rows remain.

## Tools used
Microsoft Excel: data cleaning, nested IF formulas, pivot tables,
pivot charts, slicers

## Steps
1. Worked on a copy of the downloaded dataset so the original stays intact
2. Removed 26 duplicate records (1,026 rows down to 1,000)
3. Standardised labels using Find and Replace:
   M/S became Married/Single and M/F became Male/Female
4. Renamed the longest commute category to "More than 10" for cleaner
   sorting
5. Created an Age Brackets column with nested IF formulas:
   Adolescent (under 31), Middle Age (31 to 54), Old Age (over 54)
6. Built 5 pivot tables:
   - Average income by gender and bike purchase
   - Commute distance vs bike purchase
   - Age bracket vs bike purchase
   - Cars owned vs bike purchase (% of row total)
   - Number of children vs bike purchase (% of row total)
7. Turned each pivot table into a chart
8. Built the dashboard: removed gridlines and arranged the 5 charts
9. Added a headline cell showing the overall purchase rate (48.1%)
10. Added 5 slicers (Marital Status, Education, Region, Cars, Children)
    and connected each one to all pivot tables, so a single click
    filters the whole dashboard

## Key findings
1. The overall purchase rate is 48.1% (481 of 1,000 customers).
2. Customers with no car bought a bike 61.1% of the time, compared with
   35.6% to 38.8% for customers with 2 or more cars.
3. Customers with 5 children had the lowest purchase rate (22.2%),
   compared with 42.9% to 57.4% for customers with 0 to 4 children.
4. Middle Age customers were the largest buying group: 383 of 701 bought
   a bike (54.6%), compared with 35.5% of Adolescents and 31.2% of
   Old Age customers.
5. Shorter commutes go with higher purchase rates: 54.6% for 0 to 1
   miles and 58.6% for 2 to 5 miles, against 29.7% for more than 10
   miles.

## What I changed or added myself
- Added two extra pivot tables and charts: Cars vs Purchased Bike and
  Children vs Purchased Bike, shown as percentage of row total
- Added two extra slicers (Cars and Children) and connected all five
  slicers to all charts
- Used the slicers to look at a specific group: customers with 1 or more
  cars and 4 children. This group has 98 people, of whom 40 bought a
  bike (40.8%), slightly below the overall rate of 48.1%
- Added the overall purchase rate as a headline number

## Limitations
Some groups are small, and these results show patterns in this dataset,
not proof of cause. For example, owning more cars does not by itself
explain why someone did not buy a bike.

## How to use
Open `Excel Project Dataset - Copy.xlsx` in Excel and go to the Dashboard sheet.
Click any slicer option to filter all charts. Use the Clear Filter icon
on each slicer to reset.

- `Excel Project Dataset - Copy.xlsx`: final workbook (data, pivot tables, dashboard)
- `README.md`: project description
