# Breast Cancer Classification

This project uses machine learning models to classify breast cancer as benign or malignant using the Breast Cancer Wisconsin (Diagnostic) dataset from the UCI Machine Learning Repository. Two models are implemented: **Logistic Regression** and **Random Forest**.

## Dataset Information
The dataset used in this project is from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic)). It contains 569 instances and 30 numerical features describing the characteristics of cell nuclei.

### Features:
- **ID**: Unique identifier (dropped during modeling).
- **Diagnosis**: Target variable (M for malignant, B for benign).
- 30 numerical features including mean, standard error, and worst-case values for:
  - Radius, Texture, Perimeter, Area, Smoothness, Compactness, Concavity, Symmetry, Fractal dimension.

## Models Implemented
### 1. Logistic Regression
- A simple, linear classifier trained to distinguish between benign and malignant tumors.
- Evaluation Metrics:
  - **Accuracy**: Measures overall performance.
  - **Classification Report**: Precision, recall, and F1-score for both classes.
  - **Confusion Matrix**: Distribution of actual vs. predicted classes.
  - **ROC-AUC Score**: Threshold-independent performance evaluation.

### 2. Random Forest (previous version)
- Ensemble classifier with multiple decision trees to improve robustness.
- Same evaluation metrics as above.

## Code Structure
### Step-by-Step Process:
1. **Load Data**: Load the dataset directly from the UCI repository.
2. **Preprocess Data**:
   - Convert 'Diagnosis' column to binary (M: 1, B: 0).
   - Drop 'ID' column.
3. **Split Data**: Split into training (80%) and testing (20%) sets.
4. **Scale Features**: Use `StandardScaler` to normalize data.
5. **Train Model**: Train Logistic Regression or Random Forest.
6. **Evaluate Model**:
   - Accuracy, Classification Report, Confusion Matrix, and ROC-AUC Score.

## Usage
1. Clone or download the repository.
2. Ensure you have the required Python libraries installed:
   ```bash
   pip install pandas scikit-learn
   ```
3. Run the script:
   
## Acknowledgments
Thanks to the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/index.php) for making this dataset available for educational use.


