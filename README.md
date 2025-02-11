# Titanic Survival Prediction

## Overview

This repository contains a machine learning project aimed at predicting the survival of passengers aboard the Titanic. The project leverages the famous Titanic dataset, which includes information about passengers such as age, gender, class, and more. The goal is to build a predictive model that can accurately determine whether a passenger survived or not based on these features.

## Dataset

The dataset used in this project is the Titanic dataset, which is publicly available on [Kaggle](https://www.kaggle.com/c/titanic/data). It contains the following key features:

- **PassengerId**: Unique identifier for each passenger.
- **Survived**: Target variable (0 = No, 1 = Yes).
- **Pclass**: Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd).
- **Name**: Passenger's name.
- **Sex**: Passenger's gender.
- **Age**: Passenger's age.
- **SibSp**: Number of siblings/spouses aboard.
- **Parch**: Number of parents/children aboard.
- **Ticket**: Ticket number.
- **Fare**: Passenger fare.
- **Cabin**: Cabin number.
- **Embarked**: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton).

## Project Structure

```
titanic-prediction/
│
├── data/                    # Directory containing the dataset
│   ├── train.csv            # Training dataset
│   └── test.csv             # Test dataset
│
├── notebooks/               # Jupyter notebooks for exploratory data analysis and model building
│   ├── EDA.ipynb            # Exploratory Data Analysis
│   └── Model.ipynb          # Model Training and Evaluation
│
├── src/                     # Source code for the project
│   ├── data_preprocessing.py# Script for data preprocessing
│   ├── model.py            # Script for model training and evaluation
│   └── utils.py            # Utility functions
│
├── models/                  # Directory to save trained models
│
├── requirements.txt         # List of dependencies
│
├── README.md                # This file
│
└── LICENSE                  # License information
```

## Installation

To set up the environment and install the necessary dependencies, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/titanic-prediction.git
   cd titanic-prediction
   ```

2. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

### Data Preprocessing

Before training the model, the data needs to be preprocessed. This includes handling missing values, encoding categorical variables, and feature engineering.

Run the preprocessing script:
```bash
python src/data_preprocessing.py
```

### Model Training and Evaluation

To train the model and evaluate its performance, run the following script:
```bash
python src/model.py
```

This script will:
- Load the preprocessed data.
- Split the data into training and testing sets.
- Train a machine learning model (e.g., Random Forest, Logistic Regression).
- Evaluate the model's performance using metrics such as accuracy, precision, recall, and F1-score.
- Save the trained model to the `models/` directory.

### Exploratory Data Analysis (EDA)

For a detailed analysis of the dataset, you can explore the Jupyter notebook located in the `notebooks/` directory:
```bash
jupyter notebook notebooks/EDA.ipynb
```

## Results

The model's performance metrics will be displayed after running the `model.py` script. Additionally, you can find visualizations and insights from the EDA in the `EDA.ipynb` notebook.

## Contributing

Contributions are welcome! If you'd like to contribute, please fork the repository and create a pull request. You can also open an issue to discuss potential improvements or report bugs.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Kaggle for providing the Titanic dataset.
- The machine learning community for their valuable resources and tutorials.

