# Predictive Maintenance of Industrial Machinery Using Machine Learning

This repository contains the implementation, results, and documentation for the predictive maintenance project, which uses machine learning models to predict the Remaining Useful Life (RUL) of machinery components. The project utilizes NASA's C-MAPSS dataset and evaluates both dataset-specific and unified models for RUL prediction.

---

## **Introduction**
Industrial machinery plays a critical role in sectors such as manufacturing, transportation, and aerospace. Unexpected component failures lead to:
- **Unplanned Downtime**: Reduced productivity and financial losses.
- **Safety Risks**: Potential hazards to workers and operations.

### **Objective**
This project aims to:
- Develop machine learning models tailored for predictive maintenance.
- Accurately predict RUL for machinery components under various operational scenarios.
- Compare the performance of dataset-specific models against a unified model.

### **State of the Art**
Current methods for RUL prediction:
- **Dataset-Specific Models**: Deliver high accuracy for individual datasets but lack generalization.
- **Unified Models**: Generalize predictions across datasets but face challenges with inconsistent failure patterns.

---

## **Aim**
1. **Dataset-Specific Models**:
   - Develop machine learning models (Random Forest, XGBoost, Blended Ensemble) tailored for individual datasets (FD001-FD004).
   - Perform a comparative analysis to determine the most effective model for each dataset.
2. **Unified Model**:
   - Develop a single model capable of generalizing predictions across all datasets.
   - Evaluate its performance against individual models to identify trade-offs.

---

## **Datasets**
- **Source**: [NASA C-MAPSS Dataset](https://data.nasa.gov/Aerospace/CMAPSS-Jet-Engine-Simulated-Data/ff5v-kuh6).
- **Description**:
  - 4 subsets: FD001, FD002, FD003, and FD004, representing different operating conditions and fault modes.
  - Features: 26 sensor measurements and 3 operational settings.
  - Target: Remaining Useful Life (RUL).
  - Total rows (train + test): 265,256.
 ---
## **How to Replicate the Project**

### **1. Prerequisites**
- Download the [NASA C-MAPSS Dataset](https://data.nasa.gov/Aerospace/CMAPSS-Jet-Engine-Simulated-Data/ff5v-kuh6).
- Ensure you have a Google account to use Google Colab.

### **2. File Setup**
- Place the downloaded dataset in your Google Drive for easy access in Colab.
- Clone this repository and upload the Google Colab files to your drive or workspace.

### **3. Running the Project**
For each dataset (FD001, FD002, FD003, FD004), and the unified model:
1. **Open the Colab Notebook**:
   - Navigate to `notebooks/FD001_Colab.ipynb` for FD001, and similar files for other datasets and the unified model.
2. **Follow the Steps**:
   - Each notebook contains:
     - Feature dropping.
     - Data preprocessing (e.g., correlation analysis and rolling statistics).
     - Model training for Random Forest, XGBoost, and Blended Ensemble.
     - Model evaluation (plots, metrics, and predictions).
3. **Unified Model**:
   - Open `notebooks/Applied_AI_Project_UnifiedModel.ipynb` to run the unified model across all datasets.
