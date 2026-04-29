# From Data to Prediction: ANN Regression Model

## 📌 Project Overview
This project demonstrates my first Artificial Neural Network (ANN) regression model to predict **energy output (PE)** from a power plant dataset.  
The dataset contains environmental features such as temperature, pressure, vacuum, and humidity, which are used to estimate the produced energy.

---

## 📊 Dataset
- **Source:** Power Plant Dataset (5 × 9569 samples)  
- **Input Features (X):**
  - AT: Ambient Temperature  
  - V: Exhaust Vacuum  
  - AP: Ambient Pressure  
  - RH: Relative Humidity  
- **Target Feature (Y):**
  - PE: Produced Energy  

---

## 🧠 Model Architecture
- Framework: TensorFlow / Keras  
- Layers:
  - Dense (64 units, ReLU)  
  - Dense (32 units, ReLU)  
  - Dense (1 unit, Linear for regression)  
- Optimizer: Adam  
- Loss Function: Mean Squared Error (MSE)  

---

## 📈 Model Performance
- **Training MSE:** 21.64  
- **Testing MSE:** 19.99  
- **R² Score:** 0.926  

---

## 🔑 Key Learnings
- How ANN models learn patterns from data  
- Importance of tracking both training and testing loss  
- Evaluating regression models using MSE and R² score  
- Building and optimizing models using deep learning frameworks  

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/masudaucb1303/powerplant-energy-prediction-ann.git
   cd powerplant-energy-prediction-ann
## Install dependencies:
   pip install -r requirements.txt
## Run training script:
   python src/train.py
