# Vilod Excel Whitespace Audit

Find leading and trailing whitespace in selected Excel cells before
matching IDs, joining exports, or comparing text. The audit reports counts
and leaves cells unchanged.

[Download as ZIP](../../archive/refs/heads/main.zip).

## Run it in Excel

1. In a workbook with Office Scripts enabled, open **Automate > New Script**.
2. Replace the starter code with [excel_whitespace_audit.ts](excel_whitespace_audit.ts).
3. Select a single rectangular range with at most 100,000 cells.
4. Run the script. Read the two counts in **Output**.

For example, the text values `" SKU-42 "` and `"   "` yield two cells
with outer whitespace, including one whitespace-only cell.
Numbers and formula cells are skipped. The script makes no external requests.
The counting logic was tested with simulated Excel ranges.

MIT license.
