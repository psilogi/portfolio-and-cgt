# portfolio-and-cgt

Spreadsheet and apps script to create a portfolio tracker and cgt calculator (First-In-First-Out) in Google Sheets.
Relies on data exported from Self Wealth's 'Movements' Reports.
Only set up for use with ASX listed companies.

Steps:
- Upload XLSX to Google Sheets, open, and "Save to Google Sheets".
- Open Extensions > Apps Script and paste in the provided code.
- Rename, save, and reload spreadsheet to give permissions.
- Export all trades at Self Wealth > Trading Account > Reports > Movements > Time Period > Custom.
- Copy all Trade data into "Trades" sheet.
- Access either "Portfolio Summary" or "CGT Calculator" sheet (Choose financial year in "CGT Calculator", cell B1)
- Run "CGT Tools" from Spreadsheet menu bar to, either, Update your portfolio summary or calculate cgt.
- Add graphs or other visualisations - e.g., pie chart with Column A and Column I to visualise current market holdings by stock ticker.

Updating/Adding additional financial years:
- select cell B1 in "CGT Calculator"
- select Date > Data validation
- select rule labelled B1
- "Add another item" using the format YYYY-YYYY for the financial year of interest
  - e.g., 2004-2005 for 1/07/2004 - 30/06/2005.

NOTES:
- Calculation and portfolio is only as good as the Trade data you enter.
- Any other platforms with different columns for exportswill need additional massaging
- If SW updates their export format, the calculations will not function correctly.
- Delisted stocks can be listed at C10 (e.g, 'ABC,XYZ,QRS')
  - I had to do this for a stock that was delisted. I can no longer sell the shares so they are counted as a loss
