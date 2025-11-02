# 🚗 Feature Engineering on Used Car Dataset  
**Colab Notebook:** [Open Here](https://colab.research.google.com/drive/1yEcsyTAIxL_aJDp1ix0L6hJfG0ECbIcw?usp=sharing)  

---

## 📘 Overview  
This project demonstrates **feature engineering** techniques on a **used car dataset**.  
The goal is to clean messy data, handle missing values, and create new, meaningful features that make the dataset more informative for future analysis or modeling.

---

## 🧾 Dataset  
The dataset contains details about used cars such as:  
`Make, Model, Year, Price, Kilometer, Engine, Max Power, Fuel Type, Transmission, Owner, Seller Type, Drivetrain, Length, Width, Height, Fuel Tank Capacity.`  

---

## ⚙️ Feature Engineering Steps  
- **Data Cleaning:** Removed units like “cc” / “bhp”, extracted numeric values, filled missing data using median/mode.  
- **Encoding:** Converted categorical columns using label encoding.  
- **New Features:**  
  - `Car_Age = 2025 - Year`  
  - `Car_Volume = Length × Width × Height`  
  - `Power_per_Engine = Max Power / Engine`  
  - `Performance_Index = Max Power / Car_Volume`  
  - `Price_per_KM = Price / (Kilometer + 1)`  
- **Transformations:** Log scaling of skewed features (`Engine`, `Max Power`, `Max Torque`).  
- **Scaling:** Standardized all numeric columns using Z-score normalization.  

---

## 🔍 Observations  
- Missing and inconsistent data handled successfully.  
- New features like `Car_Age` and `Performance_Index` add valuable insights.  
- Dataset is now structured, balanced, and ready for further analysis or visualization.  

---

## 🏁 Conclusion  
The notebook showcases how **feature engineering** transforms raw car data into a **clean and meaningful** dataset.  
It improves interpretability and prepares the data for future machine learning or analytical tasks.  

---

**Author:** Atharva Kadam
**Institute:** MIT Academy of Engineering, Pune  
