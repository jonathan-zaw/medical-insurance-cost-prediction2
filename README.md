# medical-insurance-cost-prediction2
This project predicts medical insurance costs using a linear regression model. The dataset used contains demographic information such as age, sex, BMI, number of children, smoking status, and region. The target variable is the charges column, which represents medical costs. The model applies log transformation to improve prediction accuracy.


Dataset

The dataset contains the following columns:
	•	Age: Age of the individual
	•	Sex: Gender (encoded as 0 for male, 1 for female)
	•	BMI: Body Mass Index
	•	Children: Number of children covered by health insurance
	•	Smoker: Smoking status (encoded as 0 for yes, 1 for no)
	•	Region: Geographic region (encoded as categorical values)
	•	Charges: Medical insurance costs (log-transformed for better model performance)

Data Preprocessing
	1.	Encoding categorical variables (sex, smoker, region).
	2.	Applying log transformation to the charges column to normalize the distribution.
	3.	Splitting the dataset into training and testing sets using an 80-20 split.

Model Training
	•	The model used is Linear Regression from sklearn.
	•	Features are selected by dropping the charges column.
	•	The model is trained on X_train and Y_train.

Model Evaluation
	•	Predictions are made on both training and test data.
	•	R-squared (R²) values are computed to measure model accuracy.
	•	A predictive system is implemented to estimate insurance costs for new input values.

