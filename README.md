# City-Cycle Fuel Consumption Analysis  

This repository contains an end-to-end analysis of the **City-Cycle Fuel Consumption Dataset**. The work is divided into two main parts:  

1. **Exploratory Data Analysis (EDA)**  
2. **Statistical Analysis**  

The goal is to better understand the dataset and to use statistical tools to validate insights, with a particular focus on predicting the **miles per gallon (mpg)** attribute.  

---

## 📊 Dataset Description  

- **Instances**: 398  
- **Attributes**: 8 (3 categorical / multi-valued discrete, 5 continuous)  
- **Target Variable**: `mpg` (miles per gallon)  
- **Special Notes**:  
  - 8 instances with missing values for `mpg` were removed.  
  - One attribute (`car name`) is a string unique to each record.  
  - Dataset contains missing values in other attributes.  
- **Task Type**: Regression (predicting `mpg`)  

**Source**:  
This dataset is a modified version from the **StatLib library** at Carnegie Mellon University.  
It was used in the **1983 American Statistical Association Exposition**.  
Later employed by **Ross Quinlan (1993)** in regression tasks.  

📂 Original dataset: `auto-mpg.data-original`  

> *“The data concerns city-cycle fuel consumption in miles per gallon, to be predicted in terms of 3 multivalued discrete and 5 continuous attributes.”* — Quinlan (1993)  

---

## 🧭 Project Structure  

### Part I: Exploratory Data Analysis (EDA)  
- Data preprocessing (handling missing values, type conversions, feature inspection)  
- Visualization of categorical and continuous attributes  
- Univariate and multivariate analysis  
- Initial insights about factors influencing `mpg`  

### Part II: Statistical Analysis  
- Reuse of preprocessed data from EDA  
- Hypothesis testing:  
  - Independence between categorical attributes  
  - Normality tests for numeric attributes  
  - Correlation analysis between numeric attributes  
- Application of both **parametric** and **non-parametric** tests  
- Estimation statistics to validate findings from Part I  
- Statistical conclusions and interpretations  

---

## ⚙️ Methodology  

1. **Data Preprocessing**  
   - Remove rows with missing `mpg` values  
   - Handle categorical and numeric features  
   - Clean and transform data  

2. **EDA**  
   - Visual exploration with histograms, scatter plots, and box plots  
   - Summary statistics for all attributes  

3. **Statistical Analysis**  
   - Chi-square tests for independence (categorical)  
   - Shapiro-Wilk / Kolmogorov-Smirnov tests for normality  
   - Pearson/Spearman correlation analysis  
   - t-tests, ANOVA, and non-parametric equivalents  

---

## 📂 Repository Contents  

- `Part1_EDA.ipynb` – Exploratory data analysis notebook  
- `Part2_Statistical_Analysis.ipynb` – Hypothesis testing & statistical insights  
- `auto-mpg.data-original` – Original dataset file  

---

## 📚 References  

- StatLib library, Carnegie Mellon University  
- Quinlan, R. (1993). *Predicting mpg attribute using regression*  
- American Statistical Association Exposition (1983)  

---

## 🚀 How to Run  

1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/city-cycle-fuel-consumption.git
   cd city-cycle-fuel-consumption
