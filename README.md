# Salla Call Center Performance Analysis

A call center performance analysis covering February to April 2022, using Excel Power Query, Power BI, and DAX to review call volume, service levels, abandonment, forecasting, and response times across three projects.

## Overview

This project examines Salla's call center operations to identify service bottlenecks, compare project and agent performance, and recommend improvements to staffing, forecasting, and customer experience.

## Dashboard

![[Salla Call Center Performance Dashboard](https://github.com/Omar1564/salla-call-center-analysis/blob/main/Salla%20Call%20Center%20Performance.pbix)](dashboard.png)

## Dataset

- **Period:** February, March, and April 2022
- **Size:** 267 operational records
- **Projects:** Project A, Project B, and Project C
- **Analysis areas:** Offered, handled, forecasted, and abandoned calls; service level; average speed of answer; and agent performance

## Tools

| Tool | Use |
| --- | --- |
| Microsoft Excel / Power Query | Data processing and cleaning |
| Power BI Desktop | Data modeling and dashboard development |
| DAX | Measures for performance analysis |
| Power BI visualizations | Dashboard design and presentation |

## Key Performance Indicators

| KPI | Result |
| --- | ---: |
| Total offered calls | 1,744,885 |
| Total handled calls | 1,721,842 |
| Overall service level (SLA) | 91.06% |
| Abandoned calls | 23,043 |
| Abandonment rate | 1.32% |
| Forecast accuracy | 71.60% |
| Weighted average speed of answer (ASA) | 14.30 seconds |

## Key Findings

### Call volume and forecasting

- **March was the busiest month:** 876,199 offered calls, compared with approximately 0.45 million in February and 0.42 million in April.
- **Abandonment was concentrated in March:** 18,802 calls were abandoned, representing over 81% of all abandoned calls and a monthly abandonment rate of 2.15%.
- **Forecasts exceeded actual volume in every month:** Approximately 2.44 million calls were forecast against 1.74 million offered calls. April had the largest gap, with approximately 0.75 million forecast calls versus 0.42 million offered calls.

### Project performance

| Project | SLA | Abandonment rate | Observation |
| --- | ---: | ---: | --- |
| Project A | 91.50% | 0.97% | Maintained a service level above 91% and abandonment below 1%. |
| Project B | 90.33% | 1.66% | Handled the largest volume share, with the lowest SLA and highest abandonment rate. |
| Project C | 95.16% | 0.86% | Achieved the highest SLA and lowest abandonment rate. |

Project B also recorded the highest accumulated ASA at 1,039.51 seconds, while Project C recorded the lowest at 520.13 seconds. These are sums of ASA, not project-level average response times; the overall weighted ASA is reported separately above.

### Agent performance

- **Highest abandonment rates:** Huda (2.97%), Youssef (2.75%), and Dina (2.59%).
- **Lowest abandonment rates:** Laila (0.34%), Samir (0.38%), and Sara (0.39%).

## Recommendations

### Improve operational performance

1. **Align staffing with peak demand.** Reallocate shifts during high-volume periods like March to reduce queue pressure and abandoned calls.
2. **Introduce IVR and callback options.** Offer self-service and virtual callbacks during long waits, particularly for Project B.
3. **Recalibrate call forecasts.** Address persistent overestimation to reduce unnecessary staffing during lower-volume months such as April.
4. **Provide targeted agent coaching.** Focus response-time and call-handling training on agents with higher abandonment rates, using low-abandonment agents as benchmarks.

### Support sales opportunities

1. **Reduce missed customer contacts.** Treat the 23,043 abandoned calls as opportunities to improve customer access and reduce potential lost orders.
2. **Apply Project C's service practices across projects.** Use its high-SLA performance as a benchmark for faster service and potential upsell or cross-sell opportunities.
3. **Connect call metrics with CRM sales data.** Measure conversion rates alongside service and handling metrics to assess the relationship between call center performance and sales.

These are proposed actions, not measured results of implemented changes.

## Repository Structure

```text
salla-call-center-analysis/
├── README.md       # Project overview, findings, and recommendations
└── dashboard.png   # Power BI dashboard screenshot
```

This repository package contains the project summary and a static dashboard preview. The underlying dataset and Power BI project file are not included in this package.
