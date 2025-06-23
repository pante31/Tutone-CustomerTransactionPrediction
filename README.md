# Santander Customer Transaction Prediction

Kaggle competition for the Project Work in _Machine Learning and Data Mining_

## Task Description

![ATM machines.](https://storage.googleapis.com/kaggle-media/competitions/santander/atm_image.png)

In this challenge, the objective is to identify which customers will make a specific transaction in the future, irrespective of the amount of money transacted. The data provided for this competition has the same structure as the real data used to solve this type of problem.
This challenge require to perform **binary classification**.

## Dataset Description

There is an anonymized dataset containing numeric feature variables, the binary `target` column, and a string `ID_code` column.
The task is to predict the value of `target` column in the test set.

### File descriptions

  - **train.csv** - the training set.
  - **test.csv** - the test set. The test set contains some rows which are not included in scoring.
  - **sample_submission.csv** - a sample submission file in the correct format.

## Results

After trying three different models, these are the final results:
- The model that delivered best **accuracy** [_**0.92**_]: `GaussianNB(var_smoothing = 1e-08)`
- The model that delivered best **precision** [_**0.85**_]: `GaussianNB(var_smoothing = 0.001)`
- The model that delivered best **recall** [_**0.68**_]: `GaussianNB(var_smoothing = 1e-09)`
- The model that delivered best **f1_score** [_**0.72**_]: `GaussianNB(var_smoothing = 1e-09)`

Also the other two models (`DecisionTreeClassifier`, `KNeighborsClassifier`) obtained decent result, but the best one, considering all scorings, is the `GaussianNB`.

## License

[MIT](https://choosealicense.com/licenses/mit/)
