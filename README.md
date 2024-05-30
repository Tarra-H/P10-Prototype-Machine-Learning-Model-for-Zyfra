# Developing a Machine Learning Prototype to Predict Gold Extraction Efficiency for Zyfra

Project Description:

Prepare a prototype machine learning model for Zyfra. The company specializes in developing efficient solutions for heavy industries. The model we create should predict the amount of gold extracted or obtained from gold ore. There is data available related to the extraction and refining processes of gold ore that you can use. Ultimately, this model is expected to contribute to the creation of a more efficient production process and eliminate parameters that do not yield profits.

Tasks to be done:
Prepare the available data
Conduct data analysis
Develop and train the model
To complete this project, you may need to refer to the documentation of the Pandas, Matplotlib, and Sklearn libraries.

The data you need is stored in three files:
gold_recovery_train.csv — download training dataset
gold_recovery_test.csv — download test dataset
gold_recovery_full.csv — download source dataset
Some parameters are not available because measurements and/or calculations were made long afterward. That's why some features present in the training set may not be in the test set. The test set also does not contain the target.

The source dataset contains both the training and test sets with all their features.
The data we have is raw data just downloaded from the data warehouse. Before creating the model, it is advisable to check the accuracy of the data.


Objective:
Create a prototype machine learning model for Zyfra.


Project Work Steps:
Prepare the data

1.1. Open the files and study the data.
 File path:
 - /datasets/gold_recovery_train.csv
 - /datasets/gold_recovery_test.csv
 - /datasets/gold_recovery_full.csv
1.2. Check if the gold recovery has been calculated correctly. Using the training set, calculate the recovery for the rougher.output.recovery feature. Find the MAE between your calculation and the feature value. Show what you find.

1.3. Analyze the features not available in the test set. What are these parameters? What types are these parameters?

1.4. Perform data preprocessing.

Analyze the data

2.1. Make notes on how the metal concentrations (Au, Ag, Pb) change depending on the purification stage.

2.2. Compare the distribution of feed particle sizes in the training set and test set. If the distribution varies significantly, the model evaluation will be incorrect.

2.3. Consider the total concentration of all substances at different stages: raw feed, rougher concentrate, and final concentrate. Do you see any abnormal values in the total distribution? If yes, do you need to remove these values from both samples? Explain what you find and remove the anomalies.

Build the model

3.1. Create a function used to calculate the final sMAPE value.

3.2. Train on different models. Evaluate these models using cross-validation. Select the best model and test it using the test sample. Show what you find.

Use the sMAPE formula and final sMAPE for evaluation metrics.
