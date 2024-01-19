# Wine Quality Prediction Project

## Overview

This project, conducted by Fahimul Gaffar for COMP 3400, focuses on predicting the quality of wines using a dataset containing various features related to wine composition. Two main approaches were explored for data preparation: predictor transformations and feature selection. Logistic regression models were built to assess the impact of these approaches on the accuracy of the predictive model.

## Data Preparation Approaches

### Predictor Transformations

In the first approach, five different transformations (logarithmic, square, square root, exponential, and reciprocal) were applied to the 'alcohol' predictor. The goal was to observe how these transformations affect the logistic regression model's accuracy. Results indicated that moderate transformations, such as square and square root, led to improved accuracy, highlighting the sensitivity of the model to changes in predictor distribution and scale.

### Feature Selection

The second approach involved dropping different subsets of predictors (1-3 predictors each) to evaluate their impact on model accuracy. The highest test accuracy was achieved when 'fixed acidity' was dropped, suggesting that this predictor might not be highly informative or could be collinear with other predictors. Overall, the accuracy remained relatively stable across different subsets, emphasizing the robustness of the dataset.

## Results and Insights

- **Predictor Transformations**: The square transformation of 'alcohol' led to the highest test accuracy (81.21%), suggesting that preserving or enhancing the relationship between the predictor and the target variable can improve model performance.

- **Feature Selection**: Dropped subsets of predictors showed relatively stable accuracy, with the highest accuracy (82.21%) achieved when 'fixed acidity' was removed. This indicates that careful feature selection can lead to slight improvements in model accuracy.

- **Comparing to Bottom-Line Accuracy**: Both approaches demonstrated slight improvements compared to the bottom-line accuracy, highlighting the importance of understanding the data and the impact of each predictor on the model.

## GitHub Repository Structure

- **Notebooks**: Contains Jupyter notebooks with the code for data preparation, model building, and analysis.
- **Data**: Includes the wine dataset used for the project.
- **Results**: Stores the results of predictor transformations and feature selection experiments.
- **Images**: Contains visualizations generated during the analysis.
- **README.md**: This file providing an overview of the project, methodologies, and key findings.

## How to Use

1. Clone the repository: `git clone [repository_url]`
2. Open and run the Jupyter notebooks in the 'Notebooks' folder sequentially.
3. Explore the results and visualizations in the 'Results' and 'Images' folders.

Feel free to adapt and build upon this project for your own analyses and experiments. Contributions and suggestions are welcome!
