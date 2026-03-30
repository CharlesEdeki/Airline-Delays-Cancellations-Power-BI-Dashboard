# ✈️ Airline Delays & Cancellations — Power BI Dashboard

<img width="929" height="517" alt="image" src="https://github.com/user-attachments/assets/b0ee3a53-fc67-40e1-bf88-fc0b90fbcaec" />


> 📁 **[View Dashboard Files on Google Drive](https://drive.google.com/drive/folders/1UfHnQZ_E-g8u_TeuUnw-RmZM2Lo2jhIE?usp=sharing)** — includes .pbix file and source dataset

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-0078D4?style=flat)
![Power Query](https://img.shields.io/badge/Power%20Query-217346?style=flat)

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

## Dashboard Preview

### Overview — All Flights
![Airline Dashboard Overview](https://raw.githubusercontent.com/charlesedeki/airline-delays-powerbi/main/screenshots/overview_page.png)
> 1.9M total flights · 791.6K delayed (40.6%) · 28.6K cancelled (1.5%) · Atlanta and Chicago are the busiest hubs

### On-Time Flights Filter View
![On-Time Filter](https://raw.githubusercontent.com/charlesedeki/airline-delays-powerbi/main/screenshots/ontime_filter.png)
> Filtered to on-time flights — United Airlines leads delay rate at 53.5%, Hawaiian Airlines lowest at 24.2%

### Delayed Flights — Root Cause Drill-Down
![Delayed Drill-Down](https://raw.githubusercontent.com/charlesedeki/airline-delays-powerbi/main/screenshots/delayed_drilldown.png)
> All carriers show 100% delayed view — used for cross-carrier delay cause comparison

### Cancellations Deep-Dive
![Cancellations View](https://raw.githubusercontent.com/charlesedeki/airline-delays-powerbi/main/screenshots/cancellations_view.png)
> 16.4K cancellations filtered — Weather and Airline/Carrier causes visible in donut, Monday peak clearly dominant

> 📁 **[Download full .pbix file and dataset → Google Drive](https://drive.google.com/drive/folders/1UfHnQZ_E-g8u_TeuUnw-RmZM2Lo2jhIE?usp=sharing)**

---

## Tools & Skills Demonstrated

| Area | Detail |
|---|---|
| Data Transformation | Power Query — cleaning raw flight records, normalising delay codes |
| Data Modelling | Star schema: flight facts + date, carrier, airport dimensions |
| Measures | DAX — on-time rate, cancellation %, weighted avg delay, cause share |
| Visualisation | KPI cards, trend lines, bar charts, drill-through pages |

---

## How to Use

1. Download `airline_dashboard.pbix`
2. Open in **Power BI Desktop** (free download from Microsoft)
3. Connect to `data/airline_data.csv` when prompted
4. Use the slicers (carrier, year, route) to explore the data
5. Click any carrier bar to drill through to route-level detail

---

## About

Built by **Charles Edeki** — Data Analyst & Educator | Abuja, Nigeria  
📧 charlesedeki093@gmail.com | [LinkedIn](https://www.linkedin.com/in/charles-edeki/) | [GitHub](https://github.com/CharlesEdeki)
