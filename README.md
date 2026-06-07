# European Hotel Review Analytics — TravelSphere BI Dashboard

**Tool:** Tableau Desktop | **Language:** Python | **Context:** RMIT University — Master of Analytics

---

## Project Overview

This project simulates a real-world business intelligence task for **TravelSphere**, a luxury travel agency curating personalised European vacation experiences. As a BI Analyst, the goal was to analyse customer feedback from a large public hotel reviews dataset and design an interactive dashboard to help the **Head of Customer Experience** make data-driven decisions on partner hotel selection.

---

## Business Questions Addressed

| Area | Question |
|---|---|
| 🗺️ Geographic Performance | Which cities and locations yield the highest customer satisfaction? |
| 🌍 Nationality Bias | Do ratings vary by reviewer nationality? Are some nationalities harsher critics? |
| 💬 Sentiment Drivers | What are the common themes in positive vs. negative reviews? |
| 📅 Seasonality | How does review volume and satisfaction change across months of the year? |

---

## Dataset

- **Source:** Public European Hotel Reviews dataset (Kaggle)
- **Scope:** 2017 reviews only (filtered by `Review_Date`)
- **Size:** 500,000+ reviews across hotels in 6 European cities
- **Key fields:** Hotel name, city, reviewer nationality, reviewer score, positive/negative review text, review date, coordinates

---

## Tools & Technologies

- **Python** — Data cleaning, preprocessing, and sentiment theme extraction
- **Tableau Desktop** — Dashboard design, interactivity, and visual storytelling
- **Tableau Prep Builder** — Optional data flow documentation

---

## Data Cleaning Steps

1. Filtered dataset to **2017 reviews only** using `Review_Date`
2. Removed records with missing or invalid coordinates (`Coordinate_Status`)
3. Cleaned reviewer nationality field — standardised country names
4. Processed positive and negative review text — removed nulls, cleaned whitespace
5. Extracted **sentiment theme categories** from review text using AI-assisted topic classification
6. Created calculated fields: `Satisfaction_Band`, `Review_Month_Name`, `Days_Since_Review`
7. Validated descriptive statistics post-cleaning (row counts, score distributions, date ranges)

---

## Dashboard Features

### Dashboard 1 — Hotel Portfolio Overview
- Average review score by city (bar chart)
- Geographic map of hotel satisfaction by coordinates
- Satisfaction band distribution (pie/donut)
- Filters: City, Satisfaction Band, Month

### Dashboard 2 — Review Insights
- Monthly review volume and average score trend (line chart)
- Reviewer nationality rating patterns (heatmap/bar)
- Top positive and negative review themes (bar charts)
- Filters: Nationality, Month, Hotel City

---

## Key Insights

- **London and Paris** hotels showed the widest satisfaction variance — high risk and high reward for luxury clients
- **Japanese and Australian** reviewers consistently rated higher; **Eastern European** reviewers tended to score lower on average
- Most common **negative themes**: room size, noise, and check-in experience
- Most common **positive themes**: location, staff friendliness, and breakfast quality
- **Summer months (June–August)** had the highest review volume but slightly lower average scores — suggesting peak season pressure on hotel quality

---

## Use Cases

### Use Case 1 — City Selection for Premium Clients
A client wants a 5-star hotel experience in Europe. The dashboard is filtered by `Satisfaction_Band = Excellent` and sorted by city — instantly surfacing the top-performing cities and specific hotels to recommend.

### Use Case 2 — Nationality-Aware Advising
A group of Australian travellers books through TravelSphere. The nationality filter reveals how Australian reviewers specifically rated each city — allowing the advisor to align recommendations with that audience's known preferences.

---

## How to Use

1. Open `Assignment2.twbx` in **Tableau Desktop 2026.1+**
2. Navigate between dashboards using the tabs at the bottom
3. Use the filter panels on the right to slice by city, month, nationality, or satisfaction band
4. Hover over any chart element for detailed tooltips
5. Click any bar or map point to cross-filter all other visuals on the dashboard

---

## Files

| File | Description |
|---|---|
| `Assignment2.twbx` | Tableau Packaged Workbook with embedded data and dashboards |
| `README.md` | This file |

---

## Author

**Aaliya Siraj**
Master of Analytics — RMIT University, Melbourne
[LinkedIn](#) | [Tableau Public](#) | [GitHub](https://github.com/aaliyasiraj)
