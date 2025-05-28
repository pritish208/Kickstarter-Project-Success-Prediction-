# Kickstarter-Project-Success-Prediction-

## Data Import & Basic Exploration
Dataset: ks-projects-201801.csv from Kickstarter.

Library imports: pandas, matplotlib, seaborn, scikit-learn, xgboost, tensorflow.

Initial steps:

data.head(), data.info(), data.isnull().sum() for overview.

Dropped unneeded columns: 'ID' and 'name'.

## 2. Data Cleaning & Preprocessing
Missing Values:

Column 'usd pledged' had missing values filled with the mean.

Target Variable Filtering:

Kept only rows with state == "successful" or "failed" — binary classification.

Feature Engineering:

Likely included dropping/reformatting of date/time or textual features (based on common practice with this dataset, but not explicitly visible yet).

Scaling:

Used StandardScaler for feature scaling.

## 3. Train-Test Split
Applied train_test_split to separate training and testing datasets.

## 4. Models Used
Logistic Regression

Random Forest

XGBoost Classifier

Each model was:

Trained on the training dataset.

Evaluated using accuracy_score.

## 5. Evaluation Metrics
The notebook used accuracy_score for evaluation — likely compared model performances.

## 6. Additional Techniques
Class Weighting: Used compute_class_weight to handle class imbalance.

Deep Learning: TensorFlow was imported, suggesting a possible attempt at using neural networks, though no code for it is visible in the extracted portion yet.
