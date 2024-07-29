## Deep Learning Challenge

## Alphabet Soup Funding Final Analysis

# Purpose
In this project, we will develop a deep learning model to perform binary classification, aiming to predict the success of organizations funded by Alphabet Soup based on the features present in the dataset. We will utilize machine learning techniques and neural networks to analyze the charity_data.csv file, which contains information about organizations that have received funding from Alphabet Soup. By leveraging metadata columns, we seek to forecast the success of potential future applicants.

# Analysis
The target variable for the model is "IS_SUCCESSFUL". All remaining features are in the model with the exception of 'EIN' and 'NAME' as they were not needed for analysis. The Input layer was determined by the number of features in the data. I chose to use twice the number of features (n2) for my first hidden layer. Second layer consisted of the same number of features as neurons (n1).

For each of the hidden layers ReLU activation function was used. The output layer was neurons and used the Sigmoid activation function. Output for first run was as follows:
268/268 - 0s - 460us/step - accuracy: 0.7244 - loss: 0.5984
Loss: 0.5983566045761108, Accuracy: 0.7244315147399902

For optimized run, I used number of features * 3 for first hidden layer and number of features/2 for hidden layer 2.
268/268 - 0s - 947us/step - accuracy: 0.7314 - loss: 0.5716
Loss: 0.5715730786323547, Accuracy: 0.7314285635948181

My accuracy is at 73% accuracy. 


# Data Preprocessing
* What variable(s) are the target(s) for your model?
The target for each model was the IS_SUCCESSFUL column. The ultimate goal is to predict which applicants will be successful, so we will utilize all other features to ultimately make a predict

* What variable(s) are the features for your model?
The available features for my model are: EIN, NAME, APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT

* What variable(s) should be removed from the input data because they are neither targets nor features?
In the first model I ran I removed the EIN column and the NAME columns as instructed. In the first attempt at optimization, I added the NAME column back in case there was any bias to any specific organizations, as there where many that where listed multiple times.

# Alternative Solutions
I believe that experimenting with the number of neurons and hidden layers can get me to an accuracy above 75%. Other strategies that can improve accuracy: change activation functions, implement dropout regularization, adjust learning rate and optimizer, use batch normalization and increase training epochs or adjust batch size.

# Technical Skills
* Machine learning
* Deep learning
* Neural networks
* Tensorflow
* Pandas
* Python
* Statistical analysis

