Overview of the analysis: Explain the purpose of this analysis.

  The purpose of this analysis is to help the non-profit organization predict what types of
  grant applicants have the greatest likelihood of a successful endeavor. The neural network
  can identify patterns in the data to help funders make better decisions about funding grant
  applicants.
  

Results: Using bulleted lists and images to support your answers, address the following questions:

Data Preprocessing

What variable(s) are the target(s) for your model?
  We are targeting whether or not a previous grant application was "successful." This can help identify
  patterns for future grant applicant funding decisions.

What variable(s) are the features for your model?
  The features for the model are variables describing the funding organization including it's income,
  the grant amount requested, and the type of organization.
  
What variable(s) should be removed from the input data because they are neither targets nor features?
  Variables removed should be those that would have a unique value for each organization (e.g., EIN, Name).

Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?
Were you able to achieve the target model performance?
I chose a moderate number of neurons for the models (32) in the first three models. For the fourth model,
I selected a higher numbner of neurons (64) to maybe improve accuracy. For the first three models, I iteratively
increased the number of layers using different techniques to try to improve accuracy. These techniques
to avoid overfitting the model (i.e., having too much "noise" or variables in the model that have 
no impact on the outcome). I used RELU to try to fit the model to a non-linear relationship
between the features and outcome (e.g., a curvilinear relationship).

What steps did you take in your attempts to increase model performance?
Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model 
could solve this classification problem, and then explain your recommendation.
The models were less than 75% accurate, meaning they only 75% of the outcomes correctly. In terms of loss, the
loss value is also consistently high (>=0.50) suggesting that there is not enough data to correctly predict the outcome.
