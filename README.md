Exploratory Data Analysis (EDA) of the Titanic dataset using Python. Investigates factors affecting passenger survival such as age, ticket class, cabin deck, and family size, with visualizations and key insights.

# Titanic Data Analysis Project

This project performs a comprehensive exploratory data analysis (EDA) on the Titanic dataset from the Seaborn library using Python. The analysis focuses on understanding factors that influenced passenger survival.

## Libraries Used
- pandas
- numpy
- seaborn
- matplotlib

## Project Steps

1. **Data Loading & Inspection**
   - Load the dataset and inspect first rows
   - Check column types and missing values

2. **Data Cleaning**
   - Remove duplicate rows
   - Convert column types as needed
   - Fill missing ages with median

3. **Feature Engineering**
   - Create a new column `family_size` combining siblings/spouses and parents/children onboard
   - Add a boolean column `is_alone` indicating if a passenger traveled alone
   - Bin `age` into categories: `<14`, `14-34`, `35-59`, `60+`

4. **Exploratory Data Analysis**
   - Frequency analysis of family size
   - Replace family sizes above 5 with `"above 5"`
   - Survival analysis by age, class, cabin, and family size
   - Visualizations: bar plots, pie charts, histograms

5. **Insights**
   - Identified age groups with the highest mortality
   - Determined which factors (age, ticket class, cabin, family size) are most associated with survival
   - Illustrated trends with clear visualizations

## How to Run
```bash
# Clone repository
git clone <repo-url>

# Open Jupyter Notebook
jupyter notebook Titanic_EDA.ipynb
