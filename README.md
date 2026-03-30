# ✈️ Airline Delays & Cancellations — Power BI Dashboard

<img width="929" height="517" alt="image" src="https://github.com/user-attachments/assets/b0ee3a53-fc67-40e1-bf88-fc0b90fbcaec" />


> 📁 **[View Dashboard Files on Google Drive](https://drive.google.com/drive/folders/1UfHnQZ_E-g8u_TeuUnw-RmZM2Lo2jhIE?usp=sharing)** — includes .pbix file and source dataset

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-0078D4?style=flat)
![Power Query](https://img.shields.io/badge/Power%20Query-217346?style=flat)

## Overview

An interactive Power BI dashboard analysing US airline performance across 1.9 million flights. Tracks flight status distribution, carrier delay rates, cancellation causes, and day-of-week patterns to give aviation analysts a clear picture of where, when, and why disruptions occur.

> **Key Question:** *Which carriers are most delayed, what is causing cancellations, and how does disruption vary across airports and days of the week?*

---

## Dashboard Features

- **3 KPI Cards with Sparklines** — Total flights (1.9M), delayed flights (791.6K), and cancelled flights (28.6K) each with an embedded trend sparkline for at-a-glance pattern reading
- **Flight Status Summary Bar** — Bottom-of-page bar showing the split between on-time (58%), delayed (40.6%), and cancelled (1.5%) across the full dataset
- **Top 10 Busiest Airports** — Horizontal bar chart ranking airports by flight volume; Atlanta and Chicago lead at 346K and 285K respectively
- **Carrier Delay Rate Ranking** — Bar chart showing delay rate % per airline; United Airlines highest at 53.5%, Hawaiian Airlines lowest at 24.2%
- **Cancellation Cause Donut Chart** — Breakdown of cancellations by Weather, Airline/Carrier, and National Air System (NAS)
- **Day-of-Week Cancellation Bar Chart** — Reveals Monday as the peak cancellation day at 2.3%, Friday lowest at 1.0%
- **Interactive Slicers** — Filter the entire dashboard by flight status (on-time, delayed, cancelled) to isolate and compare each segment

---

## Key Insight

> Weather is the dominant cause of flight cancellations, accounting for the largest share ahead of Airline/Carrier and National Air System (NAS) factors. While delays are largely an operational problem, cancellations are primarily driven by conditions outside carrier control — a distinction that matters for how airlines communicate disruptions and plan contingencies.

---

## Dashboard Preview

### Overview — All Flights
<img width="929" height="517" alt="image" src="https://github.com/user-attachments/assets/e4a4468d-1787-42f2-80ed-fcb557a711c2" />
> 1.9M total flights · 791.6K delayed (40.6%) · 28.6K cancelled (1.5%) · Atlanta and Chicago are the busiest hubs

### On-Time Flights Filter View
<img width="925" height="519" alt="image" src="https://github.com/user-attachments/assets/9911a322-e928-4308-8b54-fee74a92c5c6" />
> Filtered to on-time flights — United Airlines leads delay rate at 53.5%, Hawaiian Airlines lowest at 24.2%

### Delayed Flights — Root Cause Drill-Down
<img width="929" height="516" alt="image" src="https://github.com/user-attachments/assets/ef66c191-db3f-41e5-a5d5-106a64266d02" />
> All carriers show 100% delayed view — used for cross-carrier delay cause comparison

### Cancellations Deep-Dive
<img width="927" height="520" alt="image" src="https://github.com/user-attachments/assets/f109a0c0-f827-4966-b352-50c087a2bcf8" />
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

Built by **Charles Edeki**
📧 charlesedeki093@gmail.com | [LinkedIn](https://www.linkedin.com/in/charles-edeki/) | [GitHub](https://github.com/CharlesEdeki)
