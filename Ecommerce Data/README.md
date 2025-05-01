# 🛍️ E-commerce Business Analytics Project

## 🚀 Project Overview

This project was completed as part of Sprint 3 of a Business Analytics course. I was hired as a junior analyst to examine raw transaction logs from an e-commerce website and transform them into actionable business insights. The project focused on building a **conversion funnel**, preparing data for **cohort analysis**, and calculating **retention rates**, all using spreadsheet tools.

> 📄 [View the Project (PDF)](./Ecommerce%20Data.pdf)

---

## 📊 Dataset

The dataset includes logs of user interactions on the website. Each row represents an event such as viewing a product, opening a cart, or completing a purchase.

**Key Columns:**
- `user_id`: Unique identifier for each user
- `event_type`: Type of event (e.g., view, cart, purchase)
- `category_code`: Product category
- `brand`: Product brand
- `price`: Price in USD
- `event_date`: Date of event (YYYY-MM-DD)

---

## 📈 Part 1: Conversion Funnel

A pivot table was created to track how users moved through the funnel stages:

1. Product Page Views
2. Cart Opens
3. Purchases

**Metrics Calculated:**
- Total Conversion Rate
- Step-by-Step Conversion Rate

---

## 📦 Part 2: Data Preparation for Cohort Analysis

To analyze customer retention, we:

- **Filtered purchases** from the activity logs
- **Identified first purchase dates** per user
- **Created cohort tracking variables**:
  - `event_month`
  - `first_purchase_month`
  - `cohort_age` (months since first purchase)

---

## 📅 Part 3: Retention Rate Calculation

Using pivot tables, we:

- Grouped users into **monthly cohorts** based on first purchase
- Counted returning users over the next 4 months
- Calculated **retention rates** as a percentage of the original cohort size

---

## 📋 Part 4: Executive Summary & Documentation

- **Executive Summary Sheet**: Summarized findings from the conversion funnel and retention rate analysis
- **Table of Contents**: Organized for easy navigation
- **Formatting**: Readability-focused formatting using best spreadsheet practices (frozen headers, bold labels, borders, etc.)

---

## ✅ Results Summary

- **Conversion Funnel**:
  - Out of all users who viewed products, only a small percentage progressed to cart and ultimately completed purchases.
  - The largest drop-off occurred between product view and cart.

- **Retention Analysis**:
  - Most user cohorts had a sharp decline in activity after the first month.
  - Few users returned after two or more months post-purchase.

---

## 📌 Assumptions

- **User count** was based on *unique user IDs* at each funnel stage.
- Retention was defined as repeat purchases, not site visits or cart activity.
- Time-based cohorts were formed by the **month of first purchase**, and retention tracked monthly.

---

## 💡 Recommendations

- **Improve early-stage engagement**: Reduce the friction between viewing a product and adding to cart (e.g., clearer CTAs, personalized recommendations).
- **Enhance post-purchase retention**: Consider loyalty programs, email follow-ups, or discounts for returning customers.
- **Track user behavior over longer time periods** to identify long-term value beyond the 4-month retention window.

---

## 🧰 Tools Used

- **Google Sheets** (Advanced formulas, Pivot Tables, Formatting)
- **Spreadsheet Functions**: `VLOOKUP()`, `TEXT()`, `DATEDIF()`
- **Business Metrics**: Conversion, Retention, Cohort Tracking

---

## 📎 Files

- `Ecommerce Data.pdf`: Final version of the business analytics spreadsheet
