# 📊 Cohort Analysis Project (Databricks + BigQuery)

This project explores user retention and repeat behavior using cohort analysis in an e-commerce dataset. SQL queries were executed in **BigQuery**, and visuals were built and analyzed in **Databricks**.

>📍 All visuals and SQL queries are available in the [notebook](Explore_cohort_analysis_biqquery_catalog.cohort_db.ecom_orders_2025-07-08_11_52_57.ipynb) and Databricks dashboard. 
> [Video Presentation](https://masterschool.zoom.us/rec/play/QREQQgqzyDqCtgdFAj0aS1wd8UvjPfXkgrqu_2qIiThVA1KVqI2zjslEskgr289ff1hLiXe5vYSkaVJ_.E6aLB2EQTwomdEhN?eagerLoadZvaPages=&accessLevel=meeting&canPlayFromShare=true&from=share_recording_detail&continueMode=true&componentName=rec-play&originRequestUrl=https%3A%2F%2Fmasterschool.zoom.us%2Frec%2Fshare%2F5Yq-oz-LbtCl08wsTlWk1XALG0c6itdIqn-o8BfU7axnbpj_r05zLHQcI94lOGMC.I5lGJZzGRvryyPmV) 
32:00-40:00 Speaker Oleksandra Protsenko

---

## 🧩 Visualizations

### 📅 1. Cohort Size by Month  
![Cohort Size by Month](./images/Cohort%20Size%20by%20Month.png)

**🔍 Key Insights**  
- **January 2024**: Largest cohort — 66 users.
- **Consistent decline**: Each subsequent month shows fewer new users:
  - Feb: 48 → Mar: 33 → Apr: 27 → May: 16 → Jun: 10
- 📉 **Possible reasons**:
  - Reduced marketing/ad spend
  - Seasonal variation
  - Issues with outreach/onboarding

✅ *Actionable Insight*: Review and replicate January’s successful acquisition campaigns.

---

### 🔁 2. Repeat Purchase Rates by Cohort  
![Repeat Purchase Rates by Cohort](./images/Repeat%20Purchase%20Rates%20by%20Cohort.png)

**🔍 Key Insights**  
- **Strong 2nd Purchase Rate**: 96–100% across all cohorts.
- **Typical Drop-Off**: From 2nd to 4th order.
- **June 2024**: Underperformed — only 60% at 4th order (vs. 83% in Jan).
- **March 2024**: Best performing cohort — sustainable repeat behavior:
  - 2nd: 1.00, 3rd: 0.94, 4th: 0.82

---

### 📈 3. Retention Rate by Cohort  
![Retention Rate by Cohort](./images/Retention%20Rate%20by%20Cohort.png)

**🔍 Key Insights**  

| Cohort     | 1-month | 2-month | 3-month | Notes |
|------------|---------|---------|---------|-------|
| Jan 2024   | 21%     | 18%     | 6%      | Weak engagement after first month |
| Feb 2024   | 29%     | 15%     | 6%      | Better start, but same drop-off |
| Mar 2024   | 42%     | 15%     | 12%     | Best long-term retention |
| Apr 2024   | 41%     | 4%      | 0%      | Very sharp decline |
| May 2024   | 44%     | 6%      | 0%      | High start, no long-term engagement |
| Jun 2024   | 70%     | –       | –       | ⚠️ Long-term data not yet available |

✅ *Conclusion*  
- **March–May cohorts**: Good initial retention, but high churn by month 2–3.
- **June**: Promising 1-month retention (70%), needs monitoring.
- 🧪 **Next steps**:
  - Improve Month 2+ experience
  - Identify churn triggers
  - Test retention strategies

---

## 🧮 SQL Scripts

SQL queries used for cohort analysis are available [in this folder](./sql/), including:

- `cohort_size.sql`
- `repeat_purchase_rates.sql`
- `retention_by_month.sql`

> 💡 All queries are optimized for BigQuery and include `JOIN`, `DATE_DIFF`, `CASE` logic, and `GROUP BY` cohort aggregation.

---
