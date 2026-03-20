# 📊 BCG Furniture Sales & Profitability Analysis

Welcome to my portfolio project! I am a **Data Analyst / Power BI Developer** passionate about transforming complex data into intuitive, enterprise-grade dashboards. 

## 📝 Project Brief
This **Furniture Sales Analysis Dashboard** is an end-to-end Business Intelligence solution designed to track, analyze, and optimize sales performance across various regions and product categories. It serves as an interactive diagnostic tool that identifies revenue drivers, isolates areas of financial loss, and provides a clear view of order fulfillment and profit margins.

## 💼 Business Insights & Daily Impact
This dashboard transitions teams from manual spreadsheet reporting to automated, actionable analytics:
* **C-Level Executives & Directors:** Can monitor the macro-health of the business (Total Revenue, Profit, Loss) instantly. *Daily Impact:* Enables real-time strategic course correction without waiting for end-of-month reports.
* **Regional Sales Managers:** Can drill down into specific territories and diagnose exactly which product sub-categories (e.g., Tables vs. Chairs) are driving profits or causing localized losses. *Daily Impact:* Allows proactive targeting—managers can instantly see where to apply discounts to stagnant inventory or reallocate marketing budgets.
* **Supply Chain Leads:** Can analyze order volume trends to anticipate seasonal peaks. *Daily Impact:* Helps optimize warehouse stock levels for top-selling furniture items ahead of demand spikes.

## 🏗️ Data Architecture & The "Why" Behind Excel
**Data Source:** Microsoft Excel (Simulating a lightweight CRM/ERP extract).

> **A Note on SQL Proficiency:** While I am fully equipped with and highly proficient in **SQL** for relational database querying, complex joins, and ETL pipelines in enterprise environments, I intentionally utilized Excel for this personal portfolio project. 
> 
> *Why?* To keep this repository accessible, cost-free, and easy to maintain without requiring a paid cloud database or complex local server setup. The rigorous data modeling, cleaning, and transformation logic I applied here using Power Query and DAX perfectly mirrors the logic used when connected to enterprise SQL Server or cloud data warehouses.

## 📑 Dashboard Architecture & Page Definitions
The report is designed with a logical flow, guiding the user from a macro-overview down to granular diagnostics.

1. **Executive Summary (The Command Center):** Provides a high-level snapshot of business health. Houses core KPI cards (Revenue, Profit, Loss, Total Orders) alongside overarching trend lines. Designed to answer "How are we doing right now?" within 5 seconds.
2. **Regional & Category Diagnostics (The Drill-Down):** Breaks down high-level metrics by Geography and Product Segment. Utilizes matrix visuals and clustered bar charts for cross-filtering (e.g., clicking the 'West' region to reveal the exact profit margins of Bookcases in that area).
3. **DAX & Measure Dictionary (For Technical Review):** A dedicated view showcasing the complex measure logic driving the dashboard, demonstrating my ability to write optimized DAX code for enterprise scenarios.

## 🧮 Advanced DAX Engine (Technical Showcase)
This project moves beyond simple drag-and-drop aggregations, powered by a robust, optimized DAX engine designed for scalability:
* **Time Intelligence (YoY & YTD):** Implemented dynamic date calculations using `CALCULATE`, `SAMEPERIODLASTYEAR`, and `DATESYTD` to compare current performance against previous periods without hardcoding dates.
* **Dynamic Profitability Tracking:** Utilized variables (`VAR` and `RETURN`) within measures to cleanly isolate profitable transactions from loss-making ones. This logic responds instantly to slicer context using `SUMX` and `FILTER` iterations.
* **Dynamic Ranking:** Employed `RANKX` combined with `ALLSELECTED` to dynamically rank the Top N and Bottom N furniture sub-categories based on user-selected parameters.

# 🎨 UI/UX Design Philosophy
Approaching dashboard design with the rigor of a Senior Design Lead (incorporating 10+ years of design principle best practices), I adhered strictly to enterprise UI/UX standards:
1. **Maximized Data-to-Ink Ratio:** Eliminated heavy borders, unnecessary gridlines, and distracting 3D effects. Every pixel serves a communicative purpose.
2. **Z-Pattern Visual Hierarchy:** Structured for natural reading patterns (top-left to bottom-right). Crucial KPIs sit top-left, historical trends in the middle, and granular matrices bottom-right.
3. **Gestalt Principles of Proximity:** Grouped related visuals closely together with subtle background shading so the user's brain perceives them as a single analytical unit.
4. **Accessible Palettes:** Used a muted, professional corporate color scheme. High-contrast colors (like Red) are exclusively reserved for 'Loss' or negative metrics to ensure immediate cognitive recognition without overwhelming the user.

---
*Feel free to explore the `.pbix` file included in this repository to see the data model and DAX measures in action!*
