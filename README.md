# Employee-Churn-Prediction
This is a project to predict the Employee Churn from a Employee Dataset
# Dataset
The datset is taken from datacamp. It describes the employee data with the various attributes of every employee.
# Preprocessing
In the collected dataset there were two shhets. One containing the details of the employees who left the company and the other containing who were stil working for the company. First the two sheets were merged with a new column left setting the value 1 for the ones who left and 0 for ones who were still serving the compmay. The merged dataset contained no entries with null values, so none of the rows or columns have been dropped. Next all categorical data is converted to numerical values using Lebel Encoding. After the preprocessing is over the preprocessed data is sacved as a csv file. This is done in the proprocess.ipynb file.
# Visualization
All the necessary datas are visualized using matplotlib and seaborn library functions. The correlation heatmap is generated to visualize which of the factors among the given attribute are affecting the target value how much. Next all the statistics of the employees who have left the company are visualized. This is done in the visualization.ipynb file.
# Training and Testing
The dataset is first split into training and testing data. 80% of the data is used for testing purpose and the rest 20% is kept for testing. For training the keras library is used to train the deep learning predicting model. The network consists of 7 fully connected layer. All having relu activation function except the output layer which has sigmoid as activation function. The model is trained for 1000 epochs with 'Adam' optimizer and 'binary_crossentropy' as loss function. Upon Testing on the rest 20% data it is found that the model is giving almost 99% accuracy. These are done in model_train_test.ipynb file.
# Scope
For future the plan is to built a front end for this so that it can used for industry purpose using django or flask.
