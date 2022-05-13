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
#### The Model
In the model, there are two hidden layers with 80 and 30 neurons, respectively. Both hidden layers use the ReLU activaton function to identify non-linear patterns in the data. In the ouput layer, I used the sigmoid function to report a binary classification because I wanted to separate the data into two clusters. 

#### Model Performance
My model did not reach the 75% accuracy threshold I set out to achieve as it only achieved 72.5%. Therefore, I must make modifications to the model to reach this threshold.

#### Optimizing the Model
In order to achieve a target predictive accuracy higher than 75%, I tried a few different modifications before I achieved the target accuracy. 



### Summary
Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.