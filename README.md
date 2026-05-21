# Meta-Ad-Performance-PowerBI-Dashboard
An interactive Power BI dashboard analyzing Meta (Facebook &amp; Instagram) ad campaign performance
# Meta Ad Performance Power BI Dashboard

##  Project Overview
This project involves the development of an interactive Meta Ad Performance Dashboard using Power BI to track, analyze, and optimize paid advertising campaigns across Facebook and Instagram[cite: 6, 202]. The dashboard monitors critical marketing metrics across the conversion funnel—from top-of-funnel reach to bottom-of-funnel purchases—to evaluate audience engagement patterns and campaign Return on Investment (ROI)[cite: 6, 48, 203, 206].

### Business Objective
The primary goal is to provide the marketing team with actionable, data-driven visibility into budget utilization, platform effectiveness, and audience targeting to maximize return per dollar spent[cite: 29, 54, 203].

---

##  Data Architecture & Modeling
The dataset is structured following an optimized **Star Schema** designed to ensure fast cross-filtering, clean DAX calculation logic, and efficient dashboard loading speeds[cite: 113].

- ""**Fact Table:** - `ad_events`: Stores log-level user interaction events such as impressions, clicks, shares, comments, and final purchases[cite: 57, 80].
- **Dimension Tables:**
  - ""`ads`: Contains ad-level metadata including creative format type, platform name, and targeting criteria[cite: 86, 88].
  - ""`campaigns`: Tracks high-level campaign strategies, start/end dates, durations, and total budget allocations[cite: 66, 92, 93].
  - ""`users`: Captures target demographic segments such as age buckets, gender, geographic location, and user interests[cite: 74, 101].

---

##  Tech Stack & Advanced Power BI Features Used
- **BI Tool:** Power BI Desktop
- ""**Data Modeling:** Star Schema (1 Fact Table connected via One-to-Many relationships to 3 Dimension Tables)[cite: 113, 114, 115].
- ""**Dynamic Metric Selection:** Implemented **Field Parameters** to bundle core measures (Impressions, Clicks, and Engagements), allowing users to dynamically toggle the Y-axis and metrics of all visual charts simultaneously[cite: 4, 234, 239].
- ""**Advanced Tooltips:** Configured a hidden **Report Page Tooltip** linked to the custom "Analysis by month" calendar layout, enabling deep-dive performance pop-ups on a per-date basis[cite: 7].
- ""**Visualizations:** Custom multi-tab layout (Facebook & Instagram), Donut Charts, Bar Charts, Map Visuals, Stacked Column Charts, Area/Line Charts, and Ad Type Performance Matrices[cite: 145, 153, 166, 169, 182, 231, 236, 241, 245, 254, 260].

---

## Key Business Insights & Analytical Findings

### 1. The "Leaky Funnel" Phenomenon
""The data shows exceptional interest at the top of the funnel, achieving a Click-Through Rate (CTR) of 11.76% and an Engagement Rate of 13.56%, both of which are significantly above standard industry averages[cite: 9, 10, 130, 131]. ""However, a sharp drop-off is visible in the lower funnel, resulting in a low overall Purchase Rate of 0.61%[cite: 11, 133, 139]. 
* ""**Actionable Recommendation:** The ad creatives and audience targeting are working brilliantly to capture attention[cite: 9, 137]. The bottleneck lies post-click. ""The business must focus on conversion rate optimization (CRO) by improving landing page speeds, streamlining the checkout flow, and launching retargeting campaigns with stronger incentive offers to capture highly engaged non-buyers[cite: 13, 32, 194].

### 2. High-Yield Demographics
Audience segmentation reveals that **Females drive 43% of total engagement**, whereas Males account for only 22%[cite: 15, 147, 149]. Performance is heavily dominated by young adults within the **18-30 age group**[cite: 15, 155].
* **Actionable Recommendation:** To maximize ROI, ad delivery and budget weights should be strategically prioritized toward young adult female cohorts aged 18-30[cite: 158, 190].

### 3. Creative Format Efficiency
When evaluating historical performance across creative formats, **Video ads** emerged as the top-performing type, maintaining the highest CTR (11.9%), Conversion Rate (5.2%), and Engagement Rate (13.7%)[cite: 183, 184]. **Stories ads** follow closely as a strong secondary format[cite: 28, 185].
* **Actionable Recommendation:** Marketing spends should be scaled away from static images and carousels, shifting budget into high-quality Video and Stories content[cite: 29, 34, 187, 191].

### 4. Hourly Engagement & Timing
An hourly trend analysis indicates that user interactions peak heavily during **late afternoon and evening hours (between 15:00 and 20:00)**, while hitting the lowest levels in the early morning[cite: 23, 170, 172].
* **Actionable Recommendation:** Implement ad scheduling to focus budget distribution during these peak hours to maximize click efficiency and response velocity[cite: 23, 36, 173, 192].

### 5. Geographic Strategy Segmentation
Geographically, high traffic and engagement volumes are heavily driven by developing markets like **India and Brazil**[cite: 16, 163, 190]. Conversely, mature premium markets like **Germany and the UK** present a significantly higher baseline for individual purchasing power and conversion efficiency[cite: 16, 164].
* **Actionable Recommendation:** Execute a segmented geographic strategy. Use high-volume brand awareness and engagement campaigns in India and Brazil, while reserving lower-funnel, value-driven product conversion campaigns for Germany and the UK[cite: 17, 37, 164].
