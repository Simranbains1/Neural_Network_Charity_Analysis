# Neural_Network_Charity_Analysis

## Overview of the Analysis
This project aimed to create a binary classifier that can predict whether applicants will be successful if they are funded by Alphabet Soup. To achieve this we had to preprocess the dataset, compile, train, and evaluate the neural network model, and optimize our model. 

## Results
### Data Preprocessing
What variable(s) are considered the target for your model?
- The target is the "Is-Successful" column

What variable(s) are considered to be the features for your model?
- NAME
- APPLICATION
- TYPE
- AFFILIATION
- CLASSIFICATION
- USE_CASE
- ORGANIZATION
- INCOME_AMT
- SPECIAL_CONSIDERATIONS
- STATUS
- ASK_AMT

What variable(s) are neither and should be removed from the input data? 
- SPECIAL_CONSIDERATIONS should be removed because it cannot be quantified and only a small percentage of cases had special consideration
- STATUS should be removed because the value was (1) in each row

### Compiling, Training, and Evaluating the Model
How many neurons, layers, and and activation functions did you select for your neural network model, and why?
- There are three hidden layers each with many neurons. In order the activations were:
  - 'relu'
  - 'sigmoid'
  - 'sigmoid'
- The output function was also 'sigmoid'

Were you able to achieve the target model performance?
- Yes 

What steps did you take to try and increase model performance?
- Converted the NAME column into data points
- Added a third layer 
- Used the "sigmoid" activation function 

Difference in accuracy between the initial (top) and optimized (bottom) formulas
![AlphabetSoupCharity.png](https://github.com/Simranbains1/Neural_Network_Charity_Analysis/blob/main/AlphabetSoupCharity.png)
![AlphabetSoupCharity_Optimization.png](https://github.com/Simranbains1/Neural_Network_Charity_Analysis/blob/main/AlphabetSoupCharity_Optimization.png)

## Summary
We were able to increase the accuracy past 75% and learned that applicants are 80% more likely to be succesful if their name appears more than five times, and if they have a specific application type and classification. 

The Random Forest model was a great option for this model because we were able to get a high accuracy.
