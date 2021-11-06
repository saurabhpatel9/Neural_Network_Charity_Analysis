# Neural_Network_Charity_Analysis

## Overview and Purpose
With the Utilization of Machine Learning and Neural Networks for this undertaking, I utilized the attributes in the dataset to create a binary classifier that will assist with predicting if the candidates that will be funded by a Charitable association called Alphabet Soup will be successful or not. 
For this purpose, we had a dataset containing different measures on 34,000 organizations that have been funded by Alphabet Soup. 
This task compromises of 3 stages listed below:

1. Preprocessing of the data
2. Compiling, Training and Evaluating of the Model
3. Optimizing the model

## Analysis & Results

### Data Preprocessing : Questions Answered Below
1. The variable IS_SUCCESSFUL Column is considered as the Target variable for the model.
2. The Variables that were considered features for my model include all attributes except for the target column IS_SUCCESSFUL and the dropped columns.
2. There are certain variables which are not valuable for the evaluation of our outcome, and thus, are considered neither targets nor features and are dropped to provide a clean analytical ground. The dropped attributes are EIN & NAME.

### Compiling, Training and Evaluating the Model
#### Q: In my neural network model, the chosen number of neurons, hidden layers, and activation functions are as follows:

There are 2 hidden layers - the first layer containing 80 nodes/neurons, the second layer containing 30 nodes/neurons and an output layer.
The first and second hidden layer have the "relu" activation function and the output layer has the most commonly used "sigmoid" activation function.

![firsta](https://user-images.githubusercontent.com/86158802/140626421-b1a860c5-0399-4bd1-ad51-5dc28153826a.PNG)

#### Q: Was the model able to achieve the target model performance?
The recorded accuracy for my model was approximately 67%, hence the model was not able to reach the targeted accuracy of 75% in model performance.

![firstb](https://user-images.githubusercontent.com/86158802/140626429-c2c03bf7-e5e8-43ac-9623-a37915817dc5.PNG)


## Optimization of the mode
Therefore, the steps taken in order to increase model performance include:

### First Attempt: Removal of additional feature
The column 'USE_CASE' was removed which brought the model accuracy rise upto 70%, and proved to be the best optimized model.

![attempt1a](https://user-images.githubusercontent.com/86158802/140626437-08f0e247-1e5c-49a5-a3f9-992db6ada934.PNG)
![1b](https://user-images.githubusercontent.com/86158802/140626439-152d6c16-dbe2-4b21-9c79-6147b3d828c3.PNG)
![1c](https://user-images.githubusercontent.com/86158802/140626441-174ec285-b3af-4c0c-b058-ff2e196a97ab.PNG)

### Second Attempt: Addition of Additional neurons and hidden layers
The addition of hidden layers and neurons made the model lose accuracy and brought it down to 59%.

![2a](https://user-images.githubusercontent.com/86158802/140626443-8494deb5-6a06-432d-88e5-5c9a130f05af.PNG)
![2b](https://user-images.githubusercontent.com/86158802/140626445-f14da2cb-9aba-47dd-935a-0a9fdbd2a8f9.PNG)

### Third Attempt: Changing the Activation function 
By changing the activation function of the output layer from "sigmoid" to "tanh", the accuracy of the model went even lower than the previous models upto 47%.

![3a](https://user-images.githubusercontent.com/86158802/140626452-fee906c3-94e3-4afc-83c4-70c0e563c952.PNG)
![3b](https://user-images.githubusercontent.com/86158802/140626459-f4cfbb8c-5976-49dd-93db-aab5e7092886.PNG)

## Summary
The neural network model ended up with 67% before optimization and 70% after optimization. The loss in accuracy for the attempts 2 and 3 can be traced from the fact that the model overfitted. Therefore, by optimizing our neural network with removal of more features or addition of some more data to the dataset might be able to increase accuracy. The Random Forest classifiers which have proven to be the most robust and accurate can also be used since the current accuracies were not at par with the standards.Furthermore, the random forest models deliver faster performance than neural networks and thus, the following model can also prevent the data from overfitting.
