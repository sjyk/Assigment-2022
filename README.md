# Assigment-2022
Template for Assignment

# Set-Up
Follow the set-up guide: Setup.md before starting the assigment. We will be tracking the progress in your notebook

# Dataset
The task that you will complete is 

Predicting the correct destination of a vessel is a relevant problem for a wide range of stakeholders including port authorities, vessel operators and many more. The prediction problem is to generate a continuous stream of predictions for the destination port of any vessel given the following information: (1) unique ID of the ship, (2) actual position of the ship, (3) name of the port of departure, (4) time stamp, and (5) vessel’s draught. The above data is provided as a continuous stream of tuples and the goal of the system is to provide for every input tuple one output tuple containing the name of the destination port. A solution is considered correct at time stamp T if for a tuple with this timestamp as well as for all subsequent tuples the predicted destination port matches the actual destination port. The goal of any solution is not only to predict a correct destination port but also to predict it as soon as possible counting from the moment when a new port of origin appears for a given vessel. After port departure and until arrival, the solution must emit one prediction per position update.

Note that at each time stamp, for prediction, you have access to the data at that time stamp and the data of the same vessel at previous time stamps. Make sure to use that information in your prediction.

# Submission

You will be expected to complete a final model in the experimental section of the notebook. Given a test file (in the same format as the training file), when we run your notebook in order, we expect to output a prediction file with one destination value for each sample value. Like the training data, we can consider the test file as a stream of data where you have access to the data at that time stamp and the data of the same vessel at previous time stamps.
