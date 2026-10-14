# Education, Salary and Working Hours Analysis

## Research Question
Does higher education level lead to higher annual salary? And how does education relate to weekly working hours? This project uses exploratory data analysis and visualization to compare workers across five education groups (from "No diploma" to "Bachelor's degree or higher").

## Dataset
- **File**: `age_salary_hours.csv`
- **Source**: Public US census-style dataset used in the CISC7204 course (University of Macau). It contains individual-level records of age, education level, annual salary, and weekly working hours.
- **Usage**: The dataset is used for academic teaching purposes only. No personal identifiable information is included.

## Methods and Tools
- **Python 3** with **pandas** for data loading and filtering (workers aged 65 or younger).
- **matplotlib** and **seaborn** for plotting.
- **squarify** for the treemap.
- Two visualizations:
  1. **Treemap** showing the proportion of workers in each education group.
  2. **Violin plots** comparing annual salary and weekly working hours across education groups.

## Key Findings
- Workers with a Bachelor's degree or higher generally show a higher annual salary distribution than workers with no diploma.
- The violin plots also reveal that higher education groups tend to have a narrower, more stable range of weekly working hours.
- The treemap shows how the sample is distributed across education categories, so the reader can judge whether each group has enough people to compare.

## Limitation
- This is an observational dataset, so the plots show correlation, not causation. Other factors (age, industry, location) are not controlled for in this simple visualization.

## How to Run
1. Install the required packages:
   ```
   pip install -r requirements.txt
   ```
2. Open `education_salary_analysis.ipynb` with Jupyter Notebook or JupyterLab.
3. Make sure `age_salary_hours.csv` is in the same folder as the notebook.
4. Run all cells top to bottom. The treemap and violin plots will display inline.

## Files
- `education_salary_analysis.ipynb` — notebook with full code and output
- `age_salary_hours.csv` — dataset
- `treemap_education.png` — treemap image
- `violin_salary_hours.png` — violin plot image
- `requirements.txt` — Python packages needed
