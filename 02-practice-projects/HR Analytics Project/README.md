# HR Analytics & Attendance Dashboard (Power BI)

An end-to-end HR analytics dashboard built in **Power BI** using three months of attendance data (April, May, June 2022) from the fictional company **AtliQ Technologies**. The project was built as hands-on practice to understand how Power BI is used in real business settings, from raw data cleaning to a decision-ready dashboard.

> Built while following the Codebasics Power BI project playlist, then implemented and tested on my own.

---

## Dashboard Preview

![Dashboard](images/dashboard.png)

*(Add your final dashboard screenshot at `images/dashboard.png`)*

---

## Business Problem

AtliQ's HR team wanted clear answers to a few questions about attendance and absence:

1. **What percentage of employees are taking sick leave, and what is the reason behind it?**
2. **On which day of the week do most people take leave?** This helps the company schedule important meetings on the day when the maximum number of people can attend.
3. **What is the split between Work From Home (WFH) and in-office presence** in the hybrid setup?
4. **Out of the total working days, how many days were employees actually present?**

---

## What the Dashboard Answers

### Key KPIs (custom DAX measures)

| KPI | Purpose |
|---|---|
| **Total Working Days** | Total working days in the selected period |
| **Present Days** | Total days employees were present |
| **Present %** | Present days as a share of working days |
| **WFH %** | Share of days worked from home |
| **Sick Leave (SL) %** | Share of days lost to sick leave |

### Visuals

- **Daily Attendance Volume**: area chart showing attendance behaviour across all 3 months, useful for spotting dips and patterns over time.
- **WFH % and SL % by Day**: line chart comparing remote work and sick leave trends by date.
- **Employee Daily Attendance & Status Grid**: matrix with employees as rows and days of the month (1, 2, 3 ...) as columns, color-coded by status (P, WFH, SL, etc.), along with per-employee Attendance % and WFH %.

---

## Tech Stack

- **Power BI Desktop**: data modelling and visualisation
- **Power Query**: data cleaning and transformation
- **DAX**: calculated measures and columns

---

## Workflow

1. **Understand the requirement**: translated the HR team's questions into measurable KPIs.
2. **Clean the data in Power Query**: cleaned one month's sheet fully and built the steps so they can be reused.
3. **Reuse the cleaning logic**: the other monthly sheets had the same structure but were raw. Using the **Advanced Editor**, I reused the same query by just changing the data source instead of repeating every step.
4. **Model the data and write DAX**: created calculated columns and measures for the five KPIs.
5. **Build the visuals**: KPI cards, trend charts, and the attendance matrix.
6. **Validate and refine**: checked the numbers against the questions the business asked.

---

## What I Learned

- Writing **calculated measures and columns** in DAX through a practical use case
- Understanding a **business requirement** and turning it into a dashboard
- **Asking the right questions** of a dataset and answering them with data
- Using **Power Query** efficiently, including the **Advanced Query Editor** to apply the same cleaning steps to other raw sheets by changing only the data source
- Gaining the confidence to implement similar projects independently

---

## Key Insights

> Fill in your own findings from the dashboard here, for example:

- Sick leave rate overall: **1.94%**
- Day of the week with the highest absence: **FRIDAY** (best day to avoid scheduling meetings)
- Best day for important meetings: **MONDAY or TUESDAY**
- WFH share: **10%**

---

## Repository Structure

```
├── README.md
├── data/            # Raw and cleaned attendance sheets
├── images/          # Dashboard screenshots
└── HR_Analytics_Dashboard.pbix
```

*(Adjust to match your actual repo.)*

---

## How to Use

1. Clone this repository.
2. Open `HR_Analytics_Dashboard.pbix` in Power BI Desktop.
3. If prompted, update the data source path to the `data/` folder.
4. Refresh the data and explore using the date slicers.

---

## Acknowledgements

Learning resource: the **Codebasics** Power BI project playlist on YouTube. Dataset context: AtliQ Technologies (practice dataset).

---

## Connect

**GitHub:** [Syznx](https://github.com/Syznx)
