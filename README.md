# CIC-Bell-DNS-EXF-2021 Multiclass Classification with data imbalancement

## Dataset Information

- **Dataset Name**: CIC-Bell-DNS-EXF-2021 Dataset [here](<https://www.unb.ca/cic/datasets/dns-exf-2021.html#:~:text=Furthermore%2C%20our%20proposed%20model%20could,from%20small%20to%20large%20sizes.>)
- **Dataset Source**: Publicly available cybersecurity threat intelligence dataset
- **Features**: 12 features
- **Data Samples**: 536,138

## Class Distribution

- Benign: 45%
- Heavy_Attack: 47%
- Light_Attack: 8%

## Data Preprocessing

After labeling the dataset, we observed the following class distribution:

- Benign: 45%
- Heavy_Attack: 47%
- Light_Attack: 8%

## Data Preprocessing

One of the initial challenges was dealing with duplicate data. After removing duplicate entries, we achieved an improved class balance with the following distribution:

- Benign: 97.85%
- Heavy_Attack: 1.39%
- Light_Attack: 0.76%

## Classification Models

We addressed the multiclass classification problem using the following techniques and machine learning models:

1. **SMOTE (Synthetic Minority Over-sampling Technique)**: A method to oversample minority classes by generating synthetic samples.
2. **SMOTEENN (SMOTE with Edited Nearest Neighbors)**: A combination of oversampling and undersampling techniques to balance the class distribution.
3. **SMOTETomek**: A combination of SMOTE and Tomek links, which aims to improve class balance.

We trained and evaluated these techniques with the following machine learning models:

- Decision Tree
- Naive Bayes
- AdaBoost
- Random Forest

## Performance Evaluation

We assessed the performance of the classification models using various metrics, including:

- **Confusion Matrix**: To analyze the model's ability to classify each class.
- **Accuracy**: A measure of overall model accuracy.
- **Precision**: Precision measures the model's ability to correctly classify positive instances.
- **F1 Score**: A harmonic mean of precision and recall.

For detailed information on the performance of each model, please refer to the [Benign-Attacked_classification.ipynb](Benign-Attacked_classification.ipynb) file.

Feel free to explore the code and results in this repository to gain insights into how we tackled this multiclass classification problem using the CIC-Bell-DNS-EXF-2021 dataset and various machine learning techniques.
