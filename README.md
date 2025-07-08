## Overview
This project uses machine-learning techniques to predict loan approval status (`Loan_Status`) based on applicant information (e.g. credit history, income, education). It demonstrates:
- Data loading and exploratory analysis
- Handling missing values and preprocessing (numerical & categorical)
- Model training with multiple classifiers
- Hyperparameter tuning via grid search
- Evaluation using accuracy, ROC-AUC, classification reports, and ROC curves

## Dataset
- **Source**: An Excel file (`loan_prediction.xlsx`) containing loan application records.
- **Target**: `Loan_Status` (`Y` = approved, `N` = rejected)
- **Features**: 
  - Numerical: ApplicantIncome, CoapplicantIncome, LoanAmount, Loan_Amount_Term, Credit_History
  - Categorical: Gender, Married, Dependents, Education, Self_Employed, Property_Area

## Requirements
pandas
numpy
scikit-learn
matplotlib
openpyxl

## Usage
1. Place your loan dataset Excel file in the project root (or update the path in the notebook).
2. Open and run the notebook:
   ```jupyter notebook loan_prediction.ipynb```
3. Walk through each cell to:

   * Load and inspect data
   * Define preprocessing pipelines
   * Train and tune models (RandomForest, AdaBoost, GradientBoosting)
   * View evaluation metrics and plots

## Results

* **Best Model**: You can see which classifier yielded the highest ROC-AUC and accuracy.
* **Metrics**: Detailed classification reports and ROC curves are produced for comparison.

## Contributing

Feel free to open issues or submit pull requests if you’d like to:

* Add new models
* Try alternative feature engineering
* Improve hyperparameter ranges
* Integrate cross-validation more deeply

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
