# Project
## Student Mental Health
1. The code first loads the dataset from a CSV file named 'Student Mental health.csv' into a pandas DataFrame. It drops rows with any missing values using dropna() function and renames the column 'Choose your gender' to 'gender'.
2. It creates various plots using matplotlib and seaborn to visualize different aspects of the dataset:
--> Histogram of age distribution.
--> Count plot showing the distribution of students in different study years, with hue based on gender.
--> Count plots showing the distribution of anxiety and depression by gender.
--> Count plot showing the distribution of anxiety by study year.
--> Count plot showing the distribution of panic attacks by CGPA.
3. It maps gender values to numerical values ('Male': 0, 'Female': 1) in a new 'Gender' column. Then it selects features ('Age', 'Gender') and target variable ('Do you have Depression?') for modeling. It also encodes the target variable to binary numerical values ('Yes': 1, 'No': 0) using map() function and astype(int) method.
4. Splits the dataset into training and testing sets using train_test_split() function.
--> Trains three different classifiers: Decision Tree, Logistic Regression, and Random Forest, using the training data.
   Makes predictions on the test set using each trained model.
--> Calculates evaluation metrics for each model: Accuracy, Precision, Recall, and F1-Score using functions from sklearn.metrics.
--> Prints the evaluation metrics for each model.
5. Provides an example usage to predict the likelihood of depression for an 18-year-old male using the trained Logistic Regression model.

## Mental illness prevalence 
This code performs K-means clustering on a dataset of mental illness prevalence rates. It first reads the data from a CSV file, selects relevant features, and preprocesses the data by scaling it. Then, it determines the optimal number of clusters using the elbow method and performs K-means clustering with four clusters. Finally, it adds cluster labels to the original dataset and prints the cluster centroids. The KMeans warning regarding the default value of n_init changing in future versions is also displayed.

## Mental Health
1.  It reads a CSV file named 'Mental Health Dataset.csv' into a pandas DataFrame. The dataset contains information about mental health, including various features and a target variable.
2.  It handles missing values by dropping rows with any missing values. Categorical variables are encoded using LabelEncoder. Unexpected string values in certain columns are identified and handled appropriately by mapping them to numerical values.
3.  The 'Days_Indoors' column is converted to numeric data type, with errors coerced to NaN. Rows with NaN values are dropped from both the feature matrix (X) and the target variable (y).
4.  The dataset is split into training and testing sets using a 80-20 split ratio. A Decision Tree Classifier model is trained on the training data.
5.  The trained model is evaluated on the test set, and the accuracy score and classification report (including precision, recall, F1-score, and support) are printed to assess the model's performance.
