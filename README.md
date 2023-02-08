# Neural Network Charity Analysis

## Overview 
The non-profit foundation Alphabet Soup is set out to fund many organizations that “protect the environment, improve people’s well-being, and unify the world”. They have raised and donated over 10 billion dollars in the past 20 years. The data analysts’ team oversees the impact of each donation and vet potential recipients. However, not every donation has fulfilled its purpose with many organizations taking the money and disappearing. The purpose of this project is to use machine learning  and neural networks knowledge to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup, or if an organization can be a high risk.
With this goal in mind, it is necessary to design and train a deep learning neural network. This model will evaluate all the types of input data and produce a clear decision-making result.

## Results

  -**Data Preprocessing**
  
For the creation of the model, preprocessing of the data was done, and columns such as 
“EIN” and “NAME” were dropped, as they did not add any input value to the model; whereas the “IS_SUCCESSFUL” column is considered the target variable for the model. Furthermore, the columns "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE","ORGANIZATION", "INCOME_AMT", and "SPECIAL_CONSIDERATIONS” were used as the model features.
 
  -**Compiling, Training, and Evaluating the Model**
Continuing with the exploration and training of the data, through scaling the data was found to have 49 features, and 25,724 samples.  Two layers were used with 90 and 40 neurons for this model. The activation functions were ReLU for the hidden layers, because of the binary-classification nature of the data, which is also why a unique neuron was used for the output layer with its activation function: Sigmoid. For the compilation Adam optimizer was used for a faster computation time and fewer parameters required.
Moreover, when evaluating the model and observing if it had achieved the target model performance with accuracy results of 0.73 (rounding up), we can speculate that a better model can be applied for this analysis as it is not a high number for performance.

As an effort to try and increase model performance, the model was bucketed with the feature ASK_AMT to organize the values by intervals. Initially, 70 and 20 neurons were used for both layers, but the number of neurons were increased as mentioned before to the total of 90, and 40 to also add-on to these efforts and increase the accuracy of the model.

 ## Summary
Even though different efforts were made to create a model with a target of 75% accuracy, the model failed to reached this number. It is recommended that supervised machine learning be applied for this type of categorical data for better results. With Random Forest, both regression and classification tasks can be performed and provide a higher level of accuracy in predicting which organizations have a higher chance of success, and which organizations represent a high risk.
