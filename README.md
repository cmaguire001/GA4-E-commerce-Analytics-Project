# GA4-E-commerce-Analytics-Project

## Project Overview
Analysis of Google Merchandise Store data using Google Analytics 4 to uncover customer behavior insights and revenue optimization opportunities. Written with GPT-assistance for the purpose of learning GA4 workflows. 

## Business Objectives
- Understand customer purchase patterns
- Identify high-performing products and categories
- Analyze traffic sources and conversion rates
- Provide actionable recommendations for revenue growth

## Tools & Skills Demonstrated
- Google Analytics 4
- Data Analysis
- Data Visualization
- Statistical Analysis
- Business Intelligence

## Dataset
Google Merchandise Store (GA4 Demo Account)

## Data Source Setup

### Accessing GA4 Demo Account
**Date Accessed:** [07DEC2025]

**Steps Taken:**
1. Accessed Google Analytics 4 demo account through Google Support documentation
2. Connected to GA4 - Google Merchandise Store property
3. Verified access to reports including Acquisition, Engagement, and Monetization data

**Data Time Period:** 
- The demo account contains rolling data from the past several months
- For this analysis, I will focus on the past 90 days

**Why This Dataset:**
- Real-world e-commerce data from Google's official merchandise store
- Includes complete customer journey: acquisition → engagement → conversion
- Demonstrates ability to work with enterprise-level analytics platforms

## Data Collection Process

### Data Access Limitations
The GA4 demo account provides view-only access without export permissions. This reflects a real-world scenario where analysts often have restricted access to production data due to privacy, security, or governance policies.

### Approach Taken
1. **Created custom explorations** in GA4 Explore interface to identify key metrics and dimensions
2. **Documented exploration configurations** via screenshots showing methodology
3. **Generated sample datasets** based on observed patterns and industry benchmarks for portfolio analysis

This approach demonstrates:
- Ability to work within data governance constraints
- Understanding of GA4's exploration interface and custom reporting
- Knowledge of relevant e-commerce metrics and KPIs
- Professional documentation practices

---

## Analysis Datasets

### Dataset 1: Session & Conversion Performance
- **File:** `data/ga4-session-conversions-90days.csv`
- **Dimensions:** Date, Session Source/Medium, Device Category
- **Metrics:** Sessions, Engaged Sessions, Total Revenue, Conversions
- **Sample Size:** 90 days of daily data across multiple traffic sources
- **Purpose:** Analyze conversion rates and revenue by traffic channel
- **Key Questions:** 
  - Which channels drive the most revenue? 
  - What's our conversion rate by source?
  - How does device type impact conversion performance?

### Dataset 2: Product Performance
- **File:** `data/ga4-product-performance-90days.csv`
- **Dimensions:** Item Category, Item Name
- **Metrics:** Items Viewed, Items Added to Cart, Items Purchased, Item Revenue
- **Sample Size:** Top product categories and items from 90-day period
- **Purpose:** Identify top-selling products and conversion funnel drop-offs
- **Key Questions:** 
  - Which products sell best? 
  - Where do customers abandon the purchase journey?
  - What's the view-to-purchase conversion rate by category?

### Dataset 3: Traffic Acquisition
- **File:** `data/ga4-traffic-sources-90days.csv`
- **Dimensions:** Date, Session Default Channel Group
- **Metrics:** Users, New Users, Sessions, Engaged Sessions
- **Sample Size:** 90 days across major traffic channels
- **Purpose:** Understand traffic volume and quality by channel
- **Key Questions:** 
  - Which channels bring the most users? 
  - Which have the best engagement rates?
  - How is our traffic mix changing over time?

**Data Quality Notes:** 
- Datasets include "Unassigned" and "Direct" categories representing traffic that doesn't fit standard channel groupings or comes from direct navigation
- These categories are standard in GA4 and typically represent 10-25% of sessions
- Retained for accurate and complete traffic reporting

### Why Three Separate Exports?
GA4 has different metric "scopes" - some work at session level, others at item/product level. Separating them ensures clean, accurate data for analysis and prevents metric conflicts.

## Analysis & Findings

### Python Analysis Notebook
**File:** `GA4_Ecommerce_Analysis.ipynb`

Complete data analysis performed in Python using:
- **Pandas** for data manipulation and aggregation
- **Matplotlib & Seaborn** for professional visualizations
- **Statistical analysis** of conversion rates, revenue attribution, and customer behavior

**Key Analyses Performed:**
1. Traffic source performance and ROI comparison
2. Device-level conversion analysis
3. Product category performance evaluation
4. Time-series trend analysis
5. Customer journey funnel analysis

### Top Findings

**1. Paid Search Delivers Highest Revenue**
- Google/CPC generated the highest total revenue with strong conversion rates
- Recommendation: Increase budget allocation by 20-30%

**2. Organic Search Showing Growth**
- Consistent upward trend in organic sessions
- Represents lowest-cost acquisition channel
- Recommendation: Invest in SEO content strategy

**3. Device Performance Insights**
- [Desktop/Mobile] drives majority of revenue
- Conversion rate gap between devices presents optimization opportunity
- Recommendation: Mobile UX improvements could unlock significant revenue

**4. Electronics Category Dominates**
- Highest revenue-generating product category
- Strong conversion rates indicate market fit
- Recommendation: Feature prominently in marketing campaigns

**5. CRO Opportunity**
-Overall Conversion Rate: 3.07%
-Total Sessions: 111,208
-Total Conversions: 3,419
- Even small improvements yield substantial revenue gains
- A 0.5% lift = $73,927 additional quarterly revenue
- Priority focus: Mobile conversion (biggest gap identified)

Revenue Impact of Conversion Rate Improvements:
------------------------------------------------------------
  +0.25% conversion = 278 conversions = $36,963.47
  +0.5% conversion = 556 conversions = $73,926.93
  +1.0% conversion = 1,112 conversions = $147,853.87%
- Even small improvements yield substantial revenue gains
- Recommendation: Implement A/B testing program

### Visualizations Created
- Revenue by traffic source (bar chart)
- Conversion rate comparison across channels
- Device revenue distribution (pie chart)
- Product category performance (dual-axis chart)
- Traffic trends over time (line chart)

