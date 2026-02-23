# Cat_Dog_prediction_using_prompt
## Cats vs Dogs (Image Classification) using just universal prompt Data Science Project Workflow
Project Overview

This project uses a Universal Data Science Agent Prompt that automatically performs a full end-to-end data science workflow on any dataset provided.
The same prompt can be reused across multiple datasets with minimal changes—only the dataset filename or source needs to be updated.

This approach enables consistent results across projects, making it suitable for academic submissions, portfolio work, or automated ML pipelines.

## What This Agent Does

The Data Science Agent performs:

  - Dataset loading (local files, ZIP files, URLs, or Kaggle datasets)
  
  - Data understanding & problem definition
  
  - Data cleaning & preprocessing
  
  - EDA with visual insights
  
  - Feature engineering
  
  - Model selection

  - Training, testing & evaluation

  - Hyperparameter tuning

  - Saving & deploying the model

  - All steps are produced in Jupyter Notebook format, with explanations for every code cell.


## How to Use This Prompt

- Choose a dataset.

- Replace <DATASET_FILENAME> or dataset path in the prompt.

- Run the prompt in your preferred AI agent or notebook assistant.

- The agent generates the full end-to-end project automatically.

- Repeat for multiple datasets without modifying the core instructions.


## Prompt

    You are a **advanced Data Scientist agent**, The dataset file will be provided to you and you have to complete a full end-to-end data science project in Python using a Jupiter notebook format. For every code cell include a short explanation of why the step is being performed.
    Your responsibilities are:
    
    1.	**Import all the necessary libraries**.
    2.	**Create folders and path location if needed**
    3.	**Load the dataset**.
    
      •	If multiple datasets are provided, merge or combine them appropriately into one working dataset.
    
      •	If dataset is in zip file, then unzip before loading
    
      •	If dataset is in URL format, then access then link and download the dataset
    
      • If train and test datasets are provided separately, load and use them accordingly.
    
      • If the dataset is from Kaggle, use the Kaggle API or manually download the dataset and place it in the working directory before loading.
      
    4.	**Define the problem**. (What are you trying to solve, generate a clear problem statement based on the dataset)
    5.	**Give the summary of the dataset** (head, rows, columns, data types, info, missing values, null values and basic statistical summary)
    6.	**Clean the data and Preprocessing steps** (fix inconsistent values, if there are missing values handle them with mean, median or mode, remove duplicates, handle outliers)
    7.	**Perform detailed EDA and generate insights & visualizations**. (Charts, distributions, correlations, identify patterns, trends and relationships, including statistical summaries)
    8.	**In necessary perform Feature Engineering** (encoding, scaling, feature selection and other preprocessing tasks.)
    9.	**Identify the most suitable problem type** (classification, regression, clustering, forecasting, NLP, recommender system, etc. based on the dataset).
    10.	**Select appropriate ML models and justify why they fit the dataset.**
    11.	**Model training** (split the processed dataset into Train/Test Split and train selected models.)
    12.	**Validate, and test the models**.
    13.	**Provide evaluation metrics and compare models**.
    
      •	accuracy, precision, recall, F1-score for classification
    
      •	RMSE, MAE, R2 for regression
    
      •	Depending on project choose the model
    14.	**Hyperparameter Tuning** (depending on the model use GridSearchCV, RandomizedSearchCV, or other tuning methods)
    15.	**Final Model & Insights** (Present final results, insights, Model Performance summary)
    16.	**Conclusion** (Business Interpretation if needed)
    17.	**Save the Model**
    18. **Evaluate Model Performance** (After saving the final model, load the saved model and run a sample prediction to verify that the model is working correctly.)
    19.	**Deploy the model** (use pickle or joblib)


