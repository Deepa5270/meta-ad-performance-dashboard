# 📊 Meta Ad Performance Dashboard — Power BI Analytics Project

![Power BI](https://img.shields.io/badge/PowerBI-Dashboard-F2C811?logo=powerbi&logoColor=black) ![DAX](https://img.shields.io/badge/DAX-Measures-yellow) ![Live](https://img.shields.io/badge/Dashboard-Live-brightgreen) ![License](https://img.shields.io/badge/License-MIT-blue)

![Meta Ad Performance Dashboard](screenshots/Facebook_dashboard.png)

🔗 **[Explore the Live Interactive Dashboard →](https://app.powerbi.com/view?r=eyJrIjoiZjAxMTA1NjQtNGM5NC00ZTdjLWJmNjQtN2ZjYWQ3ZTkyOTFlIiwidCI6ImJhZDEyODY0LTkxM2UtNGI5OS04N2Q2LWI4ZDJhZDQ1OWUyNyIsImMiOjEwfQ%3D%3D)**

An interactive Power BI dashboard analyzing Meta (Facebook & Instagram) ad performance — impressions, engagement, conversions, and spend efficiency — across platforms, demographics, geography, and time. Built with dynamic DAX measures so a single set of visuals can pivot across multiple metrics on demand.

---

## 🎯 Business Problem

A marketing team running ads across **Facebook** and **Instagram** needs one place to compare performance side by side — how ads are reaching different age groups and genders, which countries are engaging most, how performance trends by day/hour, and how ad formats (Video, Stories, Image, Carousel) stack up on CTR, engagement, and conversion — without building a separate dashboard for every platform or metric.

---

## ✨ Features

- **Platform-specific pages** — dedicated Facebook and Instagram views with identical layouts for direct comparison
- **Dynamic metric switching** — a single slicer (`Select Dynamic Measures`) lets viewers swap the Age/Country/Trend charts between Impressions, Engagements, Clicks, etc. — no duplicate visuals needed
- **KPI summary cards** — Impressions, Clicks, Shares, Comments, Purchases, Engagements, plus derived rates (CTR, Engagement Rate, Conversion Rate, Purchase Rate) and spend (Total Budget, Avg. Budget/Campaign)
- **Demographic breakdown** — donut chart (Gender) and bar chart (Age)
- **Geo analysis** — interactive map of impressions by country
- **Time analysis** — weekly and hourly impression trend charts, plus a calendar heatmap with month-level drill filtering
- **Ad format comparison table** — Impressions, Clicks, CTR, Purchase Rate, Engagement Rate, Conversion Rate broken down by ad type (Video/Stories/Image/Carousel), with conditional-formatting gradients
- **Custom slicers** — filter by Campaign Name and Target Interest
- **Page navigation** built with a custom navigator styled to match brand icons

---

## 📊 Dashboard Gallery

### Facebook
![Facebook Dashboard](screenshots/Facebook_dashboard.png)

### Instagram
![Instagram Dashboard](screenshots/Instagram_dashboard.png)

👉 **[Open the live dashboard](https://app.powerbi.com/view?r=eyJrIjoiZjAxMTA1NjQtNGM5NC00ZTdjLWJmNjQtN2ZjYWQ3ZTkyOTFlIiwidCI6ImJhZDEyODY0LTkxM2UtNGI5OS04N2Q2LWI4ZDJhZDQ1OWUyNyIsImMiOjEwfQ%3D%3D)** and switch between Facebook/Instagram pages, change the Dynamic Measures slicer, or filter by month yourself.

---

## 🛠️ Tech Stack

| Layer | Tool |
|---|---|
| Data modeling & measures | Power BI Desktop, DAX |
| Data transformation | Power Query |
| Visualization | Power BI (native + New Card visual) |
| Hosting | Power BI Service (Publish to Web) |

---

## 📁 Project Structure
---

## ▶️ How to Explore

**Option 1 — No install needed:**
Click the [live dashboard link](https://app.powerbi.com/view?r=eyJrIjoiZjAxMTA1NjQtNGM5NC00ZTdjLWJmNjQtN2ZjYWQ3ZTkyOTFlIiwidCI6ImJhZDEyODY0LTkxM2UtNGI5OS04N2Q2LWI4ZDJhZDQ1OWUyNyIsImMiOjEwfQ%3D%3D) above and interact directly in your browser.

**Option 2 — Open the source file:**
```bash
git clone https://github.com/Deepa5270/meta-ad-performance-dashboard.git
```
Open `meta_dashboard.pbix` in [Power BI Desktop](https://www.microsoft.com/en-us/download/details.aspx?id=58494) (free) to inspect the data model, Power Query steps, and DAX measures directly.

---

## 🧠 DAX Concepts Demonstrated

| Concept | Where |
|---|---|
| `SELECTEDVALUE()` for dynamic titles | `Age Title`, `Map Title`, `Gender Title` |
| Disconnected table pattern for metric-switching | `Select Dynamic Measures` table |
| Safe division with `DIVIDE()` | CTR, Engagement Rate, Conversion Rate, Purchase Rate |
| Aggregation across related tables | `Total Budget`, `Avg Budget/Campaign` |
| Conditional formatting (gradient by field) | Ad Type performance table |

See [`dax_measures.md`](dax_measures.md) for the full list of formulas with explanations.

---

## 🔍 Key Insights

- **Facebook drives ~1.75x more volume than Instagram** (216K vs 123.8K impressions), but Instagram maintains a competitive engagement rate (14% on both platforms).
- Ad impressions peak in the **20–30 age bracket** before tapering off, on both platforms.
- **Video and Stories formats** consistently outperform Image and Carousel on CTR and engagement rate.
- Weekly impression trends show **consistent day-to-day performance** with no major volatility, indicating stable ad delivery pacing.
- Conversion rate is notably higher on Facebook (5.21%) compared to Instagram (4.82%), suggesting stronger down-funnel performance there despite similar engagement levels.

---

## 🚀 Next Steps

- Add year-over-year comparison once more historical data is available
- Integrate a real-time refresh via scheduled dataset refresh (requires Pro license)
- Extend ad-type analysis with cost-per-result and ROAS metrics

---

## 📄 License

This project is licensed under the MIT License — see [LICENSE](LICENSE) for details.


