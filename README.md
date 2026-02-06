# Porter Delivery Analytics Dashboard

## Problem Statement
Porter Delivery has experienced a **decline in customer satisfaction**, largely linked to delays and inconsistent delivery performance. This project analyzes Porter’s delivery data to uncover the **drivers of late deliveries**, identify **operational bottlenecks**, and provide **actionable recommendations** to improve on-time performance, partner utilization, and overall customer experience [web:16][web:20][web:23].

---

## Analysis Done
- Consolidated and explored Porter Delivery’s operational dataset, focusing on order timestamps, restaurant categories, and delivery partner availability [web:16][web:23].
- Performed **data cleaning**, addressing missing values in `actual_delivery_time`, `store_primary_category`, and partner-related fields such as `total_onshift_partners` and `total_busy_partners` [web:20][web:23].
- Converted `created_at` and `actual_delivery_time` to **datetime**, enabling accurate **delivery duration** calculations and time-based analysis (hour, weekday) [web:20][web:23].
- Engineered features for:
  - Delivery duration in minutes.
  - Peak ordering windows (hour of day, day of week).
  - Partner utilization and workload intensity.
- Assessed **operational performance** by:
  - Measuring the share of orders delivered within a 30-minute benchmark.
  - Analyzing delivery time distributions to detect delays and outliers.
  - Comparing average delivery time across **store categories** and identifying **slowest-performing stores**.
  - Examining the relationship between **order volume** and **active/busy partners**, highlighting under- or over-staffed periods.
- These steps exposed systemic issues such as:
  - High pressure during peak demand with insufficient partners.
  - Consistently slow stores or categories.
  - Specific days and time windows with recurring delays.

---

## Dashboard Overview
> To use the dashboard, open `Solution.xlsx` and navigate to the **“Dashboard”** sheet. All interactivity is available on this tab.

The Excel dashboard summarizes key operational KPIs and patterns:

- **Headline metrics:**  
  - Total orders: **197,421**  
  - Revenue: **₹52.95 Cr**  
  - Average delivery time: **48.47 minutes**  
  - Partner utilization: **93.15%**
- **Time-based views:** Daily order and revenue trends enable tracking of demand spikes and performance stability.
- **Category & Market Insights:** Visuals by category and market (e.g., market ID) highlight high-volume and high-delay segments.
- **Performance monitoring:** Charts compare average delivery time and volume to spotlight underperforming stores and time windows.
- **Interactivity:** Date slicers (e.g., 21–23 Jan 2015) support deep dives into specific periods for incident-level diagnosis.
- Built for **operations leaders and strategy teams** to monitor performance, manage capacity, and act quickly on issues impacting customer satisfaction.

![Porter Delivery Dashboard](Potter.PNG)

---

## Recommendations
- **Strengthen peak-hour staffing:** Align delivery partner capacity with identified peak hours and high-demand days to reduce delays.
- **Target underperforming stores:** Provide process support or SLAs for the slowest stores and categories, or adjust their order acceptance rules.
- **Optimize routes and batching:** Use delivery duration insights to refine routing, batching, and zone assignments for partners.
- **Monitor 30-minute SLA adherence:** Track and report the percentage of orders delivered within 30 minutes as a core operational KPI.
- **Implement continuous monitoring:** Use the dashboard regularly to review trends, validate improvements, and quickly react to new bottlenecks.

---

**Author:** `Kshitij Saini`  
**LinkedIn:** [Kshitij Saini](https://www.linkedin.com/in/kshitijsaini-b950b7299?utm_source=share_via&utm_content=profile&utm_medium=member_android)
