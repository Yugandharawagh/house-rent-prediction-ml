# house-rent-prediction-ml
Machine Learning model to predict house rent using RandomForest with full preprocessing pipeline and model deployment.

🏠 House Rent Prediction using Random Forest

This project predicts house rent based on features like BHK, Location, Area (sqft), Tenant Type, Furnishing, Floor, and more.
It uses:
1)RandomForestRegressor
2)ColumnTransformer + Pipeline
3)OneHotEncoding
4)Train-Test Split
5)Model Evaluation (R2 Score & MAE)
6)Model Deployment (saved with joblib)

📌 Dataset Example
| ListingID | Locality | BHK | Area_sqft | Furnishing     | Floor | Age_Years | Availability | Tenant_Type | Parking | Lift | Balconies | Bathrooms | Rent_INR |
| --------- | -------- | --- | --------- | -------------- | ----- | --------- | ------------ | ----------- | ------- | ---- | --------- | --------- | -------- |
| PN100000  | Hadapsar | 1   | 402       | Semi-Furnished | 8     | 19        | Immediate    | Bachelor    | 0       | 1    | 3         | 1         | 19200    |
| PN100001  | Baner    | 1   | 449       | Furnished      | 20    | 20        | Immediate    | Family      | 1       | 1    | 2         | 1         | 34800    |

⚙️ Model Building Steps

1)Data Cleaning
2)Encoding categorical features using OneHotEncoding
3)ColumnTransformer + Pipeline
4)Train-Test Split
5)RandomForestRegressor
6)Evaluation
7)R2 Score
8)MAE
9)Saving the model using joblib

📂 Installation
pip install -r requirements.txt

▶️ Training the model
python src/train_model.py

📌 Prediction Example (predict.py)
python src/predict.py
