# ✈️ Flight Delay Prediction Using Artificial Neural Network

## 📌 Project Overview

This project predicts whether a commercial flight will be delayed using an Artificial Neural Network (ANN).

The model uses flight-related information such as airline, origin airport, destination airport, scheduled departure time, day of the week, flight number, and flight duration.

The project demonstrates how Artificial Neural Networks can handle a large dataset containing both numerical and high-cardinality categorical features.

## 🎯 Objective

The main objective is to develop a machine learning system that predicts:

* `0` → Flight Not Delayed
* `1` → Flight Delayed

## 📊 Dataset

The dataset contains approximately **539,383 flight records** and the following columns:

| Feature       | Description              |
| ------------- | ------------------------ |
| `id`          | Unique record identifier |
| `Airline`     | Airline code             |
| `Flight`      | Flight number            |
| `AirportFrom` | Origin airport           |
| `AirportTo`   | Destination airport      |
| `DayOfWeek`   | Day of the week          |
| `Time`        | Scheduled departure time |
| `Length`      | Flight duration          |
| `Delay`       | Target variable          |

The `id` column is excluded from model training because it is only an identifier.

## 🧠 Machine Learning Approach

The project follows this pipeline:

```text
Flight Dataset
      ↓
Data Cleaning
      ↓
Exploratory Data Analysis
      ↓
Feature Selection
      ↓
One-Hot Encoding
      ↓
Feature Scaling
      ↓
Train / Validation / Test Split
      ↓
Artificial Neural Network
      ↓
Prediction
      ↓
Performance Evaluation
```

## 🔧 Technologies Used

* Python
* Google Colab
* Pandas
* NumPy
* Scikit-learn
* TensorFlow
* Keras
* Matplotlib
* Seaborn
* Joblib

## 🏗️ ANN Architecture

The neural network consists of:

```text
Input Layer
     ↓
Dense Layer - 128 neurons
     ↓
Batch Normalization
     ↓
Dropout
     ↓
Dense Layer - 64 neurons
     ↓
Batch Normalization
     ↓
Dropout
     ↓
Dense Layer - 32 neurons
     ↓
Dropout
     ↓
Output Layer - 1 neuron
     ↓
Sigmoid Activation
```

## 🔤 Categorical Feature Processing

The following categorical features are transformed using One-Hot Encoding:

* Airline
* AirportFrom
* AirportTo

Numerical features are standardized using `StandardScaler`.

## 📈 Model Evaluation

The model is evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC
* Confusion Matrix
* ROC Curve
* Precision-Recall Curve

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/flight-delay-prediction-ann.git
```

### 2. Open the notebook

Open:

```text
Flight_Delay_Prediction_ANN.ipynb
```

using Google Colab or Jupyter Notebook.

### 3. Upload the dataset

Upload your flight dataset when prompted by the notebook.

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

### 5. Run the notebook

Execute the notebook cells sequentially.

## 📁 Project Structure

```text
flight-delay-prediction-ann/
│
├── Flight_Delay_Prediction_ANN.ipynb
├── README.md
├── requirements.txt
│
├── data/
│   └── README.md
│
├── models/
│   └── README.md
│
└── images/
    ├── confusion_matrix.png
    ├── roc_curve.png
    └── training_accuracy.png
```

## 🔮 Future Improvements

Possible improvements include:

* Flight cancellation prediction
* Real-time flight delay prediction
* Weather data integration
* Airport congestion information
* Holiday and seasonal features
* Live airline data integration
* Hyperparameter optimization
* Comparison with Random Forest, XGBoost and Logistic Regression
* Web application using Streamlit or Flask
* Cloud deployment

## 👨‍💻 Author

**Sayan Adhikary**

B.Tech Computer Science & Engineering

## ⭐ Project Highlights

* Large-scale flight dataset
* High-cardinality categorical feature processing
* One-Hot Encoding
* Artificial Neural Network
* TensorFlow/Keras
* Binary classification
* Model evaluation using multiple metrics
* Prediction probability and optimized classification threshold
