# NLP-project

This repo implements a bag of words model and logistic regression to predict whether a Stack Overflow question will be open or closed based on the words in the question. 
Contains:

cleaning:
  - Uses beautifulsoup to remove html from the original dataset and spaCy to lemmatize the text and remove stopwords, punctuation, and spaces.

data_exploration:
  - Explores the clean dataset to find number of closed questions, number of open questions, and common scores.
  - Establishes correlation between scores and whether a question is open or closed.
  
modeling:
  - Implements bag of words and logistic regression models for the dataset as given (without regard to ratio of closed and open questions in the data). 
  - Discussion confusion matrix, diagnostics curves (precision-recall, ROC), and choice of logistic regression regularization parameter.
  
modeling-halfset_test:
  - Implements the same as the modeling notebook but for a manually constructed dataset that is 50% closed and 50% open. Discusses differences in the results as a result of that choice.
  
modeling-ratio_tests:
  - Uses the same models and loops through different ratios of closed-to-open questions in dataset to assess changes in accuracy and confusion matrix values.
