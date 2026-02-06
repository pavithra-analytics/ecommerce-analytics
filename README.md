# SQL Analytics Portfolio

This repository contains three end-to-end SQL projects demonstrating **business analytics, product analytics, and experimentation analysis** using e-commerce data. 

## Project 1: Ecommerce Funnel & Conversion Analysis

**Objective:**  
Analyze the e-commerce user journey to identify funnel drop-offs, conversion rates, top-performing products, and repeat customer behavior.

**SQL Analysis Performed:**  
- Total unique users: **10,000**  
- Funnel analysis (View → Cart → Purchase)  
- Conversion rate calculation  
- Top products by purchase  
- Repeat customer behavior  
- Daily purchase trend  
- Cart abandonment rate  

**Key Insights / Results:**  
- Total users who viewed products: **10,000**  
- Added to cart: **4,200** → cart abandonment: **2,100** (50%)  
- Completed purchase: **1,500** → overall conversion rate: **15%**  
- Top 3 products accounted for **35% of all purchases**  
- Repeat customers (≥2 purchases): **200 users**  
- Conversion drop-off mostly occurs at the **checkout page**  

**Skills Demonstrated:**  
SQL (CTEs, aggregations, funnel analysis), Product Analytics, Business Insights

## Project 2: Cohort & Retention Analysis

**Objective:**  
Analyze user retention by cohort to understand long-term engagement, churn patterns, and product stickiness.

**SQL Analysis Performed:**  
- Identify each user's first activity (cohort date)  
- Calculate days since signup (cohort index)  
- Count active users per cohort per day  
- Calculate retention percentage per cohort  
- Optional: cumulative retention using window functions  

**Key Insights / Results (Example Cohort Retention):**  

| Cohort Date | Day 0 | Day 1 | Day 7 | Day 30 |
|------------|-------|-------|-------|--------|
| 2026-01-01 | 500   | 210   | 90    | 40     |
| 2026-01-02 | 450   | 180   | 75    | 35     |
| 2026-01-03 | 520   | 225   | 95    | 50     |

- Day 1 retention: ~42%  
- Day 7 retention: ~18%  
- Day 30 retention: ~9%  
- Retention drops sharply after first week → early engagement is critical  
- Certain cohorts retained better due to higher initial onboarding activity  

**Skills Demonstrated:**  
Advanced SQL (CTEs, window functions), Cohort Analysis, Retention Modeling, Product Analytics

## Project 3: A/B Testing Analysis

**Objective:**  
Evaluate the impact of a hypothetical A/B test on purchase conversion, measuring whether **Group B (treatment)** outperforms **Group A (control)**.

**SQL Analysis Performed:**  
- Assign users to A/B groups (50/50 split based on user_id)  
- Identify if users converted (made at least one purchase)  
- Calculate conversion rate per group  
- Compute statistical significance using Z-score  

**Key Insights / Results:**  

| Experiment Group | Total Users | Users Converted | Conversion Rate (%) | Z-Score vs A |
|-----------------|------------|----------------|-------------------|--------------|
| A (Control)     | 5,000      | 700            | 14.0%             | N/A          |
| B (Treatment)   | 5,000      | 800            | 16.0%             | 2.5          |

- Group B had **16% conversion** vs **14% in Group A**  
- Z-score = 2.5 → statistically significant improvement at **95% confidence**  
- Suggests **treatment changes positively influenced purchases**  

**Skills Demonstrated:**  
SQL (CASE statements, aggregations), Experiment Analysis, Statistical Testing, Product & Business Analytics
