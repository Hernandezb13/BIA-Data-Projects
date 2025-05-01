# 🏙️ NYC Airbnb Market Analysis — Spreadsheet Data Project

## 📌 Project Overview

This project was completed as part of the **TripleTen Business Intelligence program**. As a Junior BI Analyst, I was hired to help a client analyze Manhattan Airbnb data to identify profitable investment opportunities. Using spreadsheet tools, I determined which neighborhoods and property types generate the most rental activity and revenue.

📄 [Final Report (PDF)](./NYC%20AirBNB%20.pdf)

---

## 🧾 Dataset Summary

The analysis used two key data tables:

- **`listings`** – Includes property details like price, bedroom count, neighborhood, and `number_of_reviews_ltm` (used as a proxy for rental frequency)
- **`calendar`** – Daily availability and adjusted price data for each listing over a 30-day period

---

## 🎓 Project Context: TripleTen Requirements

- **Role**: Junior BI Analyst (student)
- **Objective**: Help a client identify top-performing vacation rentals in Manhattan
- **Data Cleaning**:
  - Maintained a raw copy of the dataset
  - Documented all cleaning steps in a separate worksheet
- **Tools**: Google Sheets / Excel
- **Key Deliverables**:
  - Pivot tables identifying attractive neighborhoods and room types
  - Revenue estimates for top listings
  - A stakeholder-facing final report with data-driven recommendations

---

## 📊 Analysis Breakdown

### 1️⃣ Most Attractive Neighborhoods & Property Sizes

- Used `number_of_reviews_ltm` as an estimate of rental frequency
- Created pivot tables to analyze:
  - Top neighborhoods by review count
  - Most popular bedroom counts
  - Differences in room-type preference across neighborhoods

**Insight**: One-bedroom units were most attractive across neighborhoods, except for Midtown, which favored studios.

---

### 2️⃣ Revenue Estimates for Top Listings

- Added `top_listing` column in `listings` to flag listings in top neighborhoods with the most popular room type
- In the `calendar` table:
  - Created a `revenue_earned` column:
    ```excel
    =IF([available] = "f", [adjusted_price], 0)
    ```
- In `listings`:
  - Used `SUMIF()` to calculate total 30-day revenue from `calendar`
  - Estimated annual revenue by multiplying by 12
- Created a pivot table filtered by `top_listing = 1` to rank listings by estimated revenue

---

## 💡 Key Insights

- **Harlem**, **Lower East Side**, and **East Village** had the highest review volumes
- Midtown stood out for its popularity in **studio apartments**
- Top listings in 1-bedroom and studio formats demonstrated strong revenue potential

---

## ✅ Recommendations

- Focus investment on **1-bedroom listings** in high-review neighborhoods like **Harlem** and **East Village**
- Treat **Midtown studios** as a unique, high-performing property type
- Use **review count over the last 12 months** as a proxy for booking frequency
- Prioritize properties with high pricing and frequent availability for higher revenue

---

## 🧰 Skills Demonstrated

- Data cleaning and documentation
- Pivot table analysis for segmentation and ranking
- Spreadsheet functions: `IF()`, `SUMIF()`, conditional logic
- Revenue modeling using adjusted nightly pricing
- Stakeholder-focused reporting and insight delivery

---

## 📎 Files Included

- `NYC AirBNB .pdf` – Final project report
- `listings_cleaned.xlsx` – Listings data with new columns for filtering and revenue
- `calendar_processed.xlsx` – Calendar data with nightly revenue calculations

