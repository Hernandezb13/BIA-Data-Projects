# 📊 Shopify App Analysis — Power BI Project

## 🚀 Project Overview

This project was completed as part of the **TripleTen Business Intelligence program**. As a Junior BI Analyst, I was tasked with analyzing data scraped from the Shopify App Store to uncover trends, app performance indicators, and developer responsiveness. This analysis was executed in **Power BI**, with visualizations structured around key business questions.

> 📁 Project File: [`TTBH.pbix`](./TTBH.pbix)

---

## 🧾 Dataset Overview

The dataset, sourced from Shopify's publicly available data, includes 4 related tables:

- **apps**: Details of apps in the Shopify App Store (e.g., name, reviews, developer info)
- **apps_categories**: Join table mapping apps to their multiple categories
- **categories**: Descriptions of app categories
- **reviews**: User-generated ratings, comments, helpfulness scores, and developer replies

---

## 📝 Project Context (TripleTen Requirements)

- 🏫 **Role**: Junior BI Analyst (student project)
- 🧰 **Tools**: Power BI, DAX, Data Modeling
- 📁 **Deliverables**:
  - 1 .pbix file with 3 report pages
  - Screenshots of each completed visualization
  - DAX-calculated columns and relationship modeling
- 📌 **Key Focus Areas**:
  - App landscape metrics and trends
  - Review quality and developer response behavior
  - App-level performance by developer

---

## 📊 Report Sections & Visuals

### 🔹 Part 1: App Landscape

Report Page: **App Landscape**

- ✅ KPI Card: Count of unique Shopify apps
- 📈 Line Chart: Sum of review counts over time (by `lastmod` date)
- ⚪ Scatterplot: `reviews_count` (X) vs `average_rating` (Y)
  - Includes annotated insights to interpret outliers and density

---

### 🔹 Part 2: Reviews

Report Page: **Reviews**

- 🧮 **DAX Calculation**:
  - `helpful_reviews = rating * (1 + helpful_count)`
  - KPI Card showing average value of `helpful_reviews`
- ✅ **Developer Responsiveness**:
  - `developer_answered = IF(ISBLANK(developer_reply), 0, 1)`
  - Scatterplot comparing `average_rating` vs `developer_answered`

---

### 🔹 Part 3: App Reviews

Report Page: **App Reviews**

- 🔗 **Data Modeling**:
  - Created relationship: `Reviews[app_id]` → `Apps[id]` (many-to-one)
- 📊 **Visualizations**:
  - Bar Chart: Sum of ratings by developer (note: potentially misleading)
  - Bar Chart: Average `helpful_reviews` by developer (adjusted view)
  - Bar Chart: Developer responsiveness filtered to apps with `reviews_count > 500`

---

## 📌 Key Insights

- Apps with more reviews don’t always have higher ratings.
- Developers who respond to reviews tend to have slightly higher average ratings.
- Indie developers often show higher engagement with users through responses.
- Electronic and marketing-related apps dominate high review volumes.
  
---

## 💡 Recommendations

- Shopify developers should monitor and respond to reviews to improve user trust.
- Weighting reviews by helpfulness reveals more nuanced quality measures.
- Highlighting average review helpfulness offers a clearer picture than raw rating totals.

---

## 🧰 Skills Demonstrated

- 📊 Data modeling & relationship creation in Power BI
- 🧮 DAX formula writing for calculated fields
- 📈 Visual storytelling with KPIs, bar charts, scatterplots, and line graphs
- 🔍 Business insight extraction from app marketplace data

---

## 📎 Project Files

- `TTBH.pbix`: Full Power BI report including 3 report pages and all DAX calculations

---


