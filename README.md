# 🚨 Anomaly Detection in Network Traffic
This project demonstrates **Anomaly Detection** on the **KDD Cup 1999** dataset using two approaches:
- **Isolation Forest**
- **Autoencoder Neural Network**
The aim is to identify suspicious or malicious network traffic based on learned normal patterns.

## 📁 Dataset
- Dataset Link - https://www.kaggle.com/datasets/galaxyh/kdd-cup-1999-data
- Source: KDD Cup 1999 Dataset (10% subset)
- Format: CSV & zip with a mix of **categorical** and **numerical** features.

(must be download and unzip the dataset before running the code)

## 🔧 Features Used
- Preprocessing: 
  - One-hot encoding for categorical columns
  - StandardScaler for numerical features
- Train-test split: 80/20

## 📊 Models Used

### ✅ 1. Isolation Forest
- Unsupervised anomaly detection algorithm
- Detects anomalies based on how easy data points are isolated in trees

### ✅ 2. Autoencoder (Neural Network)
- Trained to reconstruct normal patterns
- High reconstruction error indicates anomalies

## 📈 Evaluation

- **Isolation Forest**: Anomaly scores are based on tree structures (lower = more anomalous)
- **Autoencoder**: Mean Squared Reconstruction Error is calculated
- Both methods use a **threshold** to label test samples as anomalous.

## 📌 Outputs

- Distribution plots of:
  - Isolation Forest Anomaly Scores
  - Autoencoder Reconstruction Errors
- Number of anomalies detected by each model
- Top 5 anomalies from each model

## 🧪 Libraries Used

pandas
numpy
scikit-learn
matplotlib
seaborn
tensorflow
Install them using:  pip install -r requirementts.txt
## 🚀 How to Run
Clone the repository: git clone https://github.com/your-username/anomaly-detection-network.git
cd anomaly-detection-network
Place the dataset kddcup.data_10_percent_corrected inside a folder named network_data.

## Run the notebook -- jupyter notebook Anomaly_Detection_in_Network_Traffic_Project.ipynb

