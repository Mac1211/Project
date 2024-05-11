# Project
## Mental illness prevalence 
This code performs K-means clustering on a dataset of mental illness prevalence rates. It first reads the data from a CSV file, selects relevant features, and preprocesses the data by scaling it. Then, it determines the optimal number of clusters using the elbow method and performs K-means clustering with four clusters. Finally, it adds cluster labels to the original dataset and prints the cluster centroids. The KMeans warning regarding the default value of n_init changing in future versions is also displayed.
## Mental Health
1.  It reads a CSV file named 'Mental Health Dataset.csv' into a pandas DataFrame. The dataset contains information about mental health, including various features and a target variable.
2.  It handles missing values by dropping rows with any missing values. Categorical variables are encoded using LabelEncoder. Unexpected string values in certain columns are identified and handled appropriately by mapping them to numerical values.
3.  The 'Days_Indoors' column is converted to numeric data type, with errors coerced to NaN. Rows with NaN values are dropped from both the feature matrix (X) and the target variable (y).
4.  The dataset is split into training and testing sets using a 80-20 split ratio. A Decision Tree Classifier model is trained on the training data.
5.  The trained model is evaluated on the test set, and the accuracy score and classification report (including precision, recall, F1-score, and support) are printed to assess the model's performance.
