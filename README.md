# cancer_regression
Analysis of cancer related statistics
# 🧬 Cancer Mortality Rate Analysis

This project explores and analyzes a real-world dataset of cancer-related statistics across various U.S. counties. The main objective is to understand factors influencing cancer **death rates** and to build predictive models using Python.

---

## 📁 Dataset

The dataset contains **3047 rows** and **33 columns**. It includes variables such as:

- `target_deathrate` – **Target variable** representing cancer-related death rates
- Demographic data (e.g., `medianage`, `pctwhite`, `pctblack`)
- Economic indicators (e.g., `medincome`, `povertypercent`)
- Health coverage statistics (e.g., `pctprivatecoverage`, `pctpubliccoverage`)
- Education levels by age group

---

## 📊 Steps Performed

### ✅ Step 1: Data Overview
- Loaded the dataset using `pandas`
- Reviewed missing values, datatypes, and basic statistics
- Identified target column: `target_deathrate`

### ✅ Step 2: Data Cleaning
- Columns with missing values:
  - `pctsomecol18_24`: ~75% missing → likely dropped
  - `pctprivatecoveragealone`: ~20% missing → imputed or assessed
  - `pctemployed16_over`: ~5% missing → imputed
- Checked for outliers and strange values (e.g., extreme `medianage`)

  target_deathrate	Number of cancer-related deaths per 100,000 people in the county (this is the target variable we're predicting).

📈 Cancer Statistics
Column Name:Meaning
avganncount-	Average number of new cancer cases per year in the county.
avgdeathsperyear-	Average number of cancer deaths per year.
incidencerate-	Rate of new cancer cases per 100,000 people.

💰 Economic Features
Column Name:Meaning
medincome- Median household income in the county.
povertypercent-	Percentage of people living below the poverty line.
binnedinc- Income grouped into bins/ranges for easier analysis.

👥 Demographic Features
Column Name:Meaning
popest2015-Population estimate for 2015.
medianage-Median age of all residents.
medianagemale-Median age of male residents.
medianagefemale-Median age of female residents.
birthrate-Births per 1,000 people in the population.
geography-County and state name (e.g., "Los Angeles County, California").

👨‍👩‍👧‍👦 Marital & Household Info
Column Name:Meaning
percentmarried- Percentage of adults who are married.
pctmarriedhouseholds- Percentage of households headed by married couples.

🏫 Education by Age Group
Column Name:Meaning
pctnohs18_24-	% of people aged 18–24 with no high school diploma.
pcths18_24- % of people aged 18–24 with only a high school diploma.
pctsomecol18_24- % of people aged 18–24 with some college education (no degree).
pctbachdeg18_24- % of people aged 18–24 with a bachelor’s degree or higher.
pcths25_over- % of people aged 25+ with at least high school education.
pctbachdeg25_over- % of people aged 25+ with a bachelor’s degree or higher.

💼 Employment
Column Name:	Meaning
pctemployed16_over-	% of population aged 16+ who are employed.
pctunemployed16_over-	% of population aged 16+ who are unemployed.

🏥 Health Insurance Coverage
Column Name:	Meaning
pctprivatecoverage- % of people with any private insurance.
pctprivatecoveragealone-	% with only private insurance (no public insurance).
pctempprivcoverage-	% with employer-provided private insurance.
pctpubliccoverage-	% with any public insurance (e.g., Medicaid).
pctpubliccoveragealone-	% with only public insurance (no private insurance).

🌍 Race/Ethnicity Breakdown
-Column Name:	Meaning
-pctwhite -	% of the population that is White.
-pctblack	- % that is Black or African American.
-pctasian	- % that is Asian.
-pctotherrace	- % that falls under "Other race" categories.



### ✅ Step 3: Exploratory Data Analysis (EDA)
- Visualized distributions using Seaborn and Matplotlib
- Generated correlation heatmaps to identify strong predictors of `target_deathrate`

### ✅ Step 4: Modeling
- Applied regression models:
  - Linear Regression
  - Ridge & Lasso Regression
  - Random Forest
- Evaluated performance using metrics like R² and RMSE

## 🛠 Technologies Used

- Python 3
- Pandas & NumPy
- Seaborn & Matplotlib
- Scikit-learn

## 🚀 Future Improvements

- Handle high-missing-value features with more advanced imputation
- Use feature engineering to improve model accuracy
- Try classification (e.g., high vs low death rate buckets)
- Deploy as a web app using Streamlit or Flask

## 📌 License

This project is for educational and portfolio purposes only.
https://www.kaggle.com/datasets/varunraskar/cancer-regression

## 🙋‍♀️ Author

**Daisy Faith**  
Currently studying Data Science, ML, and AI at Cube Hub Academy  
🧠 Passionate about solving real-world problems with data!
