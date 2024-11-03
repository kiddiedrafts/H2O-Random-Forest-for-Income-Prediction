# Income Prediction using Random Forest

## Description
This project implements a Random Forest model using the H2O library to predict income levels based on census data. The goal is to classify individuals' income as either less than or equal to $50K or greater than $50K, utilizing various demographic and economic features. The project includes data preprocessing step to handle missing values. It also evaluates the model's effectiveness using F1 scores to ensure a robust assessment of classification accuracy.

## Dataset
The dataset used in this project is sourced from Kaggle and can be found at the following link: [here](https://www.kaggle.com/uciml/adult-census-income).

### Dataset Description
The dataset contains various features related to individuals, including demographics and employment information. The target variable is `income`, which indicates whether the individual's income is less than or equal to $50K or greater than $50K.

- **Data/**: This folder will contain the dataset files downloaded from Kaggle.
- **Notebook/**: This folder will house your Jupyter notebooks. **Currently, we are working within the Notebook directory.**

## Project Structure
The main folders and files in the project are structured as follows:

```plaintext
Pistachio/
├── Data/
│   └── [dataset files will be here]             # Dataset CSV file
├── Notebook/
│   └── [your Jupyter notebooks will be here]    # Jupyter notebook with code                 
└── README.md                                    # Project documentation 
```

## Requirements
To run this project, you'll need the following Python libraries:
- `h2o`
- `pandas`
- `scikit-learn`

## Feature Engineering and Data Preprocessing
This project includes preprocessing steps such as:
- Handling missing values by replacing "?" with `NA`.
- Splitting the dataset into training and testing sets.
- Converting the DataFrame to H2OFrame for compatibility with H2O methods.

## Model Training
The model is trained using the H2O Random Forest algorithm with specified hyperparameters. Cross-validation is employed to enhance the robustness of the model.

## Model Performance
The model achieved the following `F1` scores:
- **F1 Score on Training Set:** 0.8670
- **F1 Score on Test Set:** 0.8561
