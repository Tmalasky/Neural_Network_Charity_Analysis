# Neural_Network_Charity_Analysis
Machine Learning and Neural Networks
## Overview
Using my knowledge of machine learning and neural networks, I will use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.
This new assignment consists of three technical analysis deliverables and a written report. You will submit the following:
- Deliverable 1: Preprocessing Data for a Neural Network Model
- Deliverable 2: Compile, Train, and Evaluate the Model
- Deliverable 3: Optimize the Model
- Deliverable 4: A Written Report on the Neural Network Model (README.md)

## Results
### Data Preprocessing

- What variable(s) are considered the target(s) for your model? The target for the model is the "Is-Successful" column. It signifies if the money was use effectively.

- What variable(s) are considered to be the features for your model? The features of this model are the NAME, APPLICATION, TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT,SPECIAL_CONSIDERATIONS, STATUS, and ASK_AMT.

- What variable(s) are neither and should be removed from the input data? ANSWER: EIN (Employer identificaiton) was dropped because the numbers could confuse the system into thinking its significant. A student could drop SPECIAL_CONSIDERATIONS because there is only a small percentage of cases that had any special consideration, and special considerations cannot be quantified. ANSWER: A student could drop STATUS because all rows were the same value, 1.

### Compiling, Training, and Evaluating the Model

- How many neurons, layers, and and activation functions did you select for your neural network model, and why? In this model there are three hidden layers each with many neurons, because this seeemed to increased the accuracy above 75%. The number of epochs wasn't changed. The first activation function was 'relu' but the 2nd and 3rd were 'sigmoid'and the output function was 'sigmoid'. Changing the 2nd and 3rd activation functions to 'sigmoid' also helped boost the accuracy.

- Were you able to achieve the target model performance? Yes

- What steps did you take to try and increase model performance? It required converting the NAME column into data points, which has the biggest impact on improving efficiency. And, it also required adding a third layer and using the "sigmoid" activation function for the 2nd and 3rd layer.

## Summary

Overall, by increasing the accuracy above 75% we are able to correctly classify each of the points in the test data 75% of the time. And, an applicant has a 80% chance of being successful if they have the following:

- The NAME of the applicant appears more than 5 times (they have applied more than 5 times)
- The type of APPLICATION is one of the following; T3, T4, T5, T6, T7, T8, T10, and T19
- The application has the following CLASSIFICATION; C1000, C2000, C3000, C1200, and C2100.

A good model to recommend is the Random Forest model because Random Forest are good for classification problems. Using this model produces a 78% accuracy.
