# ✈️ Airline Delays & Cancellations — Power BI Dashboard

<img width="929" height="517" alt="image" src="https://github.com/user-attachments/assets/45dd5f6d-509c-4779-b556-47ab07af2dce" />


## Overview

An interactive Power BI dashboard analysing US airline on-time performance data. Identifies the root causes of delays, cancellation patterns, and carrier-level performance to support operational and strategic decision-making in the aviation industry.

> **Key Question:** *Where are delays coming from — and which carriers and routes are most affected?*

---

## Dashboard Features

- **Executive KPI Summary** — On-time %, cancellation rate, and average delay minutes at a glance
- **Delay Cause Breakdown** — Carrier, weather, NAS, security, and late aircraft delay categorisation
- **Monthly Trend Analysis** — Year-over-year performance comparison with trend lines
- **Carrier Comparison** — Side-by-side performance ranking across all major airlines
- **Route Drill-Through** — Click any carrier to explore origin-destination delay patterns

---

## Key Insight

> Late aircraft arrival is the dominant avoidable delay cause — outpacing weather delays by over 2x across most carriers. This points operations teams toward turnaround time optimisation rather than external factor mitigation.

---

## Tools & Skills Demonstrated

| Area | Detail |
|---|---|
| Data Transformation | Power Query — cleaning raw flight records, normalising delay codes |
| Data Modelling | Star schema: flight facts + date, carrier, airport dimensions |
| Measures | DAX — on-time rate, cancellation %, weighted avg delay, cause share |
| Visualisation | KPI cards, trend lines, bar charts, drill-through pages |

---

## Repository Structure

```
airline-delays-powerbi/
├── airline_dashboard.pbix     # Main Power BI file
├── data/
│   └── airline_data.csv       # Source dataset
├── screenshots/
│   ├── overview_page.png
│   ├── carrier_comparison.png
│   └── route_drillthrough.png
└── README.md
```

---

## How to Use

1. Download `airline_dashboard.pbix`
2. Open in **Power BI Desktop** (free download from Microsoft)
3. Connect to `data/airline_data.csv` when prompted
4. Use the slicers (carrier, year, route) to explore the data
5. Click any carrier bar to drill through to route-level detail

---

## About

Built by **Charles Edeki** — Data Analyst 
📧 charlesedeki093@gmail.com | [LinkedIn](https://www.linkedin.com/in/charles-edeki/) | [github.com/CharlesEdeki](https://github.com/CharlesEdeki)
