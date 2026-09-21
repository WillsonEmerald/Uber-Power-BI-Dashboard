# 🚘 Uber Business Analytics Dashboard | Power BI

> **Turning ride-booking data into business decisions.**

An interactive **Uber Business Analytics Dashboard** built using **Microsoft Power BI** as part of my coursework.

The project analyzes ride bookings, revenue, vehicle performance, demand patterns, booking losses, and rider/driver experience to understand how operational data can support better business decisions.

---

## 📊 Project Snapshot

| Metric             |                 Value |
| ------------------ | --------------------: |
| 🚘 Rides Completed |               **93K** |
| ❌ Rides Lost       |               **57K** |
| 💰 Revenue         |              **₹52M** |
| 📈 Tool            |          **Power BI** |
| 🧮 Analysis        | **DAX + Power Query** |

> **Note:** The figures above represent the dataset/dashboard used in this academic project.

---

## 🎯 Project Objective

The goal of this project was not simply to create charts.

It was to answer a more important business question:

> **"What can Uber actually do with this information?"**

The dashboard transforms raw booking data into an interactive business intelligence solution that helps explore:

* Revenue performance
* Booking trends
* Vehicle performance
* Demand patterns
* Lost bookings
* Cancellation behaviour
* Rider experience
* Driver experience
* Operational performance

The overall workflow was:

**Raw Data → Data Cleaning → Data Transformation → Data Modeling → DAX → Visualization → Business Insights**

---

## 🔍 Business Questions

The dashboard was designed around several practical business questions:

### 🚘 Vehicle Performance

* Which vehicle categories generate the most revenue?
* Which vehicle types receive the highest booking volume?
* Are certain vehicle categories performing differently from others?

### 📍 Demand Analysis

* Which locations generate the highest demand?
* Where are bookings concentrated?
* Which areas could require additional driver availability?

### 📅 Time-Based Analysis

* How do bookings change over time?
* How does revenue change across different periods?
* Are there identifiable demand patterns?

### ❌ Lost Bookings

* How many potential bookings are being lost?
* What are the major reasons behind lost bookings?
* Are cancellations concentrated among riders or drivers?
* Where could operational improvements reduce lost demand?

### ⭐ Customer & Driver Experience

* What patterns appear in rider ratings?
* What patterns appear in driver ratings?
* How does experience vary across different booking or vehicle categories?

---

# 📈 Dashboard

The Power BI dashboard provides an interactive view of Uber's booking and revenue performance.

### Dashboard Overview

![Dashboard Overview](screenshots/dashboard-overview.png)

### Revenue & Vehicle Analysis

![Revenue Analysis](screenshots/revenue-analysis.png)

### Booking & Demand Analysis

![Booking Analysis](screenshots/booking-analysis.png)

### Lost Bookings & Cancellations

![Cancellation Analysis](screenshots/cancellation-analysis.png)

---

# 💡 Key Insights

Some of the questions explored through the dashboard include:

### 1. Revenue Performance

The dashboard provides a breakdown of revenue across vehicle categories, helping identify where the largest contribution to overall revenue comes from.

### 2. Demand Concentration

Location-level analysis helps reveal areas with higher booking activity and potential demand concentration.

### 3. Booking Losses

The analysis separates completed and lost bookings, allowing potential operational bottlenecks and cancellation patterns to be investigated.

### 4. Vehicle Performance

Comparing booking volume and revenue across vehicle types provides a way to understand differences in vehicle-level performance.

### 5. Customer & Driver Experience

Ratings and booking behaviour provide additional context beyond purely financial metrics.

---

# 🛠️ Tools & Technologies

### Business Intelligence

* **Microsoft Power BI**

### Data Preparation

* **Power Query**
* Data cleaning
* Data transformation
* Data type management
* Data quality checks

### Data Analysis

* **DAX**
* Calculated measures
* KPIs
* Time-based analysis
* Aggregations
* Comparative analysis

### Data Visualization

* Interactive dashboards
* KPI cards
* Bar charts
* Line charts
* Donut charts
* Maps / geographic analysis
* Slicers
* Drill-down analysis

---

# 🧮 Example DAX Measures

Some of the analytical logic used in the dashboard included measures for bookings, revenue, completed rides, and lost bookings.

```DAX
Total Bookings =
COUNTROWS('Bookings')
```

```DAX
Completed Rides =
CALCULATE(
    [Total Bookings],
    'Bookings'[Booking Status] = "Completed"
)
```

```DAX
Total Revenue =
SUM('Bookings'[Booking Value])
```

```DAX
Lost Rides =
CALCULATE(
    [Total Bookings],
    'Bookings'[Booking Status] <> "Completed"
)
```

> The exact measures may vary depending on the structure and naming of the underlying dataset.

---

# 🔄 Data Analytics Workflow

```text
                RAW BOOKING DATA
                       │
                       ▼
                DATA CLEANING
                       │
                       ▼
              POWER QUERY TRANSFORM
                       │
                       ▼
                DATA MODELING
                       │
                       ▼
                 DAX MEASURES
                       │
                       ▼
              INTERACTIVE DASHBOARD
                       │
                       ▼
              BUSINESS INSIGHTS
                       │
                       ▼
                 DECISIONS
```

---

# 🧠 From Data → Insight → Decision

One of the main objectives of this project was to move beyond descriptive visualization.

For example:

```text
Observation
     ↓
High demand in a location
     ↓
Business Question
     ↓
Is driver availability sufficient?
     ↓
Potential Action
     ↓
Review driver allocation / availability
```

Similarly:

```text
Observation
     ↓
High number of lost bookings
     ↓
Business Question
     ↓
Why are bookings being lost?
     ↓
Potential Action
     ↓
Investigate cancellation / availability patterns
```

The dashboard therefore focuses on connecting **metrics with potential business questions**, rather than treating visualization as the final output.

---

# 📚 What I Learned

This project gave me hands-on experience with:

* Power BI dashboard development
* Power Query
* DAX
* Data cleaning
* Data transformation
* KPI development
* Data visualization
* Business analytics
* Exploratory data analysis
* Interactive filtering
* Data storytelling
* Translating business questions into analytical views

Most importantly, I learned that:

> **A dashboard shouldn't just make data look good. It should make the next decision easier.**

---

# 🎓 Project Context

**Project Type:** Academic / Coursework Project

**Domain:** Transportation & Mobility Analytics

**Focus:** Business Intelligence & Data Analytics

**Primary Tool:** Microsoft Power BI

---

# 🚀 Potential Business Applications

A similar analytics solution could potentially support:

* Driver allocation
* Demand forecasting
* Vehicle category optimization
* Cancellation analysis
* Revenue monitoring
* Location-level demand planning
* Customer experience analysis
* Operational performance monitoring

These are potential applications of the analytical framework and are not claims about Uber's actual internal operations.

---

# 📁 Repository Structure

```text
uber-business-analytics-powerbi/
│
├── dashboard/
│   └── Uber_Business_Analytics.pbix
│
├── data/
│   └── README.md
│
├── screenshots/
│   ├── dashboard-overview.png
│   ├── revenue-analysis.png
│   ├── booking-analysis.png
│   └── cancellation-analysis.png
│
├── documentation/
│   └── project-notes.md
│
├── README.md
└── LICENSE
```

---

# ⚠️ Data & Disclaimer

This repository contains an **academic/coursework analytics project** created for learning and portfolio purposes.

The analysis is based on the dataset used for the project and should not be interpreted as representing Uber's current internal business performance.

**Uber** is a trademark of its respective owner. This project is not affiliated with, sponsored by, or endorsed by Uber.

If the underlying dataset is sourced from a third party, please refer to its original source and licensing terms before redistributing it.

---

# 👨‍💻 Author

**Willson Emerald**

MSc Big Data Analytics

Interested in:

* Data Analytics
* Business Intelligence
* Data Visualization
* AI & Analytics
* Cloud Technologies

---

## ⭐ If you found this project useful

Feel free to explore the dashboard, review the analytical approach, and connect with me to discuss data analytics, business intelligence, or data-driven products.
