# deep-learning-challenge
Module21

## Overview
The purpose of this project was to create a model for Alphabet Soup in order to predict whether applicants would be successful or not for funding. The minimum accuracy score required was 75%

## Data processing
What variable(s) are the target(s) for your model?
* The target variable was the "IS_SUCCESSFUL" from the 'application_df' for both attempts

What variable(s) are the features for your model?
* For both attempts, the feature variabless were all the other columns in the 'application_df' except for the "IS_SUCCESSFUL" column

What variable(s) should be removed from the input data because they are neither targets nor features?
* The "EIN" column was removed for both attempts.
* "NAME" column was also removed for the first attempt, the second attempt did not have any additional columns removed.

## Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why?

* The first attempt had 2 hidden layers, with 20 nodes for the first layer and 10 nodes for the second layer. 100 epochs were used. The "relu" activation function was used for both hidden layers, and the "sigmoid" activation function was used for the output layer. This resulted in a 73% accuracy
![Screenshot](/var/folders/5z/xt2b2jzn6r5_2g3q71bdwxsh0000gn/T/TemporaryItems/NSIRD_screencaptureui_3yNlF3/Screenshot 2024-02-21 at 8.44.01 PM.png)

* The second attempt had 3 hidden layers, with 15, 10, and 5 nodes. Epoch utilization was reduced to 50, mainly due to cut back on personal waiting time for it to load.The first layer used the "relu" activization function, and all the other layers, including the output layer used the "sigmoid" function. Only the "EIN" column was dropped from the original dataset, and the "APPLICATION_TYPE" and "CLASSIFICATION" columns were left seperate instead of combining. The accuracy level of the second model was 77%. 
![Screenshot](/var/folders/5z/xt2b2jzn6r5_2g3q71bdwxsh0000gn/T/TemporaryItems/NSIRD_screencaptureui_tQKtxI/Screenshot 2024-02-21 at 8.43.09 PM.png)

* Were you able to achieve the target model performance?
I was successful in achieving the minimum requirement of 75% accuracy with the second model, at 77% accuracy

* What steps did you take in your attempts to increase model performance?
*- I added more columns to the dataset by keeping the "NAME" column, and keeping the "CLASSIFICATION" and "APPLICATION_TYPE" columns separate. An extra hidden layer was added, and I changed the nodes to 15, 10, and 5. 

*-Activization level for the first hidden layer remained as "relu" and the other hidden layers used a "sigmoid" activization level. This was more due to a guess and check method.

*-In order to cut back on personal waiting time, epochs were changed from 100 to 50


## Summary
In conclusion, adding extra hidden layers helped the accuracy level increase drastically, as well as changing the amount of columns in the dataset. The first attempt may have been underfit by the number of columns, and rendered a 73% accuracy score, rather than the 77% accuracy score of the second attempt.
