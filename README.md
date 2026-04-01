Overview
This Power BI report (dashboard.pbix) is a Sales Performance Dashboard built on a dataset named hero. It provides an end-to-end view of sales, profit, and shipping metrics across customers, regions, product categories, and time. The report was created in Power BI Desktop (release 2025.11) and contains 2 pages.

Report Pages
Page 1 — Sales & Profit Overview
The main analytical page. It includes the following visuals:
Visual TypeTitle / DescriptionFields UsedLine & Stacked Column Combo ChartProfit Margin of each StateState, Sum of ProfitPie ChartSales by SegmentSegment, Sum of SalesArea ChartTop 5 Customer Sales OverviewCustomer Name, Sum of SalesClustered Bar ChartShipping Days by Ship ModeShip Mode, Avg Shipping DaysLine ChartAverage of Sales by CategoryOrder Date (Year/Quarter/Month), Sum of Sales, CategoryCard VisualsKPI summaryTotal Profit, Total Sales, Sum of Profit MarginSlicerFilter by RegionRegionSlicerFilter by Order DateYear, Quarter, Month, DayImagesBranding / Logo assets—
Page 2 — Profit Margin Detail
A focused page for drilling into profit margin by geography:
Visual TypeTitle / DescriptionFields UsedCard VisualProfit MarginSum of Profit MarginSlicerFilter by CountryCountryShapeDecorative element—

Data Model
The report is powered by a single table named hero with the following known columns and measures:
Dimensions

State
Region
Country
Segment
Category
Ship Mode
Customer Name
Order Date (with date hierarchy: Year → Quarter → Month → Day)

Measures / Calculated Fields

Total Sales
Total Profit
Profit Margin (Sum)
Avg Shipping Days


The data appears to be based on a retail/e-commerce sales dataset (similar in structure to the Superstore dataset). Static image resources embedded in the report reference Zomato branding, suggesting the dashboard may be part of a food-delivery or restaurant analytics project.


Technical Details
PropertyValueFile format.pbix (Power BI Desktop)Power BI release2025.11File size~881 KBNumber of pages2Data sourceEmbedded (hero table, imported model)ThemeCY25SU11 (default 2025 theme)Auto-detected relationshipsNone (manually defined)

How to Open

Install Power BI Desktop (free).
Open dashboard.pbix via File → Open report.
Use the Region and Order Date slicers on Page 1, or the Country slicer on Page 2, to filter the data.


Publishing to Power BI Service

Sign in to your Power BI account in Desktop.
Click Home → Publish.
Select your target workspace and click Select.
Once published, share the report URL or embed it using the Embed option in the Power BI Service.


Notes

The data model is embedded directly in the file — no external data source connection is required to view the report.
To refresh with new data, replace or update the hero table via Home → Transform Data in Power BI Desktop.
