# Namma Yatri: Ride Demand & Cancellation Dashboard (Power BI)

A 10-page Power BI report on ride demand, revenue, cancellations and driver performance for Namma Yatri, a Bengaluru ride-hailing service. It shows where and when demand is highest, where revenue comes from, and where service breaks down.

## Key Findings

| Metric | Value |
|---|---|
| Total searches | 2.16K |
| Completed trips | 983 (**45.49%** completion) |
| Cancelled trips | 1.18K (**54.51%** cancellation) |
| Total revenue | ₹751K |

- **Over half of searches end in cancellation.** Service reliability is the biggest opportunity.
- **Night drives the business:** 364 trips (the most of any period) and **37.4%** of revenue. Evening is the weakest at 15.5%.
- **Revenue is concentrated in a few zones:** Bangalore South (₹30.3K), Yeshwantpur (₹29.0K) and Hebbal (₹28.1K) lead. Doddaballapur and Pulakeshinagar are at the bottom.
- **Cancellation hotspots:** Mahadevapura (49), C. V. Raman Nagar (43) and Anekal (41) have the most cancelled trips.
- **Payments are evenly split** across credit card (26.7%), debit card (24.7%), UPI (24.7%) and cash (23.9%).
- **Fare-per-km check:** 87 trips are flagged as potential outliers out of 983.

## Recommendations
1. Add driver supply at night, when demand and revenue peak.
2. Investigate the top cancellation zones to find operational bottlenecks.
3. Review the flagged fare-per-km outliers for pricing or data issues.
4. Apply what works in top-revenue zones to the lowest-performing ones.

## What's in the Report
Demand analysis · Revenue analysis · Operational efficiency (cancellations and fare anomalies) · Insights and recommendations · Trip hour vs revenue and payment methods · Cancellation and completion analysis · Trip trends by zone and time of day · Parameter-driven zone ranking · Driver trip and earnings view

## How It's Built
- **Data model:** six tables (trips, trip details, assemblies, duration/time periods, payment methods and a zone slicer table).
- **DAX measures:** completion rate, cancellation %, revenue %, successful rides, trip counts and a fare-per-km anomaly flag.
- **Interactivity:** a parameter-driven visual that switches zone ranking between trip count, revenue and requests, plus zone slicers.
- **Custom visuals:** box-and-whisker plot for fare-per-km outliers.

## Files
```
├── Namma-Yatri-PowerBI.pbix                # Power BI report file
├── report/Namma_Yatri_PowerBI_Report.pdf   # full 10-page report (PDF export)
└── README.md
```

## Tools
Power BI Desktop · DAX

## Author
**Anju Kanwar**
