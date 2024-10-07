# Credit-Risk-Classification
The code starts by importing necessary libraries, including pandas for data manipulation, numpy for numerical operations, and matplotlib for plotting. It also includes modules from scikit-learn for machine learning tasks. The dataset, containing customer data, is read from a CSV file, and an initial preview of the data is shown. Afterward, the 'id' column is dropped, and the features and target variables are separated into X (features) and y (labels).

The dataset is split into training and testing sets using a 70-30 split ratio. Missing values in the training data are handled by imputing the mean values using the SimpleImputer class. Both the training and testing sets are then standardized with StandardScaler to ensure the features are on the same scale.

The K-Nearest Neighbors (KNN) algorithm is applied to classify the credit risk, with 5 neighbors selected as the hyperparameter. The model is trained on the training set, and K-Fold and Stratified K-Fold cross-validation are used to estimate the accuracy of the model, which averages around 75%.

Predictions are made on the training set, and probabilities for each class are computed. A comparison is created between the actual and predicted values, along with the prediction probabilities. The model’s performance is evaluated using confusion matrices and classification metrics, such as precision, recall, and F1-score, showing an accuracy of 81% on the training data.

The code then iteratively checks how the model's accuracy changes for different values of k, plotting the results. Finally, the trained model and the scaler are saved using the pickle library for future use.






