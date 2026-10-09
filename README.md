# SWYNEX Task 3: Modeling and Evaluation

## Objective

Build and evaluate a baseline machine-learning classification model to predict passenger survival using the Titanic dataset.

## Dataset

* **Source:** Titanic passenger dataset
* **Records:** 891
* **Original features:** 12 columns
* **Target variable:** `Survived` (0 = did not survive, 1 = survived)

The cleaned dataset from Task 1 was reused for this project.

## Technologies Used

* Python
* Pandas
* Scikit-learn
* Matplotlib
* Seaborn
* Jupyter Notebook

## Methodology

1. Loaded the cleaned Titanic dataset.
2. Selected passenger class, sex, age, family-related variables, fare, and embarkation port as input features.
3. Encoded categorical features using one-hot encoding.
4. Split the data into 80% training and 20% testing sets, using stratification.
5. Trained a Logistic Regression baseline model.
6. Evaluated the predictions using accuracy, precision, recall, F1-score, and a confusion matrix.

## Evaluation Results

| Metric                         | Result |
| ------------------------------ | -----: |
| Accuracy                       |    80% |
| Precision — Class 1 (Survived) |    79% |
| Recall — Class 1 (Survived)    |    67% |
| F1-score — Class 1 (Survived)  |    72% |
| Weighted F1-score              |    80% |

## Key Findings

* The model achieved approximately 80% accuracy on the test dataset.
* It identified non-survivors more effectively than survivors.
* The recall for survivors was approximately 67%, meaning some actual survivors were missed.
* The confusion matrix helped distinguish correct predictions from false positives and false negatives.

## Limitations

* The dataset is historical and may not generalize to other situations.
* Median and mode imputation may introduce bias.
* Logistic Regression may not capture complex relationships.
* The model uses a limited set of features.
* Extensive hyperparameter tuning and comparisons with other algorithms were not performed.
* The model identifies predictive patterns, not causal relationships.

## Future Improvements

* Compare Logistic Regression with Decision Tree and Random Forest models.
* Tune model hyperparameters.
* Investigate feature importance and class imbalance.
* Compare evaluation metrics across models.

## Repository Contents

* `task3_modeling_evaluation.ipynb` — Modeling, evaluation, and explanations.
* `cleaned_titanic.csv` — Cleaned dataset.
* `README.md` — Project documentation.

## Conclusion

This project demonstrates a complete baseline classification workflow, from preparing features and training a model to evaluating its predictions and documenting its limitations.
