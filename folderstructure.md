# Folder Structure

- `explore`: data exploration, feature exploration should be performed over here. This can be a preceeding step 
before `prepare`, or performed after the data is concatenated into a transform-ready format. 

- `prepare`: the goal of this folder is to give us a transform-ready format for both training and testing features and labels.
Often, the dataset obtained for training (might be a bunch of csvs) and testing (REST-API request) can be different. This 
folder is ought to perform necessary transformation such that both of the dataset is equal

- `transform`: feature engineering, feature encoding, Data Cleaning should be performed over here. After receiving both transform-ready dataset from `prepare`,
a transform process that is fitted on the traning dataset, and performed on both training and testing dataset, should be performed over here. This will give us model-ready training and testing dataset

- `model`: model training, model hyperparametertuning, model selection, can be done over here. 
The goal of this repository is to have a model which is fitted on the training dataset, and can be used to predict
training dataset, and testing dataset

- `evaluate`: the code to perform model validation using training / validation data should be contained over here.

- `analyze`: model analysis, feature analysis, error analysis should be performed over here. 
This should be a step after `evaluate`, where the performance of the model as well as feature performance can be 
analyzed. Error Analysis and Model explainability should also be put over here

- `serve`: this can contains scripts to perform batch model prediction (kaggle - csv), or online prediction (REST)

- `monitor`:(Optional) this can contain scripts which aid the model monitoring for an online system, or model reporting for batch system

- `main` : the pipeline of the model should be well defined here. `prepare`, `transform`, 
and `model` has given us the neccessary steps to generate training data, validation data, testing data, and model.
the exact steps taken to perform the end-to-end ML platform should be performed here, including both `evaluate` and `serve`

- `utils`: utility code, such as logging, managing environment variables, etc
