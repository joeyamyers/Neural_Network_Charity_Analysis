# Neural_Network_Charity_Analysis

## Overview
### Purpose
A philanthropic foundation, Alphabet Soup, wants to know that their donations are being used efectively. Therefore, the goal of this project is to utilize machine learning and neural networks to create a binary classifier that is capable of predicting whether applicants will be successful or not if funded by the philanthropic group. Numerous features (x variables) are utilized to make this distinction between effective and ineffective organizations. The results of this project will help provide guidance to Alphabet Soup in making future donations. The data contains information from over 34,000 organizations that have received funding over the years and the result of how effectively the money was used.

## Results
### Data Preprocessing
During the preprocessing process, columns like id numbers and names are removed as they are not useful for the model. For categorical variables, "rare" occurences are grouped together in a "Other" column. Additionally, this categorical data needs to be encoded in order to compile, train and evaluate the model. This process creates a new column for each unique categorical variable.

![](analysis/encodedDF.png)

Target Variable (Varaible we are trying to predict):
    - IS_SUCCESSFUL: Was the money used effectively

Features of Model (Input data):
    - APPLICATION_TYPE: Application type
    - AFFILIATION: Affiliated sector of industry
    - CLASSIFICATION: Classification
    - USE_CASE: Use case
    - ORGANIZATION: Organization type
    - STATUS: Active status
    - INCOME_AMT: Income classification
    - SPECIAL_CONSIDERATIONS: Special Considerations for application
    - ASK_AMT: Funding Amount requested

Removed columns:
    - Identification columns
        - EIN
        - Name

### Compiling, Training, Evaluatingg the Model