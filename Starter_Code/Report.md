### Deep-learning-challenge_report

## Overview

The nonprofit foundation, Alphabet Soup, requires a tool to assist in selecting applicants for funding who have the highest chance of success in their ventures. The goal is to create a binary classifier using machine learning and neural networks. A provided dataset contains information on over 34,000 organizations that have received funding from Alphabet Soup in the past. The dataset includes several columns that capture metadata about each organization, such as:

EIN and NAME: Identification columns that provide unique identifiers for each organization.

APPLICATION_TYPE: Represents the type of application submitted to Alphabet Soup.

AFFILIATION: Indicates the sector of industry to which the organization is affiliated.

CLASSIFICATION: Represents the government organization classification of each organization.

USE_CASE: Describes the purpose or use case for the funding requested by the organization.

ORGANIZATION: Indicates the type of organization (e.g., corporation, trust, association).

STATUS: Reflects the active status of the organization.

INCOME_AMT: Classifies the income level of the organization.

SPECIAL_CONSIDERATIONS: Captures any special considerations mentioned in the application.

ASK_AMT: Represents the funding amount requested by the organization.

IS_SUCCESSFUL: Indicates whether the money provided to the organization was used effectively.

By utilizing the provided dataset and its features, the objective is to develop a binary classifier that can predict whether an applicant will be successful if funded by Alphabet Soup. This predictive model will assist the business team at Alphabet Soup in making more informed decisions regarding funding allocation, ultimately improving the overall success rate of funded ventures.

# Results
## Data processing
 
The  variables of our model were EIN, NAME, APPLICATION TYPE_ AFFILIATION, CALSSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT AND IS_SUCCESSFUL
There were removed EIN and NAME variables because them don´t add relevant info to our model.
Both Clasification and application_type were features in the model.

![image](https://github.com/Marce1301/deep-learning-challenge/assets/119386031/410319a0-0788-475f-aadb-3c6152271731)

## Compiling, Training, and Evaluating the Model

Neural network (DNN) model was used with TensorFlow backend.

The number of hidden nodes (neurons) for the first and second hidden layers were 9 and 18 respectively.

![image](https://github.com/Marce1301/deep-learning-challenge/assets/119386031/1aa593b5-6185-422c-9c3d-f999e4a82f2b)

The model has a total of 595 parameters, all of which are trainable

![image](https://github.com/Marce1301/deep-learning-challenge/assets/119386031/749d97bc-945a-412a-8dc9-5df99d1cd8e2)

I trained the model with an epoch of 100 getting an accuracy of 74%

![image](https://github.com/Marce1301/deep-learning-challenge/assets/119386031/a4ea07bf-507b-427c-9d30-8435ad5229f7)

![image](https://github.com/Marce1301/deep-learning-challenge/assets/119386031/1aaa8c78-89e3-4922-ba3e-e21dba89d744)

# Summary

Based on the provided evaluation results, the trained model achieved an accuracy of approximately 72.72% on the test set.

This accuracy falls short of the desired target of 75%. While the model's accuracy is not as high as desired, it still provides some predictive capability. Several layers should be considered so I can get a higher accuracy prediction based on the model.

Regardless the complexity of working with deep machine learing it was very interesting for me to experiment with these techniques while carefully monitoring the model's performance on both the training and test sets.


