
# HR Analytics Dashboard - Power BI Project

This project is an interactive **HR analytics dashboard** created in Power BI.  
It provides insights into:
- Overtime hours per department
- Total business trips by unit
- Employee demographics (optional)
- And more...

## Demo

![Dashboard Screenshot](https://github.com/mhrhpr/HR_analytics_dashboard/powerbi_images.zip)

---

## 1. Data

The data is originally provided in Excel format and is stored in the `data/` folder.

- `raw_data.xlsx`: The raw data collected from the HR system
- `cleaned_data.xlsx`: Cleaned and preprocessed data used for the Power BI visuals

---

## 2. Power BI Report

The Power BI file is located in the `powerbi/` folder:
- `hr_dashboard.pbix`: The main Power BI report with all visuals and filters

---

## 3. Python Script (Optional)

To clean and transform the data before using it in Power BI, a Python script was used.

Path: `scripts/prepare_data.py`

```python
# Sample code used in the script:
import pandas as pd

df = pd.read_excel('data/raw_data.xlsx')
df.dropna(inplace=True)
df.to_excel('data/cleaned_data.xlsx', index=False)
