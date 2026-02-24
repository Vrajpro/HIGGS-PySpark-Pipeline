# HIGGS Boson Classification: A Distributed PySpark Pipeline

**Author:** Vraj Dipakkumar Parekh (Student ID: 16485659)
**Course:** MSc in Data Science (Coventry University)
**Module:** 7006SCN - Machine Learning and Big Data - 2526JANMAR

## 📌 Project Overview
This repository contains the code and resources for a distributed machine learning pipeline built using Apache Spark (PySpark). The objective is to accurately classify high-energy physics collisions to distinguish the Higgs boson signal from background noise. 

The project addresses the Big Data challenge of processing the 7.48GB UCI HIGGS dataset (11 million rows) on standard hardware by implementing strict memory management, distributed data processing, and a 5% stratified sampling strategy.

## 🚀 Key Technologies Used
* **Data Processing:** Apache Spark (PySpark), MLlib
* **Machine Learning Models:** Logistic Regression, Linear SVM, Random Forest, Gradient Boosted Trees (GBT)
* **Environment:** Google Colab
* **Visualization:** Tableau Public

## 📁 Repository Structure
* `/notebooks/`: Contains the modular PySpark pipeline split into four sequential stages (`1_data_ingestion.ipynb`, `2_feature_engineering.ipynb`, `3_model_training.ipynb`, `4_evaluation.ipynb`) to simulate enterprise-level checkpoints.
* `/scripts/`: Contains `run_pipeline.py`, the unified Python script designed for automated, top-to-bottom pipeline execution.
* `/tableau/`: Contains the exported Tableau workbook (`.twbx`) containing the interactive visualisations.
* `/data/`: Directory architected for the raw HIGGS dataset (Dataset excluded from repository submission due to 7.48GB GitHub/University portal size limitations).
* `Final_Report.pdf`: The final academic report detailing the methodology, results, and Big Data scaling strategies.

## ⚙️ How to Run the Code
**Option 1: Modular Execution (Google Colab)**
1. Upload the four sequential notebooks from the `/notebooks/` folder to Google Colab.
2. Download the original HIGGS dataset from the UCI Machine Learning Repository and mount it to your Google Drive environment.
3. Run the notebooks sequentially (1 through 4). The pipeline handles data ingestion, feature engineering, model training, and evaluation.

**Option 2: Automated Execution (Terminal/Local Spark)**
1. Ensure Apache Spark is installed and configured on your local machine or cluster.
2. Run the command `python scripts/run_pipeline.py` to execute the entire pipeline end-to-end automatically.

## 📊 Tableau Dashboard
The visual analysis of the model's performance and scalability can be viewed interactively here:
https://public.tableau.com/views/Vraj_Parekh_7006SCN_HIGGS_Dashboard/DataQualityPipelineMonitoring?:language=enUS&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

## 🔗 Dataset Source
Baldi, P., Sadowski, P., & Whiteson, D. (2014). HIGGS Dataset. UCI Machine Learning Repository. 
https://doi.org/10.24432/C5V312