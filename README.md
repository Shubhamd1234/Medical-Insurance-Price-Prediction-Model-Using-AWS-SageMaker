# **Medical Insurance Price Prediction Model Using AWS SageMaker**

## **Goal of the Model**

The primary objective of this project is to predict **medical insurance prices** based on customer data using AWS SageMaker. The project involves building, training, and deploying a machine learning model using SageMaker's built-in Linear Learner algorithm.

## **Source of Data**

The dataset used for training and testing was sourced from **Kaggle** and uploaded to **Amazon S3** for easy integration with SageMaker.

## **Work Flow**
1. **Basic Information of Data**: Checked the shape of the dataset, described the columns, verified data types, and performed initial data inspections.
2. **Data Preprocessing**: Cleaned the dataset by handling missing values, Duplicate values, Invalid values and more.
3. **Exploratory Data Analysis (EDA)**: Performed data exploration, feature analysis, and visualized important patterns in the data and correlaiton matrix.
4. **Environment Setup**: Set up the AWS SageMaker environment and configured IAM roles and S3 buckets for data storage.
5. **Data Preparation**: Uploaded the dataset to S3, split into training and test sets.
6. **Model Training**: Used SageMaker’s Linear Learner algorithm with hyperparameter tuning (epochs, batch size).
7. **Model Deployment**: Deployed the trained model to a SageMaker endpoint for real-time predictions.
8. **Model Testing**: Evaluated the model using test data and handled serialization/deserialization for predictions.
9. **Model Evaluation**: Assessed the model’s performance with relevant metrics.

## **Tools and Technologies Used**

- **AWS SageMaker**: For building, training, and deploying the model.
- **Amazon S3**: For storing datasets.
- **IAM Roles**: For managing permissions in AWS.
- **Python & Jupyter Notebook**: For coding and model building.
- **Boto3**: AWS SDK for Python to interact with the SageMaker API.

### **Key Steps in the Project**:

- **Environment Setup**: Connected SageMaker to necessary AWS resources like S3 for data storage and IAM roles for permissions.
- **Data Upload**: Uploaded the insurance data to S3 in CSV format.
- **Model Training**: Trained the model using SageMaker’s Linear Learner algorithm, optimizing key hyperparameters.
- **Model Deployment**: Deployed the model for real-time predictions on a SageMaker-hosted endpoint.
- **Prediction & Evaluation**: Tested the model using unseen data, validating prediction accuracy.

### **Feature Engineering**:

- Calculated key features like **age, BMI, smoking status, and number of dependents**.
- Handled missing data, outliers, and feature scaling to improve the model's accuracy.
- Applied one-hot encoding to categorical variables like **region** and **smoker status**.

## **Modeling and Algorithms**

The project leveraged the **Linear Learner** algorithm provided by SageMaker. After training and deployment, the model was tested using real-world insurance data.

### **Model Performance Considerations**

- **Non-Linear Data**: The features (age, BMI, etc.) exhibit non-linear relationships with the target (insurance price), making it challenging for the linear model to capture all patterns effectively.
- **Sensitivity to Outliers**: Linear regression is sensitive to outliers, and the dataset includes critical outliers that significantly impact prices. Removing them would reduce the model’s ability to predict real-world cases accurately.

### **Conclusion:**

The **AWS SageMaker** model for predicting medical insurance prices performed good. This project highlights the potential of **cloud-based machine learning** for efficient and scalable deployment in real-world applications.




    

