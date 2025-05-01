# 📦 Monitoring Returns — Storytelling with Data (Tableau Project)

## 📌 Project Overview

This project was completed as part of the **TripleTen Business Intelligence program**. As a Junior BI Analyst, I was tasked with preparing a return analysis for the **Superstore CEO**. The goal was to investigate what’s driving customer returns and how the company can reduce return volume. I used **Tableau** to clean, visualize, and present the data in a compelling story arc for stakeholders.

📄 [Final Report (PDF)](./Montitoring%20Returns%20Story-2.pdf)

---

## 🧾 Dataset Summary

- **File Used**: `Superstore.xls`
- **Data Sources**:
  - `Orders` table (sales, categories, dates, customers)
  - `Returns` table (used in LEFT JOIN to retain both returned and non-returned entries)

---

## 🎓 Project Context: TripleTen Requirements

- 🏫 **Student Role**: Junior BI Analyst (student project)
- 📈 **Primary Goal**: Identify return trends, uncover root causes, and recommend actions
- 🧰 **Tool Used**: Tableau
- ✅ **Project Components**:
  - Visual worksheets analyzing returns by product, customer, time, and geography
  - Custom-calculated field: `Returns_Calculated` (1 = Yes, 0 = Null)
  - Dashboard mock-ups (3+ sketches) and finalized interactive dashboard
  - Presentation-ready story points and summary insights

---

## 📊 Key Visual Analyses

### 🔹 Return Rates by Dimension

- 📦 **Product**:
  - Highest return volume: **Binders (Office Supplies)**
  - Highest sales + returns: **Chairs (Furniture)**
  - Highest average return rate: **Technology (0.27)**

- 👥 **Customers**:
  - 214 customers made 2+ returns
  - Highest individual return rate approached **0.95**

- 🗺️ **Geography**:
  - **Utah, California, and Oregon** had the highest return rates
  - The **West region** stood out for elevated return activity

- 📆 **Time**:
  - **August** had the highest average return rate (0.3864)
  - Return trends analyzed across months and years (2018–2021)

- 🔁 **Composite Views**:
  - Region + Sub-Category
  - Month + Category
  - Sales vs. Returns (Scatterplot)

---

## 🧰 Skills Demonstrated

- 🧮 Custom calculated fields: `Returns_Calculated`, `Order_Count`
- 🔗 Data modeling with LEFT JOIN between `Returns` and `Orders`
- 📈 Interactive Tableau dashboards and filters
- ✍️ Storytelling using captions and storyboard flow
- 🖊️ Mock-up creation for dashboard wireframes

---

## 🧠 Key Insights

- **Returns should be measured** by both **rate** and **total number**, depending on the use case
- **Technology products** had the highest return rate, despite lower volume
- **Seasonality** and **region** are significant root causes — the **West region** and **August** had higher return activity
- **Certain customers** and **product sub-categories** (e.g., binders, chairs) drive disproportionate returns

---

## ✅ Recommendations

- Monitor **high-return sub-categories** (Binders, Chairs, Phones) for quality or fulfillment issues
- Focus on **customer-level patterns** to flag high-risk returners
- Investigate **West Coast operational processes** for root causes
- Use the dashboard filters to regularly **track return trends** by time, region, and category
- Implement return reduction strategies during **seasonal peaks** (e.g., August)

---

## 🧩 Project Artifacts

- 🖼️ 3+ Dashboard sketch mockups (pen & paper)
- 📊 Final Tableau Dashboard (interactive)
- 📄 Story Points with narrative captions
- 🎥 Optional recorded presentation or exported PDF

---

## 📎 Files Included

- `Montitoring Returns Story-2.pdf` – Final analysis and story presentation
- `Superstore.xls` – Original dataset (not included in this repo)
- (Optional) Tableau workbook `.twbx` or screen recording (if available)


