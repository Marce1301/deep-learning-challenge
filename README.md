# Deep-learning-challenge
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, you have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as:

* EIN and NAME—Identification columns
* APPLICATION_TYPE—Alphabet Soup application type
* AFFILIATION—Affiliated sector of industry
* CLASSIFICATION—Government organization classification
* USE_CASE—Use case for funding
* ORGANIZATION—Organization type
* STATUS—Active status
* INCOME_AMT—Income classification
* SPECIAL_CONSIDERATIONS—Special considerations for application
* ASK_AMT—Funding amount requested
* IS_SUCCESSFUL—Was the money used effectively

This challenge was performed using Google Colab

## Instructions
# Step 1: Preprocess the Data

Using your knowledge of Pandas and scikit-learn’s StandardScaler(), you’ll need to preprocess the dataset. 

Start by uploading the starter file to Google Colab, then using the information we provided in the Challenge files, follow the instructions to complete the preprocessing steps.

![image](https://github.com/Marce1301/deep-learning-challenge/assets/119386031/41c75a6e-91fa-4452-8def-866a5ad3ffb6)

Read in the charity_data.csv to a Pandas DataFrame, and be sure to identify the following in your dataset:
What variable(s) are the target(s) for your model?
What variable(s) are the feature(s) for your model?

Drop the EIN and NAME columns.

![image](https://github.com/Marce1301/deep-learning-challenge/assets/119386031/03de66f3-1346-409b-a4bb-611d5e7fcd95)

Determine the number of unique values for each column.

![image](https://github.com/Marce1301/deep-learning-challenge/assets/119386031/d0a609aa-dcb7-4f75-b503-1ba6b7677c88)

For columns that have more than 10 unique values, determine the number of data points for each unique value.

Use the number of data points for each unique value to pick a cutoff point to bin "rare" categorical variables together in a new value, Other, and then check if the binning was successful.

![image](https://github.com/Marce1301/deep-learning-challenge/assets/119386031/feae5429-007f-4183-bdfd-b9416b4c2406)

Use pd.get_dummies() to encode categorical variables.

![image](https://github.com/Marce1301/deep-learning-challenge/assets/119386031/96cabaf1-c173-4f79-933a-733eca8d1171)

Split the preprocessed data into a features array, X, and a target array, y. Use these arrays and the train_test_split function to split the data into training and testing datasets.

![image](https://github.com/Marce1301/deep-learning-challenge/assets/119386031/ade229ed-3f30-4714-955c-a851b576ab11)


Scale the training and testing features datasets by creating a StandardScaler instance, fitting it to the training data, then using the transform function.

![image](https://github.com/Marce1301/deep-learning-challenge/assets/119386031/5843bdb1-5346-4239-a4ae-4263295b6b6d)


# Step 2: Compile, Train, and Evaluate the Model
Using your knowledge of TensorFlow, you’ll design a neural network, or deep learning model, to create a binary classification model that can predict if an Alphabet Soup-funded organization will be successful based on the features in the dataset. You’ll need to think about how many inputs there are before determining the number of neurons and layers in your model. Once you’ve completed that step, you’ll compile, train, and evaluate your binary classification model to calculate the model’s loss and accuracy.

* Create a neural network model by assigning the number of input features and nodes for each layer using TensorFlow and Keras.
* Create the first hidden layer and choose an appropriate activation function.
* Create an output layer with an appropriate activation function.
* Check the structure of the model.
* Compile and train the model.
* Create a callback that saves the model's weights every five epochs.
* Evaluate the model using the test data to determine the loss and accuracy.
* Save and export your results to an HDF5 file. Name the file AlphabetSoupCharity.h5.

![image](https://github.com/Marce1301/deep-learning-challenge/assets/119386031/3b9b03a6-0af2-49e7-ba8b-505d5abb5c1d)

![image](https://github.com/Marce1301/deep-learning-challenge/assets/119386031/ea3bac1c-c3bd-420e-b034-806377d3eb30)

![image](https://github.com/Marce1301/deep-learning-challenge/assets/119386031/ce9af6bf-9664-43a9-be4b-381d4b4b9684)

# Step 3: Optimize the Model

Using your knowledge of TensorFlow, optimize your model to achieve a target predictive accuracy higher than 75%.

Use any or all of the following methods to optimize your model:

* Adjust the input data to ensure that no variables or outliers are causing confusion in the model, such as:
* Dropping more or fewer columns.
* Creating more bins for rare occurrences in columns.
* Increasing or decreasing the number of values for each bin.
* Add more neurons to a hidden layer.
* Add more hidden layers.
* Use different activation functions for the hidden layers.
* Add or reduce the number of epochs to the training regimen.
* Create a new Google Colab file and name it AlphabetSoupCharity_Optimization.ipynb.
* Import your dependencies and read in the charity_data.csv to a Pandas DataFrame.
* Preprocess the dataset as you did in Step 1. Be sure to adjust for any modifications that came out of optimizing the model.
* Design a neural network model, and be sure to adjust for modifications that will optimize the model to achieve higher than 75% accuracy.
* Save and export your results to an HDF5 file. Name the file AlphabetSoupCharity_Optimization.h5.
![image](https://github.com/Marce1301/deep-learning-challenge/assets/119386031/ce9af6bf-9664-43a9-be4b-381d4b4b9684)
# Step 4: Write a Report on the Neural Network Model

https://github.com/Marce1301/deep-learning-challenge/blob/main/Starter_Code/Report.md


# References
IRS. Tax Exempt Organization Search Bulk Data Downloads. https://www.irs.gov/
