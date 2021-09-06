# Neural Networks and Deep Learning Models

## Overview of the Analysis
AlphabetSoup wants to create a model to better understand which organizations are worth donating to and which are high risk. Our task was to create a mathematical, data-driven solution by designing and training a depp neural network. We used Python and the "TensorFlow" library to accomplish the project.

## Results
### Data Preprocessing
- What variable(s) are considered the target(s) for your model?
  - "IS_SUCCESSFUL"

- What variable(s) are considered to be the features for your model?
  - "APPLICATION_TYPE"
  - "AFFILIATION" 
  - "CLASSIFICATION" 
  - "USE_CASE" 
  - "ORGANIZATION" 
  - "INCOME_AMT" 
  - "SPECIAL_CONSIDERATIONS" 
  - "ASK_AMT" 
  - "STATUS"

- What variable(s) are neither targets nor features, and should be removed from the input data?
  - "EIN"
  - "NAME"

### Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why?
  - The most successful neural model had 3 hidden layers with 240, 80, and 60 neurons respectively. We used a "ReLU" activation function for the middle layers and a "Sigmoid" activation function for the outer layer. This model was able to achieve the highest accuracy for all optimization trials at 73%.

- Were you able to achieve the target model performance?
  - We were unable to achieve the target model performance of 75% or greater. Our best optimization model achieved 73% accuracy. 

- What steps did you take to try and increase model performance?
  - We changed the number of neurons in the hidden layers.
  - we changed the activation functions of the hidden layers.

## Summary
Unfortunately, we were unable to achieve the target model performance of 75% accuracy, with our best optimization model achieving 73% accuracy. The final model had 3 hidden layers with 240, 80, and 60 neurons respectively; and used a "ReLU" activation function for the middle layers and a "Sigmoid" activation function for the outer layer.

### Recommendation
We could try running this data with a Random Forest Classifiers model, since this model easily handles both outliers in the data and nonlinear forms of data. 
