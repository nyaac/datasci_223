# Classification on EMNIST Dataset

## Introduction

The aim of is to identify and classify letters from the emnist dataset. The exercise is split into two parts: 
    1. Classify letters a -> g
    2. Model showdown: upper vs lowercase on abcXYZ

# Part 1: Classify letters a -> g 

# Key Steps

Data Preprocessing 
- The emnist dataset is loaded and preprocessed. A subset of emnist dataset containing only the lowercase characters is loaded and labeled 'a2g'. The necessary libraries are imported for splitting the dataset, logistic regression, to calculate accuracy, random forest, evaluation, and visualization. 

Splitting Data
- The a2g data was split into X and Y. Then, further split into test and train datasets to ensure evaluation on unseen data. 

Model Evaluation on Logistic Regression and Random Forest
- For both models, using the trained model, the test set was used to predict label. The confusion matrix was generated for both models and visualized using a heatmap. 

Cross Validation
- Cross validation was performed on both models, computing the mean and standard deviation of accuracy scored across the folds of each model. 

# Part 2: Model showdown: upper vs lowercase on abcXYZ

# Key Steps

Data Preprocessing
- A subset of emnist dataset containing upper and lowercase letters is loaded and labeled 'abcxyz'. The necessary libraries are imported, such as GridSearchCV, Kfold, RandomForestClassifier, and NumPy.  

Splitting Data
- The abcxyz data was split into X and Y. Then, further splits into train and validation sets to ensure evaluation on unseen data. 

Parameter Tuning
- A parameter grid was established, however, fewer options were used for a quicker execution. Regarding the max depth, simple values were selected for the same reason.

Model Training
- The grid search object was fitted to the training set to find the optimal parameters. The best performing model was selected from the grid search. 

Combining Datasets
- The validation and train set were combined to retrain the model on the entire dataset, enhancing its performance. The best model is refitted on the combined data to obtain the finalized model. 

### Discussion

This exercise was very challenging and a little bit frustrating. It was more frustrating  because a lot of the time spent trying to figure out how to get the code to run efficiently and timely to actually see results. Overall, I think its a great exercise to show what it would be like to be a full-time data scientist.
