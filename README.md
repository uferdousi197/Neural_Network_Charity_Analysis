# Neural_Network_Charity_Analysis

# Overview of the Analysis
In this dataset I used the features to create a binary classifier which will help predict if applicants will be funded by a Charitable organization called Alphabet Soup. For this analysis we had a dataset containing various measures on 34,000 organizations that have been funded by Alphabet Soup. This project compromised of the following 3 steps:

- Preprocessing the data for the neural network
- Compile, Train and Evaluate the Model
- Optimizing the model
- Results

# Data Preprocessing
- Variable that was considered as the target for my model: IS_SUCCESSFUL Column
- Variables that were considered features for my model: Every Column except for IS_SUCCESSFUL which is our target and the ones we will drop
- Variable that were neither targets or features for the dataset: Columns that I dropeed are EIN, NAME because they will have little to no impact om our outcome

# Compiling, Training and Evaluating the Model
The number of neurons, layers, and activation functions I selected for my neural network model:

For my neural network model, I had 2 hidden layers. My first layer had 80 neurons, the second had 30 along with an output layer. 
The first and second hidden layer have the "relu" activation function and the activation function for the output layer is "sigmoid."


# Was the model able to achieve the target model performance?
The model was not able to reach the target of 75%. The accuracy for my model was 69%.


# The steps taken to try and increase model performance

- Method 1: Removed additional feature, that is the 'USE_CASE' column. 
Rest of the model components stayed the same, however model accuracy went down to 63%.

- Method 2: Adding Additional neurons to hidden layers and additional hidden layers are added. 
The accuracy went down again, this time it was 53%.

- Method 3: Changing activation function of output layer from "sigmoid" to "tanh." 
The accuracy of the model went down even more to 50%.

# Summary
The model ended up with an accuracy score of 50% post optimization. 
The initial neural network had a accuracy score of 69%. This loss in accuracy can be explained from the fact that the model was overfitted. 
Furthermore, we could also optimize our neural network by removing features or simply adding more data to the dataset and increase accuracy. Since our accuracy score wasn't up to the standard with the neural networks, we could have made use of the Random Forest classifiers. The Random Forest model is robust and due to it's sufficient number of estimators and tree depth, it woudl fit better. The Random Forest model have a faster performance than neural networks and would prevent the data from being overfitted.
