# 🛡️ Network Intrusion Detection System Using Machine Learning

A machine learning-based **Network Intrusion Detection System (NIDS)** designed to classify network traffic as either normal or malicious.

The project uses the **NSL-KDD dataset** and a Random Forest classifier to detect different types of network attacks. A graphical interface was also developed to allow users to interact with the trained model and classify network traffic.

## 🎯 Project Overview

Network intrusion detection systems help identify malicious activity by analyzing network traffic and detecting patterns associated with cyberattacks.

This project applies machine learning techniques to network traffic classification using the NSL-KDD dataset.

The system performs:

1. Data preprocessing
2. Categorical feature encoding
3. Feature scaling
4. Model training
5. Model evaluation
6. Network traffic classification
7. GUI-based prediction

## ✨ Features

* 🛡️ Network intrusion detection
* 🤖 Machine learning classification
* 🌐 NSL-KDD dataset
* 🌲 Random Forest classifier
* 🔢 Categorical feature encoding
* 📏 Feature scaling
* 📊 Model evaluation
* 🖥️ Graphical user interface
* 🔍 Network traffic prediction
* 📈 Classification metrics

## 🗂️ Dataset

The project uses the **NSL-KDD dataset**, an improved version of the original KDD Cup 1999 dataset designed for evaluating intrusion detection systems.

The dataset contains network connection records with features describing characteristics of network traffic.

The classification task is to determine whether network traffic represents:

* **Normal traffic**
* **Attack traffic**

The dataset includes multiple attack categories, including:

* Denial of Service (DoS)
* Probe
* Remote-to-Local (R2L)
* User-to-Root (U2R)

## 🔄 Data Preparation

Before training the machine learning model, the dataset undergoes several preprocessing steps.

### Categorical Encoding

Categorical features are converted into numerical representations using `LabelEncoder`.

This allows machine learning algorithms to process features such as:

* Protocol type
* Service
* Connection flag

### Feature Scaling

Numerical features are standardized using `StandardScaler`.

This places features on comparable scales and improves consistency during model training.

### Train/Test Data

The project uses:

* `KDDTrain+` for training
* `KDDTest+` for testing

Keeping the test data separate allows the trained model to be evaluated on previously unseen network traffic.

## 🤖 Machine Learning Model

### Random Forest

The main classification model is **Random Forest**.

Random Forest combines multiple decision trees and aggregates their predictions to produce the final classification.

Advantages include:

* Good classification performance
* Ability to handle many features
* Robustness against overfitting
* Works well with nonlinear relationships
* Suitable for tabular datasets

## 🧠 Machine Learning Pipeline

```text
NSL-KDD Dataset
       ↓
Data Cleaning
       ↓
Categorical Encoding
       ↓
Feature Scaling
       ↓
Random Forest Training
       ↓
Model Evaluation
       ↓
New Network Traffic
       ↓
Prediction
       ↓
Normal / Attack
```

## 📊 Model Evaluation

The trained model is evaluated using standard classification metrics:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix

These metrics provide a more complete evaluation than accuracy alone, particularly because intrusion detection involves identifying potentially rare attack classes.

## 🖥️ Graphical User Interface

A Python/Tkinter graphical interface was developed to make the intrusion detection system easier to use.

The interface allows users to:

* Enter network traffic information
* Submit traffic for classification
* View the predicted class
* Display classification results

This provides an accessible interface for interacting with the machine learning model without directly running Python commands.

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* Tkinter
* Random Forest
* NSL-KDD

## 📚 Python Libraries

### Pandas

Used for:

* Dataset loading
* Data manipulation
* Data cleaning
* Feature preparation

### NumPy

Used for numerical operations and data processing.

### Scikit-learn

Used for:

* `LabelEncoder`
* `StandardScaler`
* `RandomForestClassifier`
* Model evaluation
* Classification metrics

### Matplotlib & Seaborn

Used for visualizing model performance and evaluation results.

### Tkinter

Used to develop the graphical user interface.

## 🧪 Results

The Random Forest model achieved strong classification performance on the NSL-KDD dataset.

The evaluation results demonstrated that machine learning can effectively identify patterns associated with malicious network traffic.

The GUI successfully connects the trained model with user input and displays the resulting classification.

## 🔍 Example Workflow

A network connection is provided to the system:

```text
Network Traffic
      ↓
Feature Processing
      ↓
Encoding & Scaling
      ↓
Random Forest
      ↓
Prediction
      ↓
┌───────────────┐
│ Normal        │
│      OR       │
│ Attack        │
└───────────────┘
```

## ⚠️ Limitations

* The system is trained specifically on the NSL-KDD dataset.
* Real-world network traffic may differ significantly from the training data.
* Dataset-based performance does not necessarily represent production intrusion detection performance.
* The current system focuses on classification rather than real-time packet capture.
* Some attack categories contain significantly fewer samples than others.

## 🔮 Future Improvements

Potential improvements include:

* 🌐 Real-time packet capture
* 📡 Live network monitoring
* 🤖 Comparison with additional ML models
* 🧠 Deep learning approaches
* 📊 Interactive dashboards
* 🚨 Real-time intrusion alerts
* ☁️ Cloud-based monitoring
* 🔄 Continuous model retraining
* 📈 More detailed attack-type classification

## 🎓 Academic Project

**Domain:** Machine Learning & Cybersecurity
**University:** MSA University

## 👥 Team

* Gamila Hasan
* Team Members
