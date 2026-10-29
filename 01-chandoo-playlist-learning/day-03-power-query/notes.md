# Day 03: Power Query, Automating Data Cleanup

**Source:** (How to use Power Query in Excel/Power BI - Perfect Guide and Chandoo.yt)
**Dataset:** Student registration data (names, emails, registration date, course, fees paid)
**Tool:** Power Query inside Excel (the same tool is also inside Power BI)

## What is Power Query?

Power Query is a data cleaning tool built into Excel (since 2013) and Power BI. It does ETL:

- **Extract:** get data from a source
- **Transform:** clean and reshape it
- **Load:** send the clean data back to Excel or Power BI

**The big idea:** Power Query records every cleaning step I do. When the source data changes, I click Refresh and all steps run again automatically. No need to clean the data by hand every time.

## Steps I followed

| # | Task | Power Query feature used |
|---|------|--------------------------|
| 1 | Remove extra rows at the top and unwanted columns | Remove Rows, Choose Columns |
| 2 | Make the first row the column names | Use First Row as Headers |
| 3 | Remove rows where important columns are blank | Filter Rows, Remove Null values |
| 4 | Remove duplicate records using the email column | Remove Duplicates |
| 5 | Create a Student ID from first name + first letter of last name | Column From Examples |
| 6 | Decide the term start date from the registration date | Conditional Column |
| 7 | Mark fee payment as Full, Part or None | Conditional Column |
| 8 | Send the clean data back to Excel as a table | Close and Load |
| 9 | Change the source data and update everything | Refresh |

## Concepts I learned

**1. Every step is recorded**
Each action (filter, remove, add column) is saved in the "Applied Steps" list on the right. I can click any step to see how the data looked at that point, or delete it.

**2. Data types matter**
Power Query needs each column set as text, number or date. This is important because conditions only work correctly on the right type. For example, comparing dates needs a Date column and checking fees needs a Number column.

**3. Column From Examples**
I type a few sample results and Power Query guesses the formula for me. I used it to build the Student ID from the name columns. It writes the M code in the background, so I don't need to code it by hand.

**4. Conditional Column**
This is an if-then-else builder with a visual screen. I used it for two business rules:

- Term start date: if the registration date is before 15 December, the term starts in February, otherwise in April
- Fee status: Full if the full fee (500) is paid, Part if less than that, None if empty

**5. Cleaning duplicates and blanks**
Removing duplicates (by email) and blank rows is just one step each, and it runs again on every refresh.

**6. Refresh**
After changing the source file, one click on Refresh updates the clean table and any pivot table made from it.

## Pivot table on clean data

After loading, I made a pivot table to summarize fees and number of students by course. This works well because the data is now clean.

## Key takeaways

- Do not clean data by hand every time, let Power Query record the steps
- Set the correct data type early, it avoids errors later
- Column From Examples is a quick way to build new columns without code
- The same skills work in Excel and in Power BI, so this is a core skill for any data analyst

## My own notes

- (write here where you got stuck, which step was new for you, what you want to try next)

## Files in this folder

- README.md (these notes)
- student-data-raw.xlsx (original data)
- student-data-clean.xlsx (after Power Query)

