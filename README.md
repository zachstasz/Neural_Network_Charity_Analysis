# Neural Network Charity Analysis

## Overview of the Analysis

Using data from Alphabet Soup, we will create a neural network to determine how the company can best predict where to make investments.

## Results

- Data Preprocessing
  - The target variable for our model is "IS_SUCCESSFUL", the column which states whether the investment was successful or not.
  - The feature variables for our model are Application Type, Affiliation, Classification, Use Case, Organization, Status, Income Amount, Special Considerations, and Asking Amount.
  - The EIN and Name are neither targets or features, and should be removed from the data.

- Compiling, Training, and Evaluating the Model
  - In the original model, there were two hidden layers and one output layer to tackle the amount of data and variables.
    - The first hidden layer had 80 neurons.
    - The second hidden layer had 30 neurons.
    - Both hidden layers used the "relu" activation function because it enables nonlinear relationships.
    - The output layer used the "sigmoid" activation feature because it will produce a probability output.
  - The target model performance of 75% was not achieved. This model was at 73% accuracy. 
  - I made four changes in an attempt to increase the model accuracy.
    - I removed the "Special Considerations" column.
    - I added an additional hidden layer.
    - I changed the hidden layers' activation function to Leaky Relu.
    - I added additional neurons. 100 for the first layer, 40 for the second, and 40 for the third.

## Summary

Unfortunately even after we changed the model, the accuracy stayed the same at 73%.

To increase accuracy, we could remove more features or add more data to test another result. We could also have used Random Forrest Classifiers and seen if that model produced better results.
