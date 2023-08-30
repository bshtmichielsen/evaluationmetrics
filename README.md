# evaluationmetrics

Exercise

First run the notebook as given to see if it loads the data correctly, after that continue with the exercise below.




Cross Validation

When training the model and tuning its hyperparameters, overfitting on the training data is possible. Therefore you need to apply cross validation to avoid overfitting. Perform 5-fold cross-validation using the function cross_val_score. Show what the accuracy scores are, and calculate the average accuracy score.




StratifiedKFold

The function StratifiedKFold is a variation of k-fold which returns stratified folds: Each set contains approximately the same percentage of samples of each target class as the complete set. Apply StratifieldKFold on the face recognition with k = 5. Print out the accuracy score of each fold, and calculate the average accuracy score.




Glasses

Instead of recognising people, the same dataset can also be used to decide whether a person is wearing glasses or not. This is a binary problem for which you need to make a new target variable 'glasses' which has either 0 or 1. Use the indices below to know which images have glasses and put a 1 in the target variable. The indices indicate ranges, so for example (10, 19) means images 10 up to (and including?) 19 do have glasses. Then:

- Create a training & test set for this new problem
- Again train support vector machine, but this time for the new target named `glasses`.
- Show a classification report
- Apply cross validation to avoid overfitting




glasses = [
    (10, 19), (30, 32), (37, 38), (50, 59), (63, 64),
    (69, 69), (120, 121), (124, 129), (130, 139), (160, 161),
    (164, 169), (180, 182), (185, 185), (189, 189), (190, 192),
    (194, 194), (196, 199), (260, 269), (270, 279), (300, 309),
    (330, 339), (358, 359), (360, 369)
]





