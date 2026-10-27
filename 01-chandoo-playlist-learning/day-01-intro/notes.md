# Day 01: Introduction to Power BI and My First Report

**Source:** Chandoo Power BI playlist, Video 1
**Dataset:** Awesome Chocolates (shipment data for 2022, 6 columns, about 1,000 rows)

## What is Power BI?

Power BI is a free tool from Microsoft (Power BI Desktop) that helps me turn raw data into charts, reports and dashboards. It can pull data from Excel files, SQL Server databases, or even typed-in data.

## What I did today

1. Installed Power BI Desktop
2. Imported the Excel file using "Import data from Excel"
3. Picked the right sheet in the Navigator window and loaded the data
4. Built my first visuals (column chart, bar chart, line chart)
5. Tried cross-filtering, drill down and the AI "Explain the decrease" feature
6. Saved my report as a .pbix file

## Power BI screen: 3 main parts

| Part | What it does |
|------|--------------|
| Ribbon (top) | Menu with all the features, similar to Excel or Outlook |
| Canvas (center) | The dotted area where my charts and tables appear |
| Right-side panels | Visualizations pane (to pick and format charts) and Fields pane (list of my data columns) |

## Charts I built

- **Column chart:** Country on X-axis, Boxes Shipped on Y-axis. Australia shipped the most, New Zealand the least.
- **Bar chart:** Product on Y-axis, Boxes Shipped on X-axis. Shows shipments per product.
- **Line chart:** Date on X-axis to see the trend over time.

I also learned to change chart colors from the Format pane.

## Cool things I learned

**1. Visuals talk to each other (cross-filtering)**
Click a country in one chart and the other charts update to show only that country. Click again to reset. Hovering on any bar shows a tooltip with exact numbers.

**2. Date hierarchy and drill down**
Power BI automatically splits a Date column into Year > Quarter > Month > Day. I can drill down from year to quarter to month using the buttons on the chart. In the monthly view, sales started strong in January, dipped in February and recovered in March.

**3. AI insight: Explain the decrease**
Right-click on the February dip and Power BI explains why sales fell. It found that several products had much lower shipments that month.

## Saving and sharing

- File > Save stores the report on my computer as a .pbix file
- To share with others, I have to publish it to the Power BI service (needs sign-in)
- Sharing inside a company needs Power BI Pro or Premium licenses

## Key takeaways

- Power BI Desktop is free, so anyone can start practicing
- Charts are interactive by default, no extra setup needed
- Date fields get a built-in hierarchy, which makes time analysis easy
- Built-in AI features can save time when finding the reason behind a change in data

## Questions / things to explore next

- How to clean data using Power Query before loading it
- Other chart types and when to use each one

## Files in this folder

- README.md (these notes)
- report.pbix (my Day 1 report)
- screenshot.png (my dashboard)
