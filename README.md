# Power Plant Energy Prediction using ANN (PyTorch)

## Project Overview
This project is my first attempt at building an Artificial Neural Network (ANN) regression model using PyTorch.  
The goal is to predict energy output (PE) from a power plant dataset based on environmental conditions.

## Dataset
Features (X):
- AT: Ambient Temperature
- V: Exhaust Vacuum
- AP: Ambient Pressure
- RH: Relative Humidity

Target (Y):
- PE: Produced Energy

Dataset size: 9569 samples × 5 columns (4 input features + 1 target).

## Model Architecture (PyTorch)
Input: 4 features  
Hidden Layer 1: 6 neurons, ReLU  
Hidden Layer 2: 6 neurons, ReLU  
Output: 1 neuron (regression output)

## Training, Validation & Evaluation
Optimizer: Adam  
Loss Function: Mean Squared Error (MSE)  
Epochs: 60  
Best model saved as best_model.pt  

Results:  
- Training MSE: 21.64  
- Testing MSE: 19.99  
- R² Score: 0.926  

## Key Learnings
- How ANN models learn patterns from data  
- Importance of tracking both training and validation loss  
- Saving the best model during training  
- Evaluating regression models using MSE and R² score  
- Hands-on practice with PyTorch training loop, validation, and evaluation  

## How to Run
1. Clone the repository:
   git clone https://github.com/masudrr72/powerplant-energy-prediction-ann.git
   cd powerplant-energy-prediction-ann

2. Install dependencies:
   pip install -r requirements.txt

3. Run training script:
   python src/train.py

## Project Structure
powerplant-energy-prediction-ann/
│
├── data/                
├── notebooks/           
├── src/                 
├── results/             
├── requirements.txt     
├── README.md            
└── LICENSE              

## License
This project is licensed under the MIT License.
