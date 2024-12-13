# Car Evaluation Machine Learning Project

## Project Overview

This project focuses on car evaluation using machine learning techniques to classify cars based on various attributes. We employed multiple classification algorithms to predict car ratings using features like buying cost, maintenance, number of doors, number of persons, luggage boot size, and safety.

## Dataset

The dataset is sourced from the UCI Machine Learning Repository (Car Evaluation Dataset). It contains categorical features describing various aspects of cars and their corresponding evaluation ratings.

### Features
- Buying price
- Maintenance cost
- Number of doors
- Number of persons
- Luggage boot size
- Safety rating

### Target Classes
- Unacceptable (unacc)
- Acceptable (acc)
- Good
- Very Good (vgood)

## Methodology

We used three different machine learning algorithms to classify car evaluations:

1. **K-Nearest Neighbors (KNN)**
   - Hyperparameters: 3 neighbors
   - Preprocessing: Label encoding for categorical features
   - Evaluation Metrics: Accuracy, Confusion Matrix, Classification Report

2. **Support Vector Machine (SVM)**
   - Kernel: Linear
   - Cross-validation: 10-fold
   - Evaluation: Mean accuracy and standard deviation

3. **Decision Tree**
   - Random state: 42
   - Evaluated using accuracy, confusion matrix, and classification report

## Results

### KNN Classifier
- **Overall Accuracy**: 86.90%
- **Feature Importance** (from most to least important):
  1. Persons: 68.98%
  2. Luggage Boot: 68.98%
  3. Buying Price: 58.96%
  4. Doors: 57.61%
  5. Safety: 55.30%
  6. Maintenance: 45.47%
- **Mean Absolute Error**: 0.25

### SVM Classifier
- **Accuracy**: 0.72 (with 0.02 standard deviation)

### Decision Tree Classifier
- **Accuracy**: 0.97
- Performed exceptionally well, with near-perfect precision and recall for most classes

## Key Insights

1. The number of persons and luggage boot size are the most influential features in determining a car's rating.
2. Maintenance cost seems to have the least impact on car evaluation.
3. The Decision Tree classifier significantly outperformed KNN and SVM, suggesting that the car evaluation problem might have clear, interpretable decision boundaries.

## Visualizations

The project includes two main visualizations:
1. A confusion matrix heatmap showing prediction accuracies
2. A decision tree visualization illustrating the classification logic

## Requirements
- Python 3.x
- scikit-learn
- pandas
- numpy
- seaborn
- matplotlib
- ucimlrepo

## How to Run
1. Clone the repository
2. Install the required dependencies
3. Run the Jupyter notebook or Python script

## Future Work
- Experiment with hyperparameter tuning
- Try ensemble methods like Random Forest
- Collect more diverse data to improve model generalization

## Contributors
[Eng. Yara Daraghmeh ]

## License
[ MIT License]
