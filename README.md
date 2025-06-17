# 🧠 Stroke Prediction Model in R (Interactive Web App & Report)

# [Link Here and wait for 60s to Open Live App](https://mashhood23.shinyapps.io/StrokePredictorApp/)  

*"Data science in healthcare isn't just about prediction — it's about making insights useful, understandable, and actionable. This project brings that philosophy to life."*

This project presents a complete, end-to-end solution for predicting stroke risk using real-world healthcare data. Developed entirely in **R** and powered by **Shiny**, it combines interactive user interfaces, advanced machine learning modeling, and visual communication — all integrated within a single, beautifully styled `RMarkdown` document.

🌐 **Live App**: [Try the Stroke Predictor App](https://mashhood23.shinyapps.io/Build-Deploy-Stroke-Prediction-Model-R/)  
📄 **Full Source File**: `Build-deploy-stroke-prediction-model-R.Rmd`

---

## 🚀 Project Overview

The goal of this project is to empower healthcare professionals and researchers with a simple, interactive tool that estimates the likelihood of a stroke based on patient-specific attributes such as age, glucose levels, hypertension status, and more.

Using modern data science techniques, the app was designed to:
- Preprocess and explore real-world clinical data
- Train and evaluate multiple predictive models
- Visualize key risk factors and performance metrics
- Deploy an interactive prediction interface using **R Shiny**
- Serve as a reproducible and professional report via **R Markdown**

---

## 📦 App Features

✅ **Interactive Web App** (Shiny-based)  
✅ **Responsive Dashboard UI** with `bslib`, custom CSS & watermark  
✅ Real-time **stroke risk prediction** based on 10+ user inputs  
✅ **Machine Learning Models**: Logistic Regression, Random Forest, XGBoost  
✅ Integrated **SMOTE balancing** for handling imbalanced data  
✅ Full **EDA, preprocessing, model tuning, and evaluation**  
✅ **Faceted density plots**, ROC curves, variable importance, and calibration  
✅ Fully reproducible in a single `.Rmd` file

---

## 📊 Data & Preprocessing

The model is trained on a public healthcare dataset (`healthcare-dataset-stroke-data.csv`) with 11 predictors and a binary outcome (`stroke`).

Key preprocessing steps included:
- Handling missing values (PMM imputation via `mice`)
- Conversion and normalization of categorical/numeric fields
- Addressing class imbalance using **SMOTE** from the `themis` package
- Feature engineering using the `recipes` package

---

## 🧠 Model Building

Using the `tidymodels` framework, we trained and evaluated:

- `Logistic Regression` — for interpretability
- `Random Forest` — for robustness and nonlinearity
- `XGBoost` — for gradient-boosted performance

Metrics used: **AUC**, **Accuracy**, **Recall**, **F1**, and **Precision**

Cross-validation was performed using stratified 5-fold CV.

---

## 🎨 Shiny App UI Highlights

- Custom blue-themed UI using `bslib::bs_theme()`
- Brain watermark background (`brain_watermark.png`)
- Predict button with rounded hover effect
- Two-column result boxes (green/red) showing stroke vs. no-stroke probabilities
- Uses `renderUI()` and `observeEvent()` for interactivity

---

## 📁 File Structure

| File | Description |
|------|-------------|
| `Build-deploy-stroke-prediction-model-R.Rmd` | Full report + shiny app + code (main file) |
| `healthcare-dataset-stroke-data.csv` | Dataset used for training the models |
| `brain_watermark.png` | Watermark image for UI background |
| `README.md` | This file |

---

## 🧪 How to Run This Project Locally

1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/stroke-prediction-shiny.git
   cd stroke-prediction-shiny
2. Open Build-deploy-stroke-prediction-model-R.Rmd in RStudio

3. Click "Run Document" or run this in console:

---

## 📤 Deployment
This app is deployed on shinyapps.io, enabling real-time, browser-based interaction without needing R installed.

Visit the live app:
🌐 https://mashhood23.shinyapps.io/Build-Deploy-Stroke-Prediction-Model-R/

---

### 📚 Author
### Mashhood Raza Khan
### 📧 mashhood1223@gmail.com
### 📍 India

---
