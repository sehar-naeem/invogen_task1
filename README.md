# Inovegen Internship — Week 1 Assignment
## Task 1: Data Cleaning & Exploratory Data Analysis (EDA)

### 📌 Project Overview
This repository contains the complete Data Cleaning and Exploratory Data Analysis (EDA) workflow for the Titanic passenger dataset as part of the Inovegen AI/ML Internship Program 2026.

### 📊 Dataset Source
- **Source:** [Titanic Dataset (Data Science Dojo)](https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv)
- **Dimensions:** 891 rows, 12 initial features

---

### 🛠️ Key Steps Performed

1. **Data Inspection:**
   - Inspected dataset shape, column types, and numerical statistics.
   - Identified missing values: `Cabin` (77.1%), `Age` (19.9%), `Embarked` (0.22%).
   - Verified that there are 0 duplicate records.

2. **Data Cleaning Decisions:**
   - **`Cabin`:** Dropped the column due to excessive missingness (>77%).
   - **`Age`:** Imputed missing values using the **median age (~28 years)** to preserve all 177 affected passenger records without skew from outliers.
   - **`Embarked`:** Imputed missing entries with the **mode ('S' - Southampton)**.
   - **Redundant Features:** Removed `Ticket` and `PassengerId` identifiers.

3. **Visualizations Included:**
   - **Chart 1:** Overall Passenger Survival Count (Perished vs. Survived).
   - **Chart 2:** Survival Breakdown by Gender (Demonstrating female survival advantage).
   - **Chart 3:** Survival Breakdown by Passenger Class (1st, 2nd, and 3rd class disparity).
   - **Chart 4:** Passenger Age Distribution by Survival Outcome.
   - **Bonus Chart:** Correlation Heatmap of numerical features.

---

### 💡 Key Insights & Findings

1. **Gender Impact:** Female passengers had an overwhelming survival rate (~74%) compared to male passengers (~19%), reflecting the enforcement of the "women and children first" protocol.
2. **Socio-Economic Disparity:** Class 1 passengers had a survival rate exceeding 62%, whereas Class 3 passengers suffered the highest mortality (~24% survival rate) due to deck location and access delays.
3. **Age Vulnerability:** Children aged 0–5 had higher survival rates due to priority boarding, whereas young adults (18–35) made up the highest number of casualties.
4. **Overall Survival:** Only 38.4% (342 passengers) survived the disaster, highlighting the shortage of lifeboats.
5. **Data Preservation:** Thoughtful imputation retained 100% of the 891 passenger records rather than deleting ~78% of data.

---

### 💻 Technologies Used
- **Python 3**
- **Pandas** (Data manipulation and cleaning)
- **Matplotlib & Seaborn** (Data visualization)
- **Google Colab / Jupyter Notebook**
