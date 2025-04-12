Used Google Colab to complete the following steps, which are divided into four parts:
* Prepared the data for use on a neural network model.
* Compiled and evaluate a model using a neural network.
* Predicted loan repayment success by using your neural network model.
* Discussed creating a recommendation system for student loans.

**Part 1: Prepare the data for use on a neural network model**

Using your knowledge of Pandas and scikit-learn’s *StandardScaler()*, preprocess the dataset so that you can use it to compile and evaluate the neural network model later. Completed the following data preparation steps:
1. Read the data from https://static.bc-edx.com/ai/ail-v-1-0/m18/lms/datasets/student-loans.csv into a Pandas DataFrame. Review the DataFrame, looking for columns that could eventually define your features and target variables.
2. Created the features *(X)* and target *(y)* datasets. The target dataset should be defined by the “credit_ranking” column. The remaining columns should define the features dataset.
3. Split the features and target sets into training and testing datasets.
4. Use scikit-learn's *StandardScaler* to scale the features data.

**Part 2: Compile and Evaluate a Model Using a Neural Network**

Used knowledge of TensorFlow to design a deep neural network model. This model used the dataset’s features to predict the credit quality of a student based on the features in the dataset. Consider the number of inputs before determining the number of layers that your model will contain or the number of neurons on each layer. Then, compile and fit your model. Finally, evaluate the model to calculate its loss and accuracy.
Completed the following steps:
1. Created a deep neural network by assigning the number of input features, the number of layers, and the number of neurons on each layer using TensorFlow’s Keras.
2. Compiled and fit the model using the *binary_crossentropy* loss function, the *adam* optimizer, and the *accuracy* evaluation metric.
3. Evaluated the model using the test data to determine the model’s loss and accuracy.
4. Saved and exported your model to a keras file, and name the file *student_loans.keras*.

**Part 3: Predict loan repayment success by using your neural network model**

Use the model you saved in the previous section to make predictions on your reserved testing data.
Completed the following steps:
1. Reloaded saved model.
2. Made predictions on the testing data, saving them to a DataFrame and rounding the predictions to binary values.
3. Generated a classification report with the predictions and testing data.

**Part 4: Discuss creating a recommendation system for student loans**

Briefly answered the following questions in the space provided:
1. Describe the data that you would need to collect to build a recommendation system to recommend student loan options for students. Explain why this data would be relevant and appropriate.
2. Based on the data you chose to use in this recommendation system, would the model be using collaborative filtering, content-based filtering, or context-based filtering? Justify why the data you selected would be suitable for your choice of filtering method.
3. Described two real-world challenges that you would take into consideration while building a recommendation system for student loans. Explain why these challenges would be of concern for a student loan recommendation system.
