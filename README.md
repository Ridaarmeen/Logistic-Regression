🧠 Logistic Regression Classifier - Breast Cancer Detection
Implementation of Logistic Regression model to classify tumors as malignant or benign using the Breast Cancer Wisconsin dataset.

📌 Objective
- Load and preprocess medical data
- Train a Logistic Regression model
- Evaluate the model using key classification metrics
- Visualize the sigmoid and ROC curve
- Experiment with threshold tuning for classification

🛠️ Libraries Used
- pandas
- numpy
- scikit-learn
- matplotlib
  
🚀 Steps Overview
1. Load and Prepare Data
- Read `data.csv` using `pandas`
- Drop unnecessary columns like `id` and `Unnamed: 32`
- Map the `diagnosis` column (`M` → 1, `B` → 0)
- Split into features `X` and target `y`

2. Train/Test Split & Standardization
- Use `train_test_split` for an 80/20 split
- Standardize features using `StandardScaler`

3. Train the Logistic Regression Model
- Fit a `LogisticRegression` model using training data

4. Model Evaluation
- Generate predictions and probabilities
- Compute:
  - Confusion Matrix
  - Precision
  - Recall
  - ROC-AUC Score

5. Visualization
- Plot ROC Curve to analyze trade-off between TPR and FPR
- Visualize the sigmoid function
- Tune decision threshold and observe effects on metrics
