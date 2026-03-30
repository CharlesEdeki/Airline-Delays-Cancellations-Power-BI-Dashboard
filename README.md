# ✈️ Airline Delays & Cancellations — Power BI Dashboard

> 📁 **[View Dashboard Files on Google Drive](https://drive.google.com/drive/folders/1UfHnQZ_E-g8u_TeuUnw-RmZM2Lo2jhIE?usp=sharing)** — includes .pbix file and source dataset

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-0078D4?style=flat)
![Power Query](https://img.shields.io/badge/Power%20Query-217346?style=flat)

---

## Dashboard Preview

### Overview — All Flights
<img width="929" height="517" alt="image" src="https://github.com/user-attachments/assets/e4a4468d-1787-42f2-80ed-fcb557a711c2" />

> 1.9M total flights · 791.6K delayed (40.6%) · 28.6K cancelled (1.5%) · Atlanta leads with 346,836 flights

### On-Time Filter View
<img width="925" height="519" alt="image" src="https://github.com/user-attachments/assets/9911a322-e928-4308-8b54-fee74a92c5c6" />
> Filtered to on-time flights · United Airlines highest delay rate at 53.5%, Hawaiian Airlines lowest at 24.2%

### Delayed Flights Drill-Down
<img width="929" height="516" alt="image" src="https://github.com/user-attachments/assets/ef66c191-db3f-41e5-a5d5-106a64266d02" />
> All carriers at 100% delayed view — used for cross-carrier delay cause comparison

### Cancellations Deep-Dive
<img width="927" height="520" alt="image" src="https://github.com/user-attachments/assets/f109a0c0-f827-4966-b352-50c087a2bcf8" />
> 16.4K cancellations filtered · Weather dominates cancellation causes · Monday peak at 2.3%, Friday lowest at 1.0%

---

## The State of the Skies

Across 1.9 million US domestic flights, **40.6% were delayed and 1.5% were cancelled**, meaning fewer than 6 in 10 passengers experienced an on-time departure. In an industry where reliability is a primary purchase driver, a 58% on-time rate represents a significant and measurable competitive liability.

This analysis examines carrier-level performance, cancellation causes, airport volume patterns, and day-of-week disruption trends to determine where delays and cancellations concentrate, and what patterns emerge that airlines and airports could act on.

> **Key Question:** *Which carriers are consistently underperforming on delay rates, what is driving cancellations, and when and where does the system come under the most strain?*

---

## Inside the Dashboard

- **3 KPI Cards with Sparklines** - Total flights (1.9M), delayed flights (791.6K), and cancelled flights (28.6K), each with an embedded trend sparkline
- **Flight Status Summary Bar** - Bottom bar showing on-time (58.0%), delayed (40.6%), and cancelled (1.5%) proportions across the full dataset
- **Top 10 Busiest Airports** - Horizontal bar chart by flight volume; Atlanta (346,836) and Chicago (285,884) lead the ranking
- **Carrier Delay Rate Ranking** - Bar chart showing delay rate % per airline; United Airlines highest at 53.5%, Hawaiian Airlines lowest at 24.2%
- **Cancellation Cause Donut Chart** - Breakdown by Weather, Airline/Carrier, and National Air System (NAS)
- **Day-of-Week Cancellation Bar Chart** - Monday peaks at 2.3%, Friday lowest at 1.0%
- **Interactive Status Slicer** - Filter the entire dashboard by on-time, delayed, or cancelled to isolate each segment

---

## How Bad Is It, Really?

### The Top Line

| Metric | Value |
|---|---|
| Total Flights | 1,900,000+ |
| On-Time Rate | **58.0%** |
| Delay Rate | **40.6%** (791.6K flights) |
| Cancellation Rate | **1.5%** (28.6K flights) |

### Carrier by Carrier: Who Is Letting Passengers Down?

Delay rates vary dramatically across carriers - a 29-percentage-point spread between best and worst:

| Carrier | Delay Rate |
|---|---|
| United Air Lines | **53.5%** |
| Southwest Airlines | 51.4% |
| Spirit Air Lines | 49.2% |
| JetBlue Airways | 44.3% |
| Frontier Airlines | 40.7% |
| Virgin America | 39.4% |
| American Airlines | 37.7% |
| American Eagle | 37.1% |
| Delta Air Lines | 35.7% |
| SkyWest Airlines | 35.0% |
| Atlantic Southeast | 32.8% |
| US Airways | 31.2% |
| Alaska Airlines | 24.5% |
| Hawaiian Airlines | **24.2%** |

United Airlines delays more than half its flights. Hawaiian Airlines delays fewer than 1 in 4. The gap between them is not explained by route complexity alone, it reflects operational and scheduling differences that are within carrier control.

Alaska and Hawaiian Airlines, both operating concentrated route networks with limited hub complexity, consistently outperform the legacy mega-carriers. The data raises a structural question: whether the hub-and-spoke complexity of the largest networks is inherently delay-generating, or whether it is a management and scheduling problem that larger carriers have not yet solved.

### Why Flights Get Cancelled

Weather is the dominant cause of flight cancellations, outpacing both Airline/Carrier and National Air System (NAS) causes combined. This matters operationally: weather-driven cancellations are largely beyond carrier control, while Airline/Carrier cancellations represent preventable failures — equipment, crew, and scheduling issues that reflect internal operational decisions.

The distinction is important for how carriers communicate disruptions to customers. Framing all cancellations as weather events, when a meaningful portion are carrier-caused, erodes passenger trust and misrepresents the carrier's actual reliability.

### Monday Is the Worst Day to Fly

| Day | Cancellation Rate |
|---|---|
| Monday | **2.3%** |
| Sunday | 1.7% |
| Tuesday | 1.4% |
| Thursday | 1.3% |
| Wednesday | 1.2% |
| Saturday | 1.2% |
| Friday | **1.0%** |

Monday cancellations run at more than double the Friday rate. This is consistent with the well-documented "Monday effect" in aviation — weekend maintenance, crew positioning issues, and late aircraft from Sunday operations cascade into Monday disruptions. Airlines that carry a clean operational slate into Monday should perform meaningfully better on this metric.

### Where the Pressure Concentrates

The ten busiest airports by flight volume reveal where system pressure concentrates:

| Airport | Flights |
|---|---|
| Atlanta | 346,836 |
| Chicago | 285,884 |
| Dallas-Fort Worth | 239,551 |
| Denver | 196,055 |
| Los Angeles | 194,673 |
| San Francisco | 148,008 |
| Phoenix | 146,815 |
| Houston | 146,622 |
| Las Vegas | 133,181 |
| Minneapolis | 112,117 |

Atlanta alone handles nearly twice the traffic of any West Coast hub. Congestion at Atlanta has downstream consequences for the entire eastern seaboard network. Delays there do not stay local.

---

## Diagnosing the System

1. **Carrier-driven delays dominate the delay picture** - with delay rates ranging from 24% to 53%, the spread is too wide to be explained by external factors. Scheduling, turnaround management, and crew deployment differ substantially between carriers.
2. **Weather drives cancellations but not delays at the same rate** - the cancellation cause breakdown shows weather as the leading cancellation driver, yet overall delay rates are not proportionally explained by weather, implying late aircraft and operational factors are significant delay contributors.
3. **Monday is structurally vulnerable** - the 2.3% Monday cancellation rate vs. 1.0% on Friday is consistent and predictable, pointing to weekend operational recovery as a systemic weak point across the industry.
4. **Hub concentration amplifies disruption** - the busiest airports (Atlanta, Chicago, DFW) are also the most delay-sensitive nodes in the network. A disruption at any one of them ripples downstream to dozens of connecting routes.

---

## What the Industry Should Look Like

- Industry on-time rate above 80%, consistent with customer expectations and competitive benchmarks
- Cancellation cause transparency separating weather-caused from carrier-caused cancellations in passenger communications
- Monday operational reliability brought in line with mid-week performance through improved weekend recovery planning
- Delay rate convergence across carriers toward the Alaska/Hawaiian benchmark of 24–25%

---

## Where to Start Fixing It

**1. Carrier-specific delay reduction programmes**
The 29-point spread between best and worst carriers demonstrates that operational improvement is achievable, it is not a constraint of the industry. United, Southwest, and Spirit should study the scheduling and turnaround practices of Alaska and Hawaiian Airlines as concrete internal benchmarks.

**2. Weather-contingency routing protocols**
While weather-driven cancellations cannot be eliminated, the response time and rebooking quality can be standardised. Carriers without automated re-accommodation workflows leave customers stranded unnecessarily long after the weather event resolves.

**3. Monday recovery planning**
The Monday spike is predictable enough to plan for. Positioning reserve aircraft and crew at key hubs on Sunday evening rather than relying on standard crew scheduling would reduce the Monday cascade effect that currently inflates the start-of-week cancellation rate.

**4. Hub congestion management at Atlanta and Chicago**
With Atlanta handling 346,836 flights and Chicago 285,884, both airports are carrying disproportionate network risk. Scheduling de-peaking, distributing departures more evenly across hours, would reduce the bunching that amplifies delay propagation.

---

## Technical Breakdown

| Area | Detail |
|---|---|
| Data Modelling | Star schema - flight facts + date, carrier, and airport dimensions |
| DAX Measures | On-time rate, cancellation %, delay rate per carrier, day-of-week breakdowns |
| Power Query | Raw flight record cleaning, delay code normalisation, carrier name standardisation |
| Visualisation | KPI sparklines, ranked bar charts, donut chart, status filter slicer |
| Aviation Context | Carrier performance benchmarking, hub-and-spoke delay propagation, cancellation cause taxonomy |

---

## About

Built by **Charles Edeki**
📧 charlesedeki093@gmail.com | [LinkedIn](https://www.linkedin.com/in/charles-edeki/) | [GitHub](https://github.com/CharlesEdeki)
