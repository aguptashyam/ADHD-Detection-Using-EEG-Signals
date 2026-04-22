# ADHD Detection Using EEG Signals (Machine Learning)

This project focuses on **objective detection of Attention Deficit Hyperactivity Disorder (ADHD)** using **EEG signal processing and machine learning techniques**. The aim is to support traditional clinical diagnosis by reducing subjectivity through data-driven analysis.

---

## 📌 Project Overview

- Binary classification: ADHD vs Healthy
- 19-channel EEG signals recorded during a visual attention task
- Extensive handcrafted EEG feature extraction
- Evaluation using classical machine learning models

---

## 📂 Project Files

- **ADHD_DETECTION_ANUBHAV_GUPTA.ipynb** – Machine learning pipeline
- **Feature_extraction_ANUBHAV_GUPTA.ipynb** – EEG feature extraction
- **eeg_preprocessed_data.csv** – Cleaned EEG signals
- **preprocessed_eeg_data.csv** – Final feature dataset
- **adhdata_original_dataset.csv** – Original dataset
- **Report_ADHD_Detection_using_EEG_Signals.pdf** – Project report
- **Poster_ADHD_Detection.png** – Project poster

---

## 📊 Dataset

The dataset used in this project is publicly available on Kaggle:

**EEG Dataset for ADHD Detection**  
Source: Kaggle  
Link: [https://www.kaggle.com/datasets/danizo/eeg-dataset-for-adhd/data](https://www.kaggle.com/datasets/danizo/eeg-dataset-for-adhd/data)

- 121 subjects (61 ADHD, 60 Healthy)
- 19 EEG channels
- Sampling frequency: 128 Hz
- Task-based EEG recordings

---

## ⚙️ Methodology

### 1️⃣ EEG Preprocessing
- Signal normalization
- Segmentation into 1-second windows
- Basic artifact and noise handling

### 2️⃣ Feature Extraction
Handcrafted features were extracted from each EEG channel to capture morphological, temporal, spectral, and inter-channel characteristics.

- **Morphological Features:** Amplitude, Range, RMS
- **Time-Domain Features:** Mean, Variance, Skewness, Kurtosis, Hjorth parameters
- **Frequency-Domain Features:** Delta, Theta, Alpha, Beta band power, spectral entropy
- **Connectivity Features:** Correlation, Coherence, Phase Locking Value (PLV), Mutual Information

**Total combined features:** 760

### 3️⃣ Machine Learning Models
- Support Vector Machine (SVM)
- Random Forest
- Gaussian Process Classifier (GPC)
- Multilayer Perceptron (MLP)

Hyperparameter tuning and cross-validation were used to ensure robust performance.

---

## 📈 Results

### Model Performance
- SVM: **98.8%** accuracy
- Random Forest: **97.8%** accuracy
- Gaussian Process Classifier: **97.6%** accuracy
- Multilayer Perceptron: **97.92%** accuracy

Results indicate that classical machine learning models combined with well-engineered EEG features can achieve high ADHD classification accuracy.

---

## 🚀 How to Run

1. Clone the repository
2. Install required Python dependencies:
   ```
   pip install numpy pandas scikit-learn matplotlib seaborn jupyter
   ```
3. Open Jupyter notebooks:
   - `Feature_extraction_ANUBHAV_GUPTA.ipynb`
   - `ADHD_DETECTION_ANUBHAV_GUPTA.ipynb`
4. Run preprocessing, feature extraction, and model training cells sequentially

---

## ⚠️ Disclaimer

This project is intended strictly for **educational and research purposes**. It is **not a medical diagnostic tool** and should not be used for clinical decision-making. Always consult qualified medical professionals for diagnosis.

---

## 👤 Author

**Anubhav Gupta**

- EEG feature extraction
- Data preprocessing
- Machine learning model development and evaluation

© 2024 ADHD Detection Using EEG Signals. Academic Research Project.
