# Recommended ML Checklist


### Problem Definition
- [ ] Task Definition and Scope out Requirements
- [ ] Determine Project Feasibility
- [ ] Propose Model Metrics
- [ ] Setup Project Codebase

### Data Exploration
- [ ] Create Data Dictionary: Column Definition
- [ ] Check proposed Data Merging
- [ ] Write Down Data Assumption & Verify Data Assumption
- [ ] Perform Basic Data Profiling
- [ ] Flag out all Outlier Data, Data Inconsistencies, Missing Values
- [ ] Visualise the distribution for each feature / target column
- [ ] Visualise the correlation between the features and the target
- [ ] Visualise the scatter plot between features and target

### Data Cleaning
- [ ] Perform Data Type formatting
- [ ] Perform Missing Data imputation
- [ ] Perform Data Cleaning based on all of the problems defined above
- [ ] Perform Data Transformation on the  target, if needed

### Feature Engineering
- [ ] Perform Appropriate Train Test Split on the Data
- [ ] Perform feature engineering
- [ ] Perform feature aggregation
- [ ] Perform feature encoding
- [ ] Perform feature scaling / transformation
- [ ] Perform datetime feature engineering
- [ ] Perform feature selection, if needed

### Model Baseline
- [ ] Perform Model Baseline using Cross Validation Method
- [ ] Perform Feature Importance on each model on the Model Baseline
- [ ] Perform Error Analysis on each model on the Model Baseline
- [ ] Choose Few Models which performs well in the Model Baseline Test - make sure that the models are not highly correlated
- [ ] Build the metric function, if it is not readily available

### Model Building
- [ ] Build the Appropriate Model, using the model baseline as a performance gauge
- [ ] Perform Hyperparameter Tuning to the Model
- [ ] Build Ensemble with each of the model, aggregated with Linear Regression

### Analysis
- [ ] Perform Feature Importance on each model on the Final Model
- [ ] Perform Error Analysis on each model on the Final Model
- [ ] Perform Regression / Classification report on the Final Model
