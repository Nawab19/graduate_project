# Multi-Tasking Active Learning
This repository contains the final graduate project of my Master's degree from University of Ottawa

Dataset: IMDB movie metadata

Preprocessings:
- Deleting a few features due to high correlation
- Delete rows with missing values
- Convert Target variables into smaller number of classes
- Standardize the dataset

Split:
 - 1000 Training Instances
 - 2000 Pool Instances (For query)
 - 738 Testing Instances

General Methodology:
- Step 1: Train with 1000 instances
- Step 2: Test the model with 738 testing instances
- Step 3: Generate probability array for all instances in pool
- Step 4: For each target, select 15 instances with minimum confidence
- Step 5: Obtain labels for these 45 queries and add to training set
- Repeat steps 1 to 5 until 900 instances are added from pool

FILE DETAILS:
Active_Learning_With_Minimum_Probabilities_DT
- Multi-Tasking active learning with Decision Tree classifier and minimum confidence query sampling strategy

Active_Learning_With_Minimum_Probabilities_RF
- Multi-Tasking active learning with Random Forest classifier and minimum confidence query sampling strategy

Active_Learning_With_Minimum_Probabilities_KNN
- Multi-Tasking active learning with K-Nearest Neighbour classifier and minimum confidence query sampling strategy

Active_Learning_With_Minimum_Probabilities_SVM
- Multi-Tasking active learning with Supoort Vector Machine classifier and minimum confidence query sampling strategy

Active_Learning_With_Maximum_Probabilities_DT
- Multi-Tasking active learning with Decision Tree classifier and maximum confidence query sampling strategy

Active_Learning_With_MinAndMax_Probabilities_DT
- Multi-Tasking active learning with Decision Tree classifier and combination of minimum and maximum confidence query sampling strategy

Active_Learning_With_Minimum_Probabilities_and_Oversampled_Datasets_DT
- Multi-Tasking active learning with Decision Tree classifier and minimum confidence query sampling strategy using Oversampled Dataset

Active_Learning_With_Minimum_Probabilities_and_Undersampled_Datasets_DT
- Multi-Tasking active learning with Decision Tree classifier and minimum confidence query sampling strategy using Undersampled Dataset
