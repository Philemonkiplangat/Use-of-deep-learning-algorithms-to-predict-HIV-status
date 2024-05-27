# Use-of-deep-learning-algorithms-to-predict-HIV-status
Use-Of-Deep-Learning-in-Predicting-HIV-Status-Of-a-Person.
#### Data Source:
I used the Population-based HIV Impact Assessment (PHIA) data that consists of cross-sectional household-based surveys designed to assess HIV-related key health indicators. ICAP, based at Columbia University in collaboration with the US Centers for Disease Control and Prevention (CDC) and the Ministries of Health.

In this project, only deep learning algorithms were used, trained, and evaluated.
The male data and female data were separated since different variables used in the training and testing were not the same for males and females.
The two algorithms used were ANN and RNN since the data was structured.
The steps involved include:
- Loading the data(Adult Data)
- Feature Engineering: The major step involved splitting the male and female data since the predictors were not the same.
- Visualization
- Training the deep learning algorithms
- Saving the models
- Evaluating the models' performance on the training and testing data.
- Selection of the best models for deployment.
### Visualization summary
According to the correlation matrix for both men and women, a person's age is strongly correlated with the number of socio-behavioral traits that can predict their HIV status or persuade them to get tested because of the high likelihood of turning out positive. The location of the person greatly impacted the prediction, since ethnic Luo and Kisumu were among the important features during the prediction for both males and females.
### Model Training
Two deep learning algorithms were used, RNN and ANN
for RNN the hyperparameters used were

##### Hyperparameters used(RNN):
- LSTM units: 50
- Optimizer: Adam
- Loss function: Binary cross entropy
- Batch size: 32
- Patience for early stopping: 5 epochs
##### Hyperparameters used(ANN):
- Number of epochs: 100
- Batch size: 32
- Optimizer: Adam
- Loss function: binary_crossentropy
- Early stopping patience: 10
There was the use of early stopping to prevent overfitting
### Summary
Out of the two deep learning algorithms, RNN and ANN, the ANN algorithm emerged as the best in both males and females. After the exploratory data analysis, findings provide a potential use of the ANN algorithm with socio-behavioral-driven data to substantially identify HIV predictors and predict individuals at high risk of infection for targeted screening. For the Male dataset, ANN was the best to use in predicting the HIV status with a training score of 97.34% and a testing score of 97.09%. For the female data, the ANN algorithm still emerged the best with a training score of 98% and a testing score of 96% 
