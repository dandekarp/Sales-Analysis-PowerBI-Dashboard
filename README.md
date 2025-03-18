✨ Project Overview

This Power BI portfolio project demonstrates an end-to-end implementation of a dynamic performance dashboard for Plant Co., showcasing advanced data visualization, DAX measure development, and professional report design. The dashboard enables quick analysis of sales performance, profitability metrics, and account segmentation with powerful interactive features.
🚀 Key Features
Dynamic Metrics & Comparisons

Switch Measures for toggling between Sales, Quantity, and Gross Profit
YTD vs. Prior YTD analysis with variance calculations
GP% (Gross Profit Percentage) calculations across all dimensions

Advanced Visualizations

📊 Multi-card KPI dashboard with conditional formatting
📉 Bottom 10 Countries bar chart highlighting underperforming regions
🌊 Waterfall chart breaking down performance by Month-Country-Product
📈 Line/Column combo chart showing YTD & PYTD by product type (Indoor, Landscape, Outdoor)
🔍 Scatter plot for Account Profitability Segmentation

Professional Design

Clean, minimalist layout with custom background
Consistent color scheme with conditional formatting
Dynamic titles and informative labels
Harmonious spacing and alignment

💡 Implementation Highlights
Data Model

Star schema with fact and dimension tables
Custom date dimension for time intelligence
Product hierarchy for drill-down analysis
Account dimension for customer segmentation

DAX Measures
Copy// Example Switch Measure
Switch Measure = 
VAR SelectedValue = SELECTEDVALUE(Values[Value], "Gross Profit")
RETURN
SWITCH(
    TRUE(),
    SelectedValue = "Sales", [Sales],
    SelectedValue = "Quantity", [Quantity],
    SelectedValue = "Gross Profit", [Gross Profit]
)
Business Value

Rapid identification of underperforming regions (Canada, Germany, Japan showing largest declines)
Clear visualization of seasonal trends across quarters
Strategic account segmentation for targeted sales efforts
Product type performance comparison

🛠️ Technologies Used

Power BI Desktop
DAX for measure creation
Power Query for data transformation
PowerPoint for background design

📚 Repository Structure

data/ - Source and processed data files
src/ - Power BI files and DAX scripts
documentation/ - Detailed implementation guides
assets/ - Background designs and screenshots
tutorials/ - Step-by-step recreation guides

📊 Visualization Preview
The dashboard highlights Plant Co.'s 2024 performance with YTD Gross Profit of 1.40M, showing a slight decrease of 77.62K compared to prior year. It identifies underperforming countries and provides account profitability segmentation for strategic decision-making.
🔗 Getting Started

Clone this repository
Open the PBIX file in Power BI Desktop
Explore the data model, measures, and visualizations
Follow tutorials to understand implementation details
