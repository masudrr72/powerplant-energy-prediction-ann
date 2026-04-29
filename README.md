# Power Plant Energy Prediction using ANN (PyTorch)

## 📌 Project Overview
This project is my first attempt at building an **Artificial Neural Network (ANN) regression model** using PyTorch.  
The goal is to predict **energy output (PE)** from a power plant dataset based on environmental conditions.

---

## 📊 Dataset
- **Features (X):**
  - AT: Ambient Temperature  
  - V: Exhaust Vacuum  
  - AP: Ambient Pressure  
  - RH: Relative Humidity  
- **Target (Y):**
  - PE: Produced Energy  

Dataset size: 9569 samples × 5 columns (4 input features + 1 target).

---

## 🧠 Model Architecture (PyTorch)
```python
self.model = nn.Sequential(
    nn.Linear(x_train.shape[1], 6),
    nn.ReLU(),
    nn.Linear(6, 6),
    nn.ReLU(),
    nn.Linear(6, 1)
)
Input: 4 features

Hidden Layer 1: 6 neurons, ReLU

Hidden Layer 2: 6 neurons, ReLU

Output: 1 neuron (regression output)

⚙️ Training, Validation & Evaluation
Optimizer: Adam

Loss Function: Mean Squared Error (MSE)

Epochs: 60

Best model saved as best_model.pt

Results:
Training MSE: 21.64

Testing MSE: 19.99

R² Score: 0.926

🔑 Key Learnings
How ANN models learn patterns from data

Importance of tracking both training and validation loss

Saving the best model during training

Evaluating regression models using MSE and R² score

Hands-on practice with PyTorch training loop, validation, and evaluation

🚀 How to Run
Clone the repository:

bash
git clone https://github.com/masudaucb1303/powerplant-energy-prediction-ann.git
cd powerplant-energy-prediction-ann
Install dependencies:

bash
pip install -r requirements.txt
Run training script:

bash
python src/train.py
📂 Project Structure
Code
powerplant-energy-prediction-ann/
│
├── data/                # Dataset files
├── notebooks/           # Jupyter notebooks for exploration & training
├── src/                 # Source code (preprocessing, model, training)
├── results/             # Plots, metrics, saved models
├── requirements.txt     # Dependencies
├── README.md            # Project overview
└── LICENSE              # License file
📜 License

This project is licensed under the MIT License.
