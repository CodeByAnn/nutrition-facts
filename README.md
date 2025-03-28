# nutrition-facts
Data Wrangling and Exploration: Nutrition Facts
## Open Food Facts: Cleaning and Exploring Global Nutrition Data

### Summary

This project explores and cleans a large dataset from **Open Food Facts**, which includes nutritional and product information for over 385.000 food items. The main focus is on fixing missing or incorrect values, organizing the data for analysis, and creating clear visual summaries to understand patterns across products and countries.

---

### Dataset Overview

- **385.384 samples** and **99 columns**
- Includes nutritional info (e.g. fat, sugar, protein), product names, countries, and units
- Many missing or inconsistent values (e.g. missing vitamins, extreme outliers)
- Data types grouped by structure: per 100g, per portion, unit type, and other metadata

---

### Key Steps

### 1. **Data Cleaning**

- Removed duplicate rows and columns with too many missing values
- Filled in missing unit labels using the most frequent values (e.g. “g”, “mg”)
- Labeled missing ingredients and product names to keep track of gaps
- Replaced obviously incorrect values (e.g. 500g of fat per 100g product) with NaN
- Standardized energy values (kJ to kcal) and fixed inconsistencies

### 2. **Exploratory Analysis**

- Analyzed categorical variables like **country** and **unit type** using bar plots
- Created histograms and descriptive stats for numeric values (e.g. sugar, fat, energy)
- Found right-skewed distributions and extreme outliers in multiple features
- Used matrix and heatmap visualizations to detect and explain missing data patterns

### 3. **Special Checks**

- Flagged and cleaned rows where macronutrient totals exceeded 100g per 100g product
- Verified energy conversions between kilojoules and kilocalories
- Removed data rows that didn't match expected conversion values

---

### Observations

- Over 22 columns were removed due to more than 95% missing values
- US and Switzerland are the top countries in the dataset
- Unit usage is dominated by **grams** and **milliliters**
- Many vitamins and minerals are frequently missing, especially in older records or less regulated products
- Cleaning improved data accuracy but increased the number of NaN values, which is expected

---

### Conclusion

This project shows how essential **data cleaning** is when working with real-world datasets. By fixing structure, filling gaps, and checking for invalid values, the dataset becomes ready for meaningful analysis and modeling. Clear visualizations and organized summaries help define trends in food content, nutrition labeling and data quality across countries.
