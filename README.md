📊 BCG Furniture Sales & Profitability Analysis

📝 Project Brief
The Furniture Sales Analysis Dashboard is an end-to-end Business Intelligence solution designed to track, analyze, and optimize sales performance across various regions and product categories. Sourced from flat-file data, this project transforms raw transactional records into an interactive diagnostic tool that identifies revenue drivers, isolates areas of financial loss, and provides a clear view of order fulfillment and profit margins.

Role Target: Data Analyst / Power BI Developer

Core Tools: Power BI, Advanced DAX, Power Query

💼 Business Insights & Daily Impact
Who can use this dashboard and how does it improve their daily workflow?

C-Level Executives & Directors: Can monitor the macro-health of the business (Total Revenue, Profit, and Loss) in seconds. Daily Impact: Eliminates the need to wait for end-of-month reporting; enables real-time strategic course correction.

Regional Sales Managers: Can use interactive slicers to drill down into their specific territories and diagnose exactly which product sub-categories (e.g., Tables vs. Chairs) are driving profits or causing localized losses. Daily Impact: Replaces reactive spreadsheet crunching with proactive targeting—managers can instantly see where to apply discounts to stagnant inventory or reallocate marketing budgets.

Supply Chain Leads: Can analyze order volume trends to anticipate seasonal peaks. Daily Impact: Helps optimize warehouse stock levels for top-selling furniture items ahead of demand spikes.

🏗️ Data Architecture & The "Why" Behind Excel
Data Source: Microsoft Excel (Simulating a lightweight CRM/ERP extract).

A Note on SQL Proficiency: While I am fully equipped with and highly proficient in SQL for relational database querying, complex joins, and ETL pipelines in enterprise environments, I intentionally utilized Excel for this personal portfolio project.

Why? To keep this repository accessible, cost-free, and easy to maintain without requiring a paid cloud database or complex local server setup. The rigorous data modeling, cleaning, and transformation logic I applied here using Power Query and DAX perfectly mirrors the logic I use when connected to enterprise SQL Server or cloud data warehouses.

📑 Dashboard Architecture (Page Definitions)
The report is designed with a logical flow, guiding the user from a macro-overview down to granular diagnostics.

Executive Summary (The Command Center): Provides a high-level snapshot of business health. It houses the core KPI cards (Revenue, Profit, Loss, Total Orders) alongside overarching trend lines. It is designed to answer "How are we doing right now?" within 5 seconds of opening the report.

Regional & Category Diagnostics (The Drill-Down): Breaks down the high-level metrics by Geography and Product Segment. It utilizes matrix visuals and clustered bar charts to allow users to cross-filter (e.g., clicking the 'West' region to reveal the exact profit margins of Bookcases in that specific area).

Tooltip Integrations (Details on Demand):
Custom report page tooltips are embedded within the main visuals. Hovering over a specific month or category reveals underlying sub-metrics without cluttering the primary screen real estate.

🧮 Advanced DAX Engine
This project does not rely on simple drag-and-drop aggregations. It is powered by a robust, optimized DAX engine designed for scalability.

Time Intelligence (YoY & YTD): Implemented dynamic date calculations using CALCULATE, SAMEPERIODLASTYEAR, and DATESYTD to compare current performance against previous periods without hardcoding dates.

Dynamic Profitability & Loss Tracking: Utilized variables (VAR and RETURN) within measures to cleanly isolate profitable transactions from loss-making ones. This dynamic logic responds instantly to slicer context (e.g., SUMX and FILTER iterations).

Dynamic Ranking: Employed RANKX combined with ALLSELECTED to dynamically rank the Top N and Bottom N furniture sub-categories based on user-selected parameters.

🎨 UI/UX Design Philosophy
As a Data Analyst, I approach dashboard design with the rigor of a Senior Design Lead, adhering strictly to enterprise UI/UX principles:

Maximized Data-to-Ink Ratio: Eliminated heavy borders, unnecessary gridlines, and distracting 3D effects. Every pixel on the screen serves a communicative purpose.

Z-Pattern Visual Hierarchy: Humans read screens from top-left to bottom-right. Crucial KPIs sit at the top-left, historical trend narratives in the middle, and granular bar charts/matrices at the bottom-right.

Gestalt Principles of Proximity: Grouped related visuals closely together with subtle background shading so the user's brain perceives them as a single analytical unit.

Pre-attentive Attributes & Accessible Palettes: Used a muted, professional corporate color scheme. High-contrast colors (like Red) are exclusively reserved for 'Loss' or negative metrics to ensure immediate cognitive recognition without overwhelming the user.
