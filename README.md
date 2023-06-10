# Neural_Network_Charity_Analysis


> With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

Programming Language: Python 
Libraries: Sci-kit Learn, Keras Tuner, Tensorflow, Pandas, Matplotlib

## Overview of the analysis: Explain the purpose of this analysis.

This project is an introduction to neural networks. The question that we wanted to answer was a perfect for supervised machine learning.  This algorithm that we created was a great example of a binary classifier. 

## Results: Using bulleted lists and images to support your answers, address the following questions.

### Data Preprocessing

What variable(s) are considered the target(s) for your model?

* The `"IS_SUCCEESSFUL"` column is the target variable.

What variable(s) are considered to be the features for your model?

* The remaining columns would be considered features. For example, `"APPLICATION_TYPE"`, `"AFFILIATION CLASSIFICATION"`, `"USE_CASE"`, `"ORGANIZATION"`, `"STATUS"`, `"INCOME_AMT"`, `"SPECIAL_CONSIDERATIONS"`, and `"ASK_AMT"`.

What variable(s) are neither targets nor features, and should be removed from the input data?

* Id columns should be removed from the input data. For example, `"EIN"` and `"NAME"` are id columns that would not add any meaningful information to the model.

Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?

* Neurons: 80 in layer 1, 30 in layer 2, and 1 in the output layer.
* Layers: 3 layers 
* Activation Functions: 1st and 2nd layer were relu and the output layer was sigmoid

The rule of thumb for number of neurons in the hidden layer is two to three times the number of inputs, so that's how that was decided. 
The number of layers was a guess.  The first two layers using relu is just a guess.  The output layer can be sigmoid based on our target data being binary.

Were you able to achieve the target model performance?

Yes, I was able to achieve a balanced accuracy score of 78%.  

What steps did you take to try and increase model performance?

This was done with the help of hyper parameter tuning. I adjusted the features to no luck. I adjusted how we bagging of certain features. 

## Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.

This deep learning model does a decent job of predicting the success from funding by Alphabet.  Bek could have used any other classification algorithm such as random forest classifier.  My reasoning is that there is only one target, so running it through a deep learning model may not be necessary to get accurate predictions. The target has only two categories, so classification algorithms will likely work fine for this example. 
