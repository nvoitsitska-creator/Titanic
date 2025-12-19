# Titanic Data Analysis: Survival Insights

This project explores the Titanic dataset to understand **what factors influenced passengers’ chances of survival**. We focused on age, ticket class, deck, and family size, combining statistical analysis with visualizations to reveal interesting patterns.

## Dataset
We used the Titanic dataset from Seaborn:

- 891 passengers, 14 attributes including age, sex, class, fare, number of relatives, and survival status.

```
import seaborn as sns
df = sns.load_dataset("titanic")
```

## Libraries Used
- pandas
- numpy
- seaborn
- matplotlib

## Project Steps

1. **Data Loading & Inspection**
   - Load the dataset and inspect the first rows
   - Check column types and missing values

2. **Data Cleaning**
   - Remove duplicate rows
   - Convert column types as needed
   - Fill missing ages with the median

3. **Feature Engineering**
   - Create a new column `family_size` combining siblings/spouses and parents/children onboard
   - Add a boolean column `is_alone` indicating if a passenger traveled alone
   - Bin `age` into categories: `<14`, `14-34`, `35-59`, `60+`.

4. **Exploratory Data Analysis**
   - Frequency analysis of family size
   - Replace family sizes above 5 with `"above 5"`
   - Survival analysis by age, class, cabin, and family size
   - Visualizations: bar plots, pie charts, histograms

5. **Insights**
   - Identified age groups with the highest mortality
   - Determined which factors (age, ticket class, cabin, family size) are most associated with survival
   - Illustrated trends with clear visualizations

# Visualizations
1. Number of Relatives

Histogram: distribution of passengers by relatives
![Relatives Distribution](https://raw.githubusercontent.com/nvoitsitska-creator/Titanic/main/visualization/hist_relatives.png)

Pie chart: share of passengers by number of relatives
![Pie chart](https://raw.githubusercontent.com/nvoitsitska-creator/Titanic/main/visualization/pie_number_of_relatives.png)

2. Mortality by Age Group
Older passengers had higher mortality.
![Pie chart](https://raw.githubusercontent.com/nvoitsitska-creator/Titanic/main/visualization/pie_mortality_by_age.png)

3. Mortality by Ticket Class
3rd class: highest mortality (74%)
1st class: highest survival (37%)
![Bar chart](https://raw.githubusercontent.com/nvoitsitska-creator/Titanic/main/visualization/barplot_ticket_class.png)

4. Mortality by Cabin Deck
Passengers on decks A and G had the highest mortality.
![Bar chart](https://raw.githubusercontent.com/nvoitsitska-creator/Titanic/main/visualization/barplot_cabin_desk.png)

5. Mortality by Number of Relatives
Traveling with 5 or more relatives increases risk.
![Bar chart](https://raw.githubusercontent.com/nvoitsitska-creator/Titanic/main/visualization/barplot_relatives.png)

## Looker Studio Dashboard
Explore the interactive dashboard here: https://lookerstudio.google.com/reporting/1c4ea987-bda8-4fc1-a7c3-da9eae2ab756

## Key Insights

- Age, class, and deck location were the most important survival factors.

- Older passengers, third-class, and those on lower decks had higher mortality.
  
- Family size matters: bigger groups had lower chances of survival, likely due to slower evacuation.
  
## How to Run
```bash
# Clone repository
git clone <https://github.com/nvoitsitska-creator/Titanic_Data_Analysis.git>

# Open Jupyter Notebook
Jupyter Notebook Titanic_EDA.ipynb
```

## Author
**Anastasiia Voitsitska**

***Data Analyst***

📌 This project is part of my data analytics portfolio and demonstrates practical skills in data analysis,
data visualization, and insight communication.
