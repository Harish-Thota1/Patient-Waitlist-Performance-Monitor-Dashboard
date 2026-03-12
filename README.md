# Patient Waitlist Performance Monitor

## Overview
A 3-page interactive Power BI dashboard analysing 2.46M+ patient waitlist records 
across 20+ hospital specialties, tracking wait times by age group, case type, and 
time band from 2018 to 2021. Built to help health administrators identify bottlenecks, 
monitor trends, and prioritise patient care decisions.

---

## Objectives
- Monitor patient waitlist volumes across 20+ hospital specialties, age groups, 
  and case types in a single unified view
- Identify which patient cohorts are waiting the longest and flag those at risk 
  of breaching the 18 month threshold
- Track month on month waitlist trends and year over year performance to support 
  executive level decision making
- Enable operational teams to drill into specialty level and age band data to 
  take targeted, timely action

---

## Dashboard Pages
| Page | Description |
|---|---|
| Summary | KPI cards, donut chart for case type split, column chart for time band vs age profile, monthly trend line and top 5 specialties |
| Details | Hierarchical matrix drillable by specialty, age group, and wait time band with date, case type, and specialty slicers |
| Drill Down | Specialty group bar chart with total waitlist card for drillthrough analysis |

---

## Screenshots
> 📁 All screenshots are stored in the `images` folder

### Summary Page
![Summary Page](images/summary-page.png)
*KPI cards, case type split, age profile breakdown and monthly trend analysis*

### Details Page
![Details Page](images/details-page.png)
*Hierarchical matrix showing waitlist breakdown by specialty, age group and wait time band*

### Drill Down Page
![Drill Down Page](images/drilldown-page.png)
*Specialty group bar chart with total waitlist card for drillthrough analysis*

---

## What I Built
- Engineered a dynamic Average/Median toggle using a DAX driven parameter table, 
  enabling clinicians to switch statistical views instantly without duplicating a 
  single measure
- Unified multi period monthly snapshot files into a single fact table using Power 
  Query Append, joined to a specialty mapping dimension for clean hierarchical reporting
- Built a 3 level drillthrough hierarchy (Specialty → Age Group → Wait Time Band) 
  with back navigation Action Buttons, replicating enterprise BI UX standards
- Delivered year over year KPI comparison using DAX time intelligence, giving 
  leadership an instant read on whether waitlist volumes are improving month on month
- Segmented 2.46M+ records across 3 age bands and 7 time bands (0 to 3 months 
  through to 18+ months) to pinpoint high risk patient cohorts requiring urgent 
  intervention
- Applied a custom branded theme with conditional formatting, making critical 
  outliers visually immediate without any manual analysis

---

## Key Insights
- Orthopaedics carried the heaviest waitlist burden with 84,856 patients as of 
  March 2021, making it the highest priority specialty for capacity planning
- Outpatients dominated across all specialties, signalling systemic pressure on 
  outpatient clinic capacity rather than bed availability
- The 65+ age group in Orthopaedics had a disproportionately high number of 
  patients in the 18+ month band, indicating elderly patients were most at risk 
  of prolonged waits
- Paediatric specialties (Radiology, Neurosurgery, Oncology) showed low absolute 
  volumes but consistent presence in longer wait bands, a quality of care risk 
  given the vulnerability of the cohort
- Total waitlist grew to 2.46M records over the 3 year period, suggesting demand 
  consistently outpaced capacity across the system

---

## Recommendations
- Prioritise Orthopaedic capacity expansion as the volume and proportion of 18+ 
  month waiters in the 65+ cohort represents both a clinical and compliance risk 
  against national wait time standards
- Shift outpatient delivery model as the outpatient heavy distribution suggests 
  virtual or community based consultations could decompress waitlist pressure 
  without additional inpatient infrastructure
- Introduce specialty level wait time targets in the dashboard to trigger automated 
  alerts when a cohort crosses a threshold, moving the tool from descriptive to 
  prescriptive analytics
- Add a proper Date Table to the data model to unlock full DAX time intelligence 
  capabilities and enable more sophisticated forecasting of waitlist trajectory
- Expand data coverage beyond 2021 to make the trend analysis actionable for 
  current operational planning

---

## Tech Stack
- Power BI Desktop
- DAX
- Power Query (M)
- Data Modelling
- Time Intelligence
- Drillthrough Navigation
- Conditional Formatting
- Custom Themes

---

## Contact
**Harish Thota**  
Data Engineer and Business Analyst  
harishthota001@gmail.com  
[Portfolio](https://harish-thota1.github.io/Analyst-Portfolio/) · 
[LinkedIn](https://www.linkedin.com/in/harish-thota/)
```

---

**Your folder structure should look like this in GitHub:**
```
Patient-Waitlist-Dashboard/
│
├── images/
│   ├── summary-page.png
│   ├── details-page.png
│   └── drilldown-page.png
│
├── Health_Dashboard.pbix
└── README.md
