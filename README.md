# Investment Analysis Dashboard

## Project Overview
This project analyzes investor preferences, behavior, savings objectives, investment duration, expected returns, and information sources using **Python** and **Power BI**.

The project was completed as part of the **Cognifyz Technologies Business Analytics Internship**. The internship task document defines 10 tasks across Beginner, Intermediate, Advanced, and Expert levels, including data overview, gender distribution, descriptive statistics, investment preferences, savings objectives, information sources, investment duration, expectations, and correlation analysis.
##Power BI Data Model

<p align="center">
  <img src="images/data-model.png" alt="Power BI Data Model" width="1000">
</p>
## Objectives
- Understand the structure of the investment dataset.
- Analyze investor demographics and investment preferences.
- Identify the most preferred investment avenue.
- Study reasons behind investment choices.
- Analyze savings objectives and information sources.
- Estimate average investment duration.
- Summarize expected investment returns.
- Explore relationships between age, investment duration, and expected returns.
- Build an interactive Power BI dashboard to present key findings.

## Dataset
The dataset contains **40 records and 24 original columns**.

Important fields used in the analysis include:
- `gender`
- `age`
- `Avenue`
- `Duration`
- `Expect`
- `Reason_Mutual`
- `Source`
- `What are your savings objectives?`
- `Mutual_Funds`
- `Equity_Market`
- `Debentures`
- `Government_Bonds`
- `Fixed_Deposits`
- `PPF`
- `Gold`

Additional numeric fields such as `Duration_Numeric` and `Expect_Numeric` were created where required for calculations and correlation analysis.

## Tools & Technologies
- **Python**
- **Pandas**
- **Matplotlib**
- **Jupyter Notebook**
- **Power BI**
- **Power Query**
- **DAX**

## Tasks Performed

### Task 1 — Data Overview
Loaded the dataset with Pandas and examined its rows, columns, data types, and overall structure.

### Task 2 — Gender Distribution
Analyzed the gender column and created a visualization to compare the number of male and female participants.

### Task 3 — Descriptive Statistics
Identified numerical columns and calculated:
- Mean
- Median
- Standard deviation

### Task 4 — Most Preferred Investment Avenue
Performed frequency analysis on the `Avenue` column.

**Key Finding:** Mutual Fund is the most preferred investment avenue, selected by **18 participants**.

### Task 5 — Reasons for Investment
Analyzed `Reason_Mutual` to identify recurring reasons for investing in mutual funds.

### Task 6 — Savings Objectives
Analyzed the `What are your savings objectives?` field to identify the main financial goals of participants.

### Task 7 — Common Information Sources
Analyzed the `Source` column to determine where participants obtain investment information.

**Key Finding:** Financial Consultants are the most common information source, used by **16 participants**.

### Task 8 — Investment Duration
Converted categorical investment-duration ranges into approximate numeric values:

| Duration | Approx. Years |
|---|---:|
| Less than 1 year | 0.5 |
| 1-3 years | 2 |
| 3-5 years | 4 |
| More than 5 years | 6 |

**Average Investment Duration:** approximately **2.98 years**.

> The numeric values are representative values used to estimate an average from categorical ranges.

### Task 9 — Expectations from Investments
Analyzed the `Expect` column to summarize the return ranges expected by participants.

For numerical analysis, expected-return ranges can be represented by their midpoints:
- `10%-20%` → 15
- `20%-30%` → 25
- `30%-40%` → 35

### Task 10 — Correlation Analysis
Explored potential relationships between:
- Age and Investment Duration
- Age and Expected Return
- Investment Duration and Expected Return

Scatter plots and trend lines can be used in Power BI to visualize these relationships. Numeric proxy columns are used because `Duration` and `Expect` are stored as categorical ranges.

## Power BI Dashboard

The main dashboard includes four KPI cards:

- **Total Participants:** 40
- **Average Age:** 27.80 years
- **Most Preferred Avenue:** Mutual Fund
- **Average Investment Duration:** 2.98 years

Dashboard visualizations include:
- Preferred Investment Avenue
- Reasons for Mutual Fund Investment
- Savings Objectives
- Sources of Investment Information
- Investment Duration Distribution
- Expected Investment Returns

A separate correlation section/page can contain scatter plots for the three relationships analyzed in Task 10.

## Dashboard Theme

| Element | HEX |
|---|---|
| Header / Dark Navy | `#172554` |
| Primary Blue | `#2563EB` |
| Teal | `#0D9488` |
| Amber Accent | `#F59E0B` |
| Dashboard Background | `#F5F7FA` |
| Card Background | `#FFFFFF` |
| Main Text | `#1E293B` |

## Project Files
```text
Investment-Analysis/
│
├── Data_set 2 - Copy.csv
├── main.ipynb
├── Investment Analysis Plan.pbix
└── README.md
```

## Key Insights
- The dataset contains **40 participants**.
- The average participant age is **27.80 years**.
- **Mutual Fund** is the most preferred investment avenue.
- Mutual Fund was selected by **18 participants**.
- **Financial Consultants** are the most common source of investment information.
- The estimated average investment duration is **2.98 years**.
- Correlation analysis helps explore whether age, investment duration, and expected returns move together.

## How to Run

### Python Analysis
1. Place the CSV file and notebook in the same folder.
2. Open `main.ipynb` in Jupyter Notebook or VS Code.
3. Install the required libraries if necessary:
   ```bash
   pip install pandas matplotlib
   ```
4. Run the notebook cells sequentially.

### Power BI Dashboard
1. Open the `.pbix` file in Power BI Desktop.
2. If Power BI asks for the dataset location, update the CSV source path.
3. Refresh the data.
4. Open the report pages to explore the dashboard and correlation visuals.

## Note
The mappings used for investment duration and expected-return ranges are approximate numeric representations of categorical ranges. They are useful for summary statistics and exploratory correlation analysis but should not be interpreted as exact participant values.

## Author
**Jatindra Kumar Soni**

## Acknowledgement
Project completed as part of the **Cognifyz Technologies Business Analytics Internship Program**.
