# Task-5 - Final-Report-Automation-Presentation

## Project
**Sales Performance Analysis using Sample Superstore Data**

Prepared for **ApexPlanet Software Pvt. Ltd.**

## Dataset
- Records after cleaning: 8,827
- Date range: 03-01-2014 to 30-12-2017
- Source file: `SampleSuperstore.csv`

## Final KPIs
| KPI | Value |
|---|---:|
| Total Sales | $819,718.06 |
| Total Profit | $98,850.43 |
| Total Orders | 4,725 |
| Total Customers | 790 |
| Total Quantity | 31,853 |
| Average Order Value | $173.49 |
| Profit Margin | 12.06% |

## Main Findings
1. **West** is the strongest region by sales ($275,810).
2. **Consumer** is the largest segment ($437,711 in sales).
3. **Office Supplies** leads category sales ($343,425).
4. **Tables** has the weakest profitability ($-8,636 profit).
5. Sales increased from $158,620 in 2014 to $272,538 in 2017.

## How to Run
```bash
pip install -r requirements.txt
python automation_pipeline.ipynb
```

The script:
- loads the raw CSV
- cleans duplicates, dates and numeric fields
- calculates KPIs
- exports `output/sales_analytics_output.xlsx`
- creates charts in `output/charts/`
- writes `output/kpi_summary.txt`

## Scheduling
A GitHub Actions workflow is included at:
`.github/workflows/daily_pipeline.yml`

It runs daily at **09:00 IST (03:30 UTC)** and can also be started manually.

## Deliverables
- Final report PDF
- PowerPoint presentation
- Automation script
- Requirements file
- README
- Processed Excel workbook
- GitHub Actions workflow
- LinkedIn final-submission post
