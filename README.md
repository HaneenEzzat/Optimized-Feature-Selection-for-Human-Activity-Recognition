**Human Activity Recognition with Feature Selection (GA & PSO)**


This project applies feature selection techniques using Genetic Algorithm (GA) and Particle Swarm Optimization (PSO) to enhance classification performance for Human Activity Recognition (HAR) based on smartphone sensor data. It evaluates models including Random Forest and XGBoost, with and without feature selection.

📦 Dataset
Source: UCI Human Activity Recognition Using Smartphones Dataset

Download Method: via kagglehub

🔧 Installation
pip install pyswarm
pip install deap xgboost scikit-learn

📁 Project Structure
├── data/
│   ├── train.csv
│   └── test.csv
├── src/
│   ├── preprocessing.py
│   ├── rf_model.py
│   ├── xgboost_model.py
│   ├── ga_feature_selection.py
│   └── pso_feature_selection.py
├── visualizations/
│   ├── confusion_matrices.png
│   └── ga_fitness_curve.png
└── main.ipynb

🧠 Models Used
Random Forest

XGBoost

⚙️ Feature Selection Techniques
1. Genetic Algorithm (GA)
Tool: DEAP

Evaluation metric: Cross-validated accuracy

Final model evaluated with selected features on both RF and XGBoost

2. Particle Swarm Optimization (PSO)
Tool: PySwarm

Evaluation metric: Accuracy on a hold-out validation set

Final model evaluated with selected features on both RF and XGBoost

📊 Evaluation Metrics
Accuracy

Classification Report (Precision, Recall, F1-score)

Confusion Matrix

🧪 Experiments & Results
Model Variant	Accuracy
Random Forest (All)	~92.60%
XGBoost (All)	~93.52%
GA + Random Forest	~93.93%
GA + XGBoost	~96.47%
PSO + Random Forest	~92.53%
PSO + XGBoost	~93.31%


📈 Visualizations
Confusion matrices for all models

GA evolution curve (fitness vs generation)

🛠 Usage
Download the dataset (automatically handled by kagglehub).

Run the notebook main.ipynb to:

Preprocess the data

Train baseline models

Apply GA and PSO for feature selection

Retrain and evaluate models on selected features

نسخ
ت
