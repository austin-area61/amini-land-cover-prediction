# Amini Land Cover Prediction

This repository contains a machine learning model for land cover classification, developed as part of the Amini Data Science Internship technical assignment.

## 📌 Project Overview
The goal of this project is to predict land cover types (`building`, `cropland`, and `wcover` categories) based on geospatial data. A **Random Forest classifier** was trained using various environmental features, and predictions were made for unseen data.

## 📂 Project Structure
```
📦 amini-land-cover-prediction
 ┣ 📜 amini_land_cover_model.ipynb # Jupyter Notebook with the entire workflow
 ┣ 📜 submission.csv  # Final predictions for submission
 ┣ 📜 Technical Report 
 ┗ 📜 README.md 
```

## 🚀 How to Run the Project

### **1️⃣ Install Dependencies**
Ensure you have Python installed, then install the required libraries:
```sh
pip install pandas numpy scikit-learn matplotlib
```

### **2️⃣ Open & Run Jupyter Notebook**
Start Jupyter Notebook and open `land_cover_model.ipynb`:
```sh
jupyter notebook
```
Run all cells to **train the model** and **generate predictions**.

### **3️⃣ Final Predictions**
The model saves the predictions as `submission.csv`. This file is structured as:
```
subid, building, cropland, wcover_<30%, wcover_>30%, wcover_>60%
1548905, 0.01, 0.78, 0.45, 0.32, 0.92
1548829, 0.03, 0.65, 0.58, 0.21, 0.87
```
These values represent the **probability of each class occurring** at a given location.

## 📊 Model Performance
The trained **Random Forest Classifier** achieved the following accuracy on the validation set:
* **Building:** **99.94%**
* **Cropland:** **78.53%**
* **Wcover Categories:** **100%**

## 🛠 Possible Improvements
* **Feature Engineering:** Include more geospatial features.
* **Hyperparameter Tuning:** Optimize `n_estimators`, `max_depth`, etc.
* **Class Imbalance Handling:** Use SMOTE or weighted loss functions.

## 📜 License
This project is for educational and internship application purposes.

## 📝 Author
Developed by **Austin Onyango**
* 🔗 GitHub: [My GitHub Profile](https://github.com/austin-area61)
* 📧 Email: austinonyango.area61@gmail.com
