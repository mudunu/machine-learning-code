Machine Learning Project: Cancer Severity Prediction using KNN & Decision Tree
In this project, I built a Machine Learning system to predict the severity level of cancer patients (Low, Medium, High) using their medical data.

Step 1 – Loading and cleaning the data
I loaded a real cancer patient dataset using Python and Pandas.

I removed extra spaces in column names and converted text columns into numeric codes so that machine learning models can understand the data.

Step 2 – Preparing features and labels
I separated the data into:

Features (X): patient information (medical attributes)

Target (y): cancer severity level (Low, Medium, High)

I then split the data into training and testing sets using a custom train‑test split function.

Step 3 – Building KNN from scratch
I created my own K‑Nearest Neighbors (KNN) classifier in Python, without using scikit‑learn.

For each new patient, the model:

Calculates the distance to all other patients

Finds the k nearest neighbors

Predicts the most common severity level among them.

Step 4 – Building a Decision Tree from scratch
I implemented a Decision Tree classifier manually using Python and NumPy.

I used Gini impurity to find the best feature and threshold to split the data at each node.

I built the tree recursively, creating left and right branches until a maximum depth or pure leaf node is reached.

Step 5 – Model evaluation
I tested both models (KNN and Decision Tree) on the test data.

I calculated accuracy for each model.

I built a confusion matrix function and a classification report (precision, recall, F1‑score, support) to understand how well each class (Low, Medium, High) was predicted.

Step 6 – Cross‑validation
I implemented k‑fold cross‑validation from scratch.

I split the data into 5 folds, trained on 4 folds, and tested on 1 fold, repeating this for all folds.

I calculated cross‑validation accuracy scores for both KNN and Decision Tree and computed the mean accuracy.

I plotted the accuracy per fold for both models using Matplotlib.

Step 7 – Visualizing confusion matrices
I created a custom function to plot confusion matrices for both models.

This helped me visually compare how KNN and Decision Tree performed on each severity level.

