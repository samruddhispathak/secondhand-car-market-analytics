<div align="center">

[![Excel](https://img.shields.io/badge/Microsoft%20Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)]()
[![SPSS](https://img.shields.io/badge/IBM%20SPSS-Statistics-052FAD?style=for-the-badge&logo=ibm&logoColor=white)]()
[![Status](https://img.shields.io/badge/Status-Completed-A855F7?style=for-the-badge)]()
[![Module](https://img.shields.io/badge/Module-BBM100%20Descriptive%20Analytics-0077B5?style=for-the-badge)]()

</div>

---

## 📌 Project Overview

This business report analyses the **second-hand car market** for a fictional car dealership, **Car4All**, using a sample of **100 Aston Martin Vantage listings** scraped from an online automotive platform. The project applies descriptive statistics, hypothesis testing, and regression modelling to derive pricing insights.

> 🎯 **Goal:** Identify the key factors driving used car prices and develop a data-driven price estimation model to support dealership decision-making.

---

## 📂 Dataset

| Detail | Info |
|--------|------|
| Car Model | Aston Martin Vantage |
| Total Listings Available | 334 |
| Sample Size | 100 (random selection) |
| Randomisation Method | `=RANDBETWEEN(1, 334)` in Excel |
| Key Variables | Price, Mileage, Registration Year, Gearbox Type, Body Colour, Location |

---

## 🔍 Project Structure

### 1. Data Collection & Preparation
- Data sourced from an online car listing website
- Random sample of 100 selected using Excel's `RANDBETWEEN` function
- Cleaned text values (removed "miles", "£" symbols)
- Excluded incomplete/missing entries

### 2. Descriptive Statistical Analysis

| Variable | Mean | Median | Std Dev |
|----------|------|--------|---------|
| Price | £29,216 | £26,168 | £20,672 |
| Mileage | 69,617 mi | 50,495 mi | 49,145 mi |

- Wide variability in price due to differences in age and condition
- 95% confidence interval calculated: mean price estimated within **±£9,752**
- Newer cars and automatics consistently priced higher

### 3. Data Visualisation (Excel & SPSS)

| Chart | Type | Key Insight |
|-------|------|-------------|
| Price vs Mileage | Scatter Plot | Negative trend — higher mileage = lower price |
| Price by Gearbox | Bar Chart | Automatic cars priced significantly higher |
| Gearbox + Colour vs Price | Stacked Bar | Automatic + neutral colours dominate high price range |
| Price by Registration Year Group | Clustered Bar | Clear upward trend — newer = pricier |
| Price Distribution | Histogram | Right-skewed — most cars mid-range, few high outliers |
| Price by Gearbox | Box Plot | Automatics have higher median + wider spread |

### 4. Visualisation Design Principles Applied
- **Tufte's Principles** — minimised non-data ink, raw scatter points, no embellishment
- **Gestalt Principles** — gearbox types colour-coded, related categories grouped for easy comparison
- **Munzner's Hierarchy** — chart type matched to data type and analytical goal
- **IBCS Standards** — uniform scaling, consistent axis labels, standardised legends

### 5. Hypothesis Testing

#### ANOVA — Price by Registration Year Group
- Groups: 1995–2002 · 2003–2010 · 2011–2018 · 2019–2025
- **F = 29.71 > F crit = 2.70** · **p-value = 1.13 × 10⁻¹³**
- ✅ Reject H₀ — registration year significantly affects price
- Newest models (2019–2025) command significantly higher prices

#### t-Test — Gearbox Type (Automatic vs Manual)
- **p-value = 0.0073 < 0.05**
- ✅ Reject H₀ — automatic gearboxes are priced significantly higher than manuals

#### Chi-Square — Gearbox Type vs Body Colour
- **p-value = 0.675 > 0.05**
- ✅ Fail to reject H₀ — no significant association between gearbox type and colour

### 6. Regression Analysis

#### Simple Regression — Price vs Mileage
- **Equation:** Price = a + b(Mileage)
- Negative slope confirms: higher mileage → lower price
- Used to build an **Asking Price Calculator** for Car4All

#### Multiple Regression (SPSS) — Price vs Mileage + Registration + Gearbox
- **R² = 0.479** — model explains ~48% of price variation
- All three predictors statistically significant (p < 0.05)
- Regression diagnostics: histogram, Q-Q plot, residuals vs fitted values

---

## 🏆 Key Findings

- **Mileage is inversely related to price** — confirmed by scatter plot and regression
- **Registration year is the strongest driver** of price — newer models command significant premiums
- **Automatic gearbox adds significant market value** over manual
- **Body colour has no statistically significant effect** on gearbox choice
- Price distribution is right-skewed — a small number of low-mileage, newer models command very high prices

---

## 💼 Business Recommendations for Car4All

- Prioritise sourcing **newer automatic cars** with low mileage — highest resale value
- Use the **regression-based price calculator** to set competitive, transparent asking prices
- Adjust pricing strategy by age and condition — year of registration is the strongest value signal
- Neutral colours (black, silver, grey) dominate the high-price market — worth considering for stock selection

---

## 🛠️ Tools & Techniques

`Microsoft Excel` · `IBM SPSS Statistics` · `Data Analysis ToolPak` · `Descriptive Statistics` · `Confidence Intervals` · `ANOVA` · `t-Test` · `Chi-Square` · `Simple & Multiple Linear Regression` · `Dummy Variables` · `Data Visualisation`

---

## 👩‍💻 Author

**Samruddhi Pathak**
MSc Business Analytics · Aston University, Birmingham

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=flat&logo=linkedin)](https://www.linkedin.com/in/samruddhi-pathak-0412s)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=flat&logo=github)](https://github.com/samruddhispathak)

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=100&section=footer&animation=twinkling" width="100%"/>
</div>
