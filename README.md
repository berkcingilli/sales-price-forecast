
# Quarterly Sales Forecast Notebook – Instructions

This guide explains how to run the **quarterly_sales_forecast_notebook.ipynb** on a Windows machine using VS Code.

## 1. Install Python
Download Python (recommended 3.11 or newer):

https://www.python.org/downloads/

During installation, make sure to check:

- ✔ Add Python to PATH

---

## 2. Install VS Code

Download and install VS Code:

https://code.visualstudio.com/

After installation, install these extensions inside VS Code:

- Python
- Jupyter

You can find them in the **Extensions** tab in VS Code.

---

## 3. Prepare the Project Folder

Create a folder such as:

sales-forecast

Place the following files inside it:

- quarterly_sales_forecast_notebook.ipynb
- sales.csv
- README.md (this file)

Example structure:

sales-forecast/
│
├─ quarterly_sales_forecast_notebook.ipynb
├─ sales.csv
└─ README.md

---

## 4. Install Required Python Libraries

Open the VS Code terminal.

Run:

python -m pip install pandas numpy matplotlib scikit-learn statsmodels jupyter ipykernel

This installs the libraries required by the notebook.

---

## 5. Open the Notebook

In VS Code:

1. Open the **sales-forecast** folder
2. Open the file:

quarterly_sales_forecast_notebook.ipynb

---

## 6. Select Python Kernel

At the top right of the notebook click:

Select Kernel

Choose your installed Python interpreter.

---

## 7. Check the CSV Path

Inside the notebook confirm the following line:

CSV_PATH = "sales.csv"

If your CSV has a different name, update this value.

---

## 8. Run the Forecast

Click:

Run All

The notebook will:

1. Load the quarterly sales CSV
2. Train forecasting models
3. Predict next year's quarters
4. Display a forecast chart

---

## CSV Format

Your CSV should follow this structure:

Year,Q1,Q2,Q3,Q4
2018,120,135,128,142
2019,130,145,138,155
2020,140,150,148,160
2021,150,165,158,172
2022,165,175,170,185
2023,178,190,182,200

---

## Output

The notebook will produce:

- Forecast values for the next 4 quarters
- A chart showing historical sales and predicted values

---

## Troubleshooting

### Python not found

Run:

py -m pip install pandas numpy matplotlib scikit-learn statsmodels jupyter ipykernel

### Kernel not detected

Restart VS Code after installing packages.

---

## Notes

For best forecasting accuracy:

- Use at least **8–10 years of quarterly data**
- Avoid missing quarters
