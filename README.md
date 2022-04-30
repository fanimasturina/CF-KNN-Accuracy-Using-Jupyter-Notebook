# CF-KNN-Accuracy-Using-Jupyter-Notebook
On my thesis project, i created an expert system that calculates the result of dental diagnoses using Certainty Factor and K - Nearest Neighbor. This is the calculation of accuracy of the methods, i'm using python 3 (ipykernel) and Jupyter Notebook as a framework to calculate the accuracy. 

What needed:
100 data of dental patiens (preprocessing data) which contains patient identity (1 data - name), CF value for each patient symptoms (28 data), diagnosis results. This generated over CSV file.

Steps to Reproduce:
1. Enter the required python libraries in Jupyter Notebook, such as pandas, numpy, matplotlib, sklearn.
2. Import the Dataset file and declare it.
3. Separate the symptoms and diagnosis into 2 distinct sections. Variable X is for dataset containing patient complaints, variable y is for doctor's diagnosis. 
4. Perform data normalization using min-max normalization. (The reason why i working on Min Max Norm;  If i choose to use standardization, then there is a possibility that the results given are in the form of a negative scale value. Min-max makes a range from 0-1, more appropriate for expert systems. Secondly, When compared to Z-score normalization, Min-max can guarantee all features will scale exactly the same even though it doesn't handle outliers as well as Z-Score. But this shouldn't be a problem because some of the data are more or less identical.)
5. Train – Test split, which is splitting the dataset into testing data and training data with a ratio of testing: training = 20:80.
6. Declare the KNN method and its neighbors.
7. Predict the results of KNN.
8. Evaluate the results of the training data and the results of data testing by creating a Confusion Matrix. The Confusion Matrix shows the amount of training data that is predicted correctly and incorrectly.

Expected Result:
Accuracy results from the combination of Certainty Factor and K Nearest Neighbor methods in the application of an expert system for diagnosing dental disease i created previously.
