# Neural Network Charity Analysis

## Overview	

The purpose of this analysis is to help Alphabet Soup, a philanthropic nonprofit organization determine which organizations to give donations to who are most likely to use the money effectively. Not every donation Alphabet Soup makes is used for good. In the past, organizations or companies have taken the donations and not done anything impactful with it, or simply disappeared. Using Python’s Tensorflow library, I will create a deep learning neural network model to predict which organizations are worth donating to, and which are not. 

## Results

### Data Preprocessing
- The target for the neural network model is the IS_SUCCESSFUL binary classifier.
- The features for the neural network model are APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT.
- The variables EIN and NAME are identifier columns. These are neither targets nor features and were removed from the input dataset.

### Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why?
  - My neural network model has two hidden layers. The first hidden layer has 80 neurons, and the second hidden layer has 30 neurons. I chose to use the ReLu activation function for both of my hidden layers and the Sigmoid activation function for my output layer.
- Were you able to achieve the target model performance?
   - I was not able to achieve the target model performance of 75% accuracy for my neural network model. My model achieved 72.6% accuracy.
- What steps did you take to try and increase model performance?
  - I added a hidden layer with 30 neurons and used the ReLu activation function.
    - This model achieved 73% accuracy.
  - I modified the activation functions within the hidden layers. I used the tanh activation function instead of ReLu.
    - This model achieved 72.4% accuracy.
  - I added neurons to the hidden layers. I increased the neurons for the first hidden layer from 80 to 120 and increased the neurons for the second hidden layer from 30 to 60.
    - This model achieved 72.9% accuracy.

## Summary 

My neural network model did not achieve the 75% accuracy target. The highest accuracy I was able to achieve was 73% by increasing the number of hidden layers in my neural network model. A model that can only predict the outcome correctly 73% of the time is not very reliable. As a next step, I would try to create a Random Forest Classifier model and compare the results to my neural network model. I would choose this method because the Random Forest Classifier is a robust and accurate model that uses multiple weaker learning models to make classifications, with less processing power.
