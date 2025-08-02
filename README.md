Anomaly Detection in Networks 

📌 Overview
This repository contains a machine learning project focused on detecting anomalies in network traffic data.
It follows a complete data science pipeline — from data preprocessing 🧹 and statistical analysis 📊 to feature selection 🎯 and training ML models 🤖 — to identify potential network attacks and unusual behavior.

The project uses the CICIDS2017 dataset 🛡️, which contains both normal and malicious network traffic, to simulate real-world cybersecurity detection tasks.

📂 Project Structure
| 📁 Notebook                                                   | 📝 Description                                                                            |
| ------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| `01_preprocessing.ipynb`                                      | Loads raw CICIDS2017 CSV files and cleans, merges, and prepares the dataset for analysis. |
| `02_statistics.ipynb`                                         | Generates basic statistics and visualizations for understanding the dataset.              |
| `03_attack_filter.ipynb`                                      | Filters and extracts attack-specific traffic from the dataset.                            |
| `04_1_feature_selection_for_attack_files.ipynb`               | Performs feature selection specifically for attack data.                                  |
| `04_2_feature_selection_for_all_data.ipynb`                   | Performs feature selection for the complete dataset.                                      |
| `05_1_machine_learning_implementation_for_attack_files.ipynb` | Trains ML models on attack-only data.                                                     |
| `05_2_machine_learning_implementation_with_18_feature.ipynb`  | ML implementation using 18 selected features.                                             |
| `05_3_machine_learning_implementation_with_7_feature.ipynb`   | ML implementation using 7 selected features.                                              |
| `05_3_ml_f_measure_comparison.ipynb`                          | Compares F-measure performance across different feature sets.                             |
| `05_4_machine_learning_implementation_final.ipynb`            | Final refined ML model with best parameters.                                              |


📊 Dataset
1. Name: CICIDS2017 (Canadian Institute for Cybersecurity)
2. Description: Contains both benign and malicious network traffic data 💻, including attacks such as DDoS, Brute Force, Botnet, and more.
3. Requirements:
    📥 Download dataset from: CICIDS2017 Official Website
    📂 Place raw CSV files in a folder named CSVs inside the project directory.
    📄 Ensure derived files (all_data.csv, attacks/ folder) are in the correct locations for each notebook.

⚙️ Installation
# Clone the repository
git clone https://github.com/your-username/anomaly-detection-in-networks-ml.git
cd anomaly-detection-in-networks-ml

# Install dependencies
pip install -r requirements.txt

▶️ Usage
🆕 Beginner-Friendly Steps
1. 📥 Download the CICIDS2017 dataset and place it in the CSVs folder.
2. 📑 Open notebooks in order:
       01_preprocessing.ipynb → Data cleaning
       02_statistics.ipynb → Data exploration
       03_attack_filter.ipynb → Extract attacks
       04_feature_selection → Feature selection
       05_Machine Learning Implementation → Model training and evaluation
3. ▶️ Run all cells step-by-step in Jupyter Notebook or JupyterLab.
     ⚡ For Experienced Users
         🔄 You can start from feature selection (04_*) if preprocessed data is available.
         🛠 Modify ML model parameters inside the 05_* notebooks for experimentation.
         🔌 The pipeline supports easy integration of new algorithms.

📈 Results
Models Used: Decision Tree 🌳, Random Forest 🌲, Gradient Boosting 🚀, etc.

Metrics: Accuracy 🎯, Precision 📏, Recall 📢, F1-score 🏆.

📊 Performance comparisons between different feature sets are documented in 05_3_ml_f_measure_comparison.ipynb.

📜 License
This project is licensed under the MIT License – see the LICENSE file for details.
