# PenguinDatasetProject
project for ECPI homework

# README

## Project Overview

This project evaluates the performance of three machine learning models (Regression, Clustering, and Classification) applied to a dataset of penguins. The goal is to analyze their effectiveness in predicting penguin body mass, clustering species, and classifying species based on physical features. Additionally, scenarios were developed to simulate real-world changes, such as environmental shifts, population imbalance, and feature variation, and their impact on model predictions was analyzed.

## Results Summary

### Model Results
- **Regression Model**:
  - Predicts continuous values for body mass.
  - Achieved a Mean Absolute Error (MAE) of 210.67 after training.

- **Clustering Model (K-Means)**:
  - Groups penguins into clusters based on physical features.
  - Achieved a Silhouette Score of 0.75.

- **Classification Model**:
  - Categorizes penguins into species.
  - Achieved an accuracy of 92% with the neural network.

### Scenario Insights
1. **Environmental Shift**:
   - Reducing body mass in the data showed a consistent decrease in predictions, reflecting potential climate change impacts.
2. **Demographic Changes**:
   - Oversampling "Adelie" species caused a noticeable skew in classification predictions, highlighting the importance of balanced datasets.
3. **Physical Feature Variation**:
   - Changes to bill and flipper lengths resulted in significant variability in body mass predictions, showcasing the sensitivity of the regression model.

### Sensitivity Analysis
- Increasing bill length by 2 mm led to a slight decrease in predicted body mass, reflecting biological assumptions.
- Flipper length variations showed a direct correlation with body mass predictions, emphasizing their importance as a feature.

## Dependencies
To run this project, install the following dependencies:

- **Python (>=3.7)**
- **TensorFlow (>=2.0)**: For neural network implementation.
- **Scikit-learn (>=0.24)**: For clustering and preprocessing.
- **Matplotlib (>=3.3)**: For visualizations.
- **Pandas (>=1.2)**: For data manipulation.
- **Numpy (>=1.19)**: For numerical computations.

## How to Run the Project
1. Clone the repository or download the project files.
2. Ensure all dependencies are installed using:
   ```bash
   pip install -r requirements.txt
   ```
3. Place the penguins dataset in the project directory with the filename `penguins.csv`.
4. Run the provided Jupyter Notebook or Python script to reproduce the analysis:
   ```bash
   jupyter notebook project_analysis.ipynb
   ```

## File Structure
- **`project_analysis.ipynb`**: Main notebook containing code for the analysis.
- **`penguins.csv`**: Dataset used for training and testing.
- **`README.md`**: Project overview and instructions.

## Acknowledgments
This project utilizes the Penguins dataset for analyzing machine learning models' performance and their application in ecological research. Special thanks to the open-source libraries that made this project possible.

