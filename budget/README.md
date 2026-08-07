# Hjemmebane Event Budgets

This folder contains the reusable budget model and working venue budgets for Hjemmebane.

- `event-budget-template.xlsx` is the reusable Excel template for future venues and events.
- `sola-gk-budget.xlsx` is the populated Sola GK Excel budget.
- `sola-gk-budget.md` explains assumptions, scenarios, sponsorship packages, and costs that need confirmation.
- `sola-gk-budget.csv` contains the cost lines in a spreadsheet-friendly format.
- `baerheim-golfklubb-budget.xlsx` is the populated Bærheim Golfpark / Sandnes Golfklubb Excel budget for 2027.
- `baerheim-golfklubb-budget.md` explains the Bærheim quote, assumptions, scenarios, and missing prices.
- `baerheim-golfklubb-budget.csv` contains the Bærheim cost lines in a spreadsheet-friendly format.
- `create_workbooks.py` regenerates the template and all populated Excel workbooks after structural changes to the model.

The Excel files contain four sheets: `Inputs`, `Costs`, `Sponsorship`, and `Scenarios`. Yellow cells are intended for editing; blue and green cells contain calculations and results. Formulas recalculate when the workbook opens in Excel.

All figures are in NOK. Prices are planning estimates unless explicitly marked as provided. Confirm whether quoted supplier prices include VAT before committing to a participant fee or sponsor price.
