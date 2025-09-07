# titanic-project

# Titanic Classification – Supervised Learning Project

This project applies a full supervised machine learning flow on the **Titanic Recognition dataset**. The goal is to detrmine if a person survived or not.

## 📑 Project Overview
- **Dataset**: Titanic Recognition dataset (UCI) – 9 features.  
- **Task**: Multi-class classification.  
- **Evaluation Metric**: Macro F1-score.  

## 🔄 Workflow
1. **Data Preparation & EDA**  
- Checked class distribution: plotted the number of survivors vs non-survivors.  
- Visualized age distribution with histograms.  
- Identified missing values in 'Age' and 'Embarked' and filled them with median/mode.  
- Encoded categorical features 'Sex' and 'Embarked' using one-hot encoding.  
- Explored feature relationships with survival using plots (histograms, countplots).  

2. **Experiments**  
   - Compared random forset vs. reggresion.  
   - Trained **Logistic Regression** and **Random Forest** with multiple hyperparameters.  
   - Used **GridSearchCV with Stratified 5-Fold CV** to find the best setup.  

3. **Final Training**  
   - Re-trained the best model (random forest) on the full training set.  

4. **Test Evaluation**  
   - Evaluated on the held-out test set.  
   - Reported **79% Accuracy and 69% Macro F1-score**.  
   - Displayed the first 5 predictions and confusion matrix.  

## ✅ Results
- **Best Model**: random forest
- **Test Accuracy**: 79%  
- **Test Macro F1-score**: 69%  

## 📂 Repository Structure
├── Assignment_supervised_learning_flow.ipynb # Main Jupyter Notebook
├── titanic_train.csv # Training data
├── titanic_test.csv # Test data
├── README.md # Project documentation

## ⚙️ Requirements
- Python 3.8+  
- pandas, numpy  
- scikit-learn  
- matplotlib, seaborn
