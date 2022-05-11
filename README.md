# Neural_Network_Charity_Analysis

## Overview
### Purpose
A philanthropic foundation, Alphabet Soup, wants to know that their donations are being used efectively. Therefore, the goal of this project is to utilize machine learning and neural networks to create a binary classifier that is capable of predicting whether applicants will be successful or not if funded by the philanthropic group. Numerous features (x variables) are utilized to make this distinction between effective and ineffective organizations. The results of this project will help provide guidance to Alphabet Soup in making future donations. The data contains information from over 34,000 organizations that have received funding over the years and the result of how effectively the money was used.

## Results
### Data Preprocessing
During the preprocessing process, columns like id numbers and names are removed as they are not useful for the model. For categorical variables, "rare" occurences are grouped together in a "Other" column. Additionally, this categorical data needs to be encoded in order to compile, train and evaluate the model. This process creates a new column for each unique categorical variable.

![](analysis/encodedDF.png)

Target Variable (Varaible we are trying to predict):<br>
    - IS_SUCCESSFUL: Was the money used effectively<br>

Features of Model (Input data): <br>
    - APPLICATION_TYPE: Application type<br>
    - AFFILIATION: Affiliated sector of industry<br>
    - CLASSIFICATION: Classification<br>
    - USE_CASE: Use case<br>
    - ORGANIZATION: Organization type<br>
    - STATUS: Active status<br>
    - INCOME_AMT: Income classification<br>
    - SPECIAL_CONSIDERATIONS: Special Considerations for application<br>
    - ASK_AMT: Funding Amount requested<br>

Removed columns:<br>
    - Identification columns<br>
        - EIN<br>
        - Name<br>

### Compiling, Training, Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?
Were you able to achieve the target model performance?
What steps did you take to try and increase model performance?


### Summary
Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.