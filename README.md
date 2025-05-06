# Monthly Billing Report Generator

This project calculates monthly billing for office inventory based on active periods of usage. It processes a list of items and outputs a structured billing summary for a given month.

## 📂 Files Included

- `monthly_bill_generator.ipynb` – Main Jupyter Notebook for generating monthly bills.
- `input_items.json` – Sample data file containing item details with start and stop dates.
- `billing_report_output.json` – (Optional) Output file showing the billing results for a specific month.

## ⚙️ How It Works

The notebook:
1. Loads item data from `input_items.json`.
2. Filters items active during the selected month.
3. Calculates prorated billing amounts.
4. Groups results by `item_code`.
5. Outputs the final bill in JSON format.

### Output Example:
```json
{
  "line_items": [
    {
      "item_code": "Executive Desk (4*2)",
      "rate": 1080.0,
      "qty": 25,
      "amount": 27000.0,
      "billing_period": "2024-11-01 to 2024-11-30"
    }
  ],
  "total_revenue": 72000.0
}

▶️ Running the Notebook
Clone the repo or download the notebook.

Open in Jupyter or VSCode.

Ensure input_items.json is in the same directory.

Run all cells to generate the report.

📌 Requirements
Python 3.x

Jupyter Notebook

datetime and json (standard libraries)
