# Personal_Finance_Tracker

## Project Structure & Workflow
This Excel-based project follows a 3-layer architecture:

📑 Dataset (Dataset sheet): Contains raw monthly records of income and expenses
📊 Pivot Analysis (Calculations sheet): Builds dynamic Pivot Tables for summarization
📈 Dashboard Layer (Dashboard sheet): Visualizes insights using charts, cards, and graphs

## Dataset Description
The dataset used in this project captures real-life finance entries across various categories:

Date : Date of the transaction (dd-mm-yyyy)
Type :	Income or Expense
Category :	Spending/earning category (e.g. Housing, Job)
Amount :	Transaction amount
Day :	Weekday name (Mon, Tue, etc.) for trend analysis
Month :	Month name (Jan, Feb, etc.) for trend charts

## Feature Engineering (Excel Formula-Based)
To enhance analysis and build insightful visualizations, we performed feature extraction from the raw Date column:

Month	=TEXT(A2, "mmm")	Extracts 3-letter month name from Date
Day	=TEXT(A2, "ddd")	Extracts weekday name (Mon, Tue, etc.) from Date

These transformations helps:

  • Monthly trend visualization
  • Weekday pattern analysis
  • Dynamic grouping in PivotTables

## Pivot Table Analysis Layer
The Calculations sheet is dedicated to:

  • Creating Pivot Tables for income and expense aggregation
  • Calculating KPIs like total income, total spending, available balance
  • Deriving monthly and weekly trends
  • Feeding structured results into the dashboard using linked cells


### Key Dashboard Metrics

💰 Available Balance	$35,249
📥 Total Income	$65,440
📤 Total Spending	$30,191
🧾 Max Income Source	Data with Decisions - $50,000
🏠 Top Spending	Housing - $9,000
📅 Max Weekly Spending	Monday - Highest
📆 Max Monthly Income	October - $5,000
🧩 Dashboard Features
💳 Credit Card-Style Balance Card showing available funds
📈 Monthly Trends (bar chart) for income and expenses
📊 Top 5 Expense Categories visualized as colored KPI blocks
🕒 Weekly Trend Chart to analyze weekday spending habits
🍩 Income Source Distribution with percentage-wise donut chart
🌘 Dark Theme Dashboard for a clean and modern user experience
🛠 Tools & Techniques Used
Tool	Purpose
Microsoft Excel	Dashboard building, charts, formulas
Pivot Tables	Data aggregation, filtering
Excel Charts	Column, Donut, Line, KPI layout
Conditional Formatting	Highlighting spending levels
Excel Formulas	SUMIFS, MAX, TEXT, VLOOKUP, dynamic ranges
Icons/Emojis	Visual enhancement of sections/cards
