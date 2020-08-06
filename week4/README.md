This week we worked with statistics, particularly with hypothesis testing.
Then we saw how PCA works in practice.
3rd day we started doing neural networks and CNN. We mostly worked with Churn dataset. The aim of this notebook was to apply and improve neural networks using keras library.
We experimented with over/under sampling methods because target class was imbalanced. We tried SMOTE, TomekLinks, and SMOTETomek and neural network with 10, 20, 30 epochs.
Adam and Rmsprop optimizers were also tested and we didn't see much difference between them and we decided to leave Adam optimizer as a default optimizer. 
The highest accuracy we achieved is 88% with 30 epochs and batch size 10.
Here is the NN model that we used to train and test:

model = Sequential()
model.add(Dense(16, activation = 'relu', input_shape=(9,)))
model.add(Dense(8, activation = 'relu'))
model.add(Dense(1, activation='sigmoid'))

In the end we tried different classification algorithms. Basic Decision Tree gave us 89% and XGBoost gave 91% the highest accuracy among all the algorithms.
You can see all the results in Churn.ipynb notebook.

Feel free to use any of the public data.
Good luck learning ML/DL.
