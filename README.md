# Meta-Ad-Performance-PowerBI-Dashboard
An interactive Power BI dashboard analyzing Meta (Facebook &amp; Instagram) ad campaign performance
# Meta Ad Performance Power BI Dashboard

##  Project Overview
This project involves the development of an interactive Meta Ad Performance Dashboard using Power BI to track, analyze, and optimize paid advertising campaigns across Facebook and Instagram. The dashboard monitors critical marketing metrics across the conversion funnel—from top-of-funnel reach to bottom-of-funnel purchases—to evaluate audience engagement patterns and campaign Return on Investment (ROI).

###  Business Objective
The primary goal is to provide the marketing team with actionable, data-driven visibility into budget utilization, platform effectiveness, and audience targeting to maximize return per dollar spent.

---

##  Data Architecture & Modeling
The dataset is structured following an optimized **Star Schema** designed to ensure fast cross-filtering, clean DAX calculation logic, and efficient dashboard loading speeds.

- **Fact Table:** - `ad_events`: Stores log-level user interaction events such as impressions, clicks, shares, comments, and final purchases.
- **Dimension Tables:**
  - `ads`: Contains ad-level metadata including creative format type, platform name, and targeting criteria.
  - `campaigns`: Tracks high-level campaign strategies, start/end dates, durations, and total budget allocations.
  - `users`: Captures target demographic segments such as age buckets, gender, geographic location, and user interests.

---

##  Tech Stack & Advanced Power BI Features Used
- **BI Tool:** Power BI Desktop
- **Data Modeling:** Star Schema (1 Fact Table connected via One-to-Many relationships to 3 Dimension Tables).
- **Dynamic Metric Selection:** Implemented **Field Parameters** to bundle core measures (Impressions, Clicks, and Engagements), allowing users to dynamically toggle the Y-axis and metrics of all visual charts simultaneously.
- **Advanced Tooltips:** Configured a hidden **Report Page Tooltip** linked to the custom "Analysis by month" calendar layout, enabling deep-dive performance pop-ups on a per-date basis.
- **Visualizations:** Custom multi-tab layout (Facebook & Instagram), Donut Charts, Bar Charts, Map Visuals, Stacked Column Charts, Area/Line Charts, and Ad Type Performance Matrices.

---

##  Key Business Insights & Analytical Findings

### 1. The "Leaky Funnel" Phenomenon
The data shows exceptional interest at the top of the funnel, achieving a Click-Through Rate (CTR) of 11.76% and an Engagement Rate of 13.56%, both of which are significantly above standard industry averages. However, a sharp drop-off is visible in the lower funnel, resulting in a low overall Purchase Rate of 0.61%. 
* **Actionable Recommendation:** The ad creatives and audience targeting are working brilliantly to capture attention. The bottleneck lies post-click. The business must focus on conversion rate optimization (CRO) by improving landing page speeds, streamlining the checkout flow, and launching retargeting campaigns with stronger incentive offers to capture highly engaged non-buyers.

### 2. High-Yield Demographics
Audience segmentation reveals that **Females drive 43% of total engagement**, whereas Males account for only 22%. Performance is heavily dominated by young adults within the **18-30 age group**.
* **Actionable Recommendation:** To maximize ROI, ad delivery and budget weights should be strategically prioritized toward young adult female cohorts aged 18-30.

### 3. Creative Format Efficiency
When evaluating historical performance across creative formats, **Video ads** emerged as the top-performing type, maintaining the highest CTR (11.9%), Conversion Rate (5.2%), and Engagement Rate (13.7%). **Stories ads** follow closely as a strong secondary format.
* **Actionable Recommendation:** Marketing spends should be scaled away from static images and carousels, shifting budget into high-quality Video and Stories content.

### 4. Hourly Engagement & Timing
An hourly trend analysis indicates that user interactions peak heavily during **late afternoon and evening hours (between 15:00 and 20:00)**, while hitting the lowest levels in the early morning.
* **Actionable Recommendation:** Implement ad scheduling to focus budget distribution during these peak hours to maximize click efficiency and response velocity.

### 5. Geographic Strategy Segmentation
Geographically, high traffic and engagement volumes are heavily driven by developing markets like **India and Brazil**. Conversely, mature premium markets like **Germany and the UK** present a significantly higher baseline for individual purchasing power and conversion efficiency.
* **Actionable Recommendation:** Execute a segmented geographic strategy. Use high-volume brand awareness and engagement campaigns in India and Brazil, while reserving lower-funnel, value-driven product conversion campaigns for Germany and the UK.
