Vehicle Fraud Detection
Project Overview
This project aims to detect fraudulent vehicle insurance claims using machine learning techniques. The dataset includes various features related to vehicle insurance policies and claims, and the objective is to classify whether a given claim is fraudulent or not.

Dataset
The dataset contains the following columns:

Make: The make of the vehicle.
AccidentArea: The area where the accident occurred.
Sex: Gender of the policyholder.
Age: Age of the policyholder.
MaritalStatus: Marital status of the policyholder.
PolicyType: Type of the insurance policy.
VehiclePrice: Price range of the vehicle.
Deductible: Deductible amount of the policy.
DriverRating: Rating of the driver.
PastNumberOfClaims: Number of past claims by the policyholder.
AgeOfVehicle: Age of the vehicle.
PoliceReportFiled: Whether a police report was filed.
WitnessPresent: Whether a witness was present.
AgentType: Type of agent handling the policy.
NumberOfCars: Number of cars the policyholder has.
FraudFound_P: Target variable indicating whether fraud was found (1) or not (0).
Preprocessing
Data Cleaning: Removed irrelevant and redundant columns.
Handling Categorical Variables: Used one-hot encoding to convert categorical variables into numerical format.
Balancing the Dataset: Applied oversampling to address class imbalance.
Feature Scaling: Standardized numerical features.
Model
Random Forest Classifier (RFC)
Best Parameters: n_estimators = 100 (determined through Grid Search)
Usage
Setup Environment
Ensure you have the necessary Python libraries installed. You can install them using:


pip install pandas scikit-learn seaborn matplotlib joblib
Load the Data
Load the dataset using pandas:


import pandas as pd
df = pd.read_csv('/content/drive/MyDrive/6c0cb57b-beff-4721-92d3-e77eb4c26c3f-fraud_oracle.csv')
Preprocess the Data
Follow the preprocessing steps outlined in the code notebook.

Train and Evaluate Models
Use the provided code to train and evaluate the model.

Save and Load Models
Models and preprocessing pipelines can be saved using joblib:


import joblib
joblib.dump(model, 'model_filename.joblib')
Files
data_preprocessing.ipynb: Jupyter notebook for data preprocessing.
model_training.ipynb: Jupyter notebook for training and evaluating models.
preprocessor.joblib: Saved preprocessing pipeline.
model.joblib: Saved trained model.
Contributing
Contributions are welcome! Please fork the repository and submit a pull request.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Clone the Repository
To get a local copy of the repository, you can clone it using git:

git clone https://github.com/namyaagrawal03/TheHackateers-HumanAIze.git
