# 🏙️ NYC Airbnb Market Analysis — Spreadsheet Data Project

## 🚀 Project Overview

This project was completed as part of the **TripleTen Business Intelligence program**. As a Junior BI Analyst, I was hired to help a client explore Airbnb market trends in Manhattan and guide investment decisions. The goal was to identify which neighborhoods and property types generate the most rental activity and revenue.

📄 [View Final Report (PDF)](./NYC%20AirBNB%20.pdf)

---

## 🧾 Dataset Overview

Two primary datasets were provided in spreadsheet format:

- **`listings`**: Contains property-level data, such as neighborhood, number of bedrooms, and `number_of_reviews_ltm` (used as a proxy for bookings).
- **`calendar`**: Contains 30 days of nightly availability and `adjusted_price` data for each listing.

---

## 📝 Project Context (TripleTen Requirements)

- 🏫 **Student Role**: Junior BI Analyst
- 📊 **Objective**: Analyze Airbnb data to identify high-performing listings and investment opportunities
- 📁 **Provided Data**: `listings` and `calendar` sheets
- 🧰 **Tools Used**: Excel / Google Sheets
- 🧪 **Key Tasks**:
  - Create and document data cleaning steps
  - Use pivot tables and formulas to analyze listing activity and revenue
  - Identify the top 10 neighborhoods by rental activity
  - Estimate revenue of top listings based on availability and price

---

## 📈 Analysis Summary

### 🔍 1. Most Attractive Neighborhoods and Property Sizes

**Key Insights:**
- Neighborhoods like **Harlem**, **Lower East Side**, and **East Village** had the highest number of reviews.
- **1-bedroom properties** were the most popular across top neighborhoods.
- **Studio apartments** were notably more popular in **Midtown**.

**Approach:**
- Used pivot tables to count reviews in the `number_of_reviews_ltm` column.
- Analyzed preferences by neighborhood and room type to detect trends.
- Created filters and segmented data to explore localized preferences.

---

### 💰 2. Revenue Estimation for Top Listings

**Data Preparation:**
- Labeled top listings using a `top_listing` column (1 if listing matched top neighborhood and top room type).
- In the `calendar` sheet, added a `revenue_earned` column:
  ```excel
  =IF([available] = "f", [adjusted_price], 0)

