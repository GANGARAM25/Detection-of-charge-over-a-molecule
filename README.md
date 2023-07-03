# Detection-of-charge-over-a-molecule
We used the data from the ZINC dataset and ChEMBL dataset with epsilon values 4 and 78 respectively from both the datasets.

**Conclusion :**
APDs were first calculated for each molecule and the molecular descriptors obtained from APD
were used in prediction of the partial charges. We created 2 Models using Random Forest and
Neural Network methods to predict partial charges. Both the models were trained on the
dataset as mentioned above. We have better predictions through the neural network model as
compared to the random forest method. Improvements can be made on both the models by
increasing the size of the dataset to train the models better and both the models predict the
partial charges using different methodologies. So one better way to predict the charges is to
use both the models and predict the charges using Ensemble Learning Technique.
To predict the charges using the Random Forest model and Neural Network model we have
created a program which takes a sdf file as an input and predicts the charges. We also
calculated RMSE using the calculate_rmse() function which takes predicted charges and the
true charges as input.
We got better accuracy for every test set for the Random Forest where the number of trees =
100, maximum depth = 6, minimum number of samples to split = 6 and minimum number of
samples in leaves = 6.
We got better accuracy for every test set for the neural network in which the hyperparameters
were : Learning rate : 0.001 , Number of epochs = 100 , Batch size = 64 and number of nodes
as 80 in the first and hidden layers
