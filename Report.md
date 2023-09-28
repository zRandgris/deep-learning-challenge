# deep-learning-challenge
ML
## Overview of the Analysis

The purpose of this analysis is to use deep learning neral network models to create a model to predict and determine which organizations are more likely to become successful after receiving fundings.

## Results
### Data Processing 
1. What variable(s) are the target(s) for your model?
  - The Target Variable is 'IS_SUCCESSFUL', where 1 being successful and 0 being not
2. What variable(s) are the features for your model?
  -  variables used in this model includes every columns excluding 'IS_SUCCESSFUL' in the application_df
3. What variable(s) should be removed from the input data because they are neither targets nor features?
  -   'EIN','NAME' was dropped in the begining to create the application_df, since they are not needed.


### Compiling, Training, and Evaluating the Model

1. How many neurons, layers, and activation functions did you select for your neural network model, and why?
#### First
Neurons = 80, 30
hidden layers = 2
activation functions = relu, relu, sigmoid
#### Second
Neurons = 80
hidden layers = 1
activation functions = relu, sigmoid

#### Third
Neurons = 80, 30, 10
hidden layers = 3
activation functions = relu, relu, relu, sigmoid


3. Were you able to achieve the target model performance?
  - No
4. What steps did you take in your attempts to increase model performance?
  - Starting out with the default settings, while tuning, made drastic change on the first two attempts to see which directions did the result head towards.
  - Picked a middle ground for my third attempt
  - final trial, implemented different activation function to better fit the data.

### Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.
  - Overall my results are
** loss: 0.5517
accuracy: 0.7313 **
  - Using a different activation function may give better result
  - next time when starting out, decreasing the epoch while testing for faster run time.
