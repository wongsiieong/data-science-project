# Education, Salary and Working Hours Analysis

## Research Question
Does a higher education level correspond to a higher annual salary, and how does education relate to weekly working hours? This project compares workers across five education groups using exploratory data analysis and visualization.

## Dataset
- **File**: `age_salary_hours.csv`
- **Source**: dataset provided for the CISC7204 course teaching exercise (University of Macau).
- **Usage permissions**: used for academic teaching and analysis only. The file contains no personal identifiable information.
- **Columns**: `Age`, `Annual Salary`, `Weekly hours`, `Education`. The currency unit is not specified in the source file.
- **Sample**: 500 rows in total; 385 rows remain after filtering to workers aged under 65.

## Methods and Tools
- **Python 3**, **pandas** for loading the data and applying the age filter.
- **squarify** for a treemap showing the sample share of each education group.
- **matplotlib** and **seaborn** for violin plots comparing annual salary and weekly hours across groups.
- The filtered sample is summarized by education group (sample size, salary median and mean, hours median and mean) before plotting.

## Key Findings
- Workers with a **Bachelor's degree or higher** have the highest salary distribution: median 61,000 and mean about 89,963 (n = 195).
- The other four groups have salary medians between about 20,400 and 38,000. Salary does **not** increase monotonically with education; the small "No diploma" group (n = 11) has a median of 38,000.
- Weekly working hours are similar across groups (median 37–40 hours). The data do not show a clear monotonic relationship between education and weekly hours.

## Limitations
- This is observational data, so the plots show correlation, not causation. Age, industry, and location are not controlled for.
- The dataset contains zero salary values (65 rows) and zero hour values (54 rows); these were kept rather than separately coded.
- The filtered sample has 385 rows, and some education groups are small, so group comparisons are not equally reliable.
- The currency unit is not stated in the source file.

## Reproduction Instructions
1. Install the required packages:
   ```
   pip install -r requirements.txt
   ```
2. Place `age_salary_hours.csv` in the same folder as `education_salary_analysis.ipynb`.
3. Open the notebook with Jupyter Notebook or JupyterLab and run all cells top to bottom.
4. The two figures are saved to `images/`:
   - `images/treemap_education.png`
   - `images/violin_salary_hours.png`

## Files
- `education_salary_analysis.ipynb` — analysis notebook with code, outputs, and figure exports
- `age_salary_hours.csv` — dataset
- `images/treemap_education.png` — sample distribution by education level
- `images/violin_salary_hours.png` — salary and weekly hours by education level
- `requirements.txt` — Python packages required to run the notebook
