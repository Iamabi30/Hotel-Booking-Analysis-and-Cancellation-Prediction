# Hotel Booking Analysis and Cancellation Prediction

## Overview
This project analyzes a hotel booking dataset to uncover trends and patterns in booking demand and cancellations. Leveraging data preprocessing, exploratory data analysis (EDA), and machine learning, we aim to predict whether a booking will be canceled based on various customer, booking, and hotel-related features.

## Dataset
**Dataset Name**: Hotel Booking Demand Dataset  
**Source**: [Kaggle](/kaggle/input/hotel-booking-csv)  

### Dataset Description
The dataset contains booking information for a city hotel and a resort hotel, including details such as:
- Customer demographics
- Booking preferences
- Stay duration
- Hotel type
- Special requests

### Key Features:
- **Hotel**: Type of hotel (Resort Hotel or City Hotel)
- **Is Canceled**: Whether the booking was canceled (target variable)
- **Lead Time**: Number of days between booking and arrival
- **ADR (Average Daily Rate)**: Average price per day
- **Special Requests**: Number of special requests made

## Project Workflow
### 1. Data Preprocessing
- Handled missing values using context-appropriate strategies (e.g., mean imputation for numerical columns, mode for categorical columns).
- Encoded categorical variables using Label Encoding and One-Hot Encoding.
- Scaled numerical features using StandardScaler to normalize data.

### 2. Exploratory Data Analysis (EDA)
- Identified key booking patterns and trends using visualizations (e.g., cancellation rates, seasonal trends, and customer types).
- Detected and treated outliers in critical features like ADR.

### 3. Feature Engineering
- Derived additional features, such as "Length of Stay" and "Booking to Arrival Gap."
- Performed feature selection to retain the most impactful variables.

### 4. Model Building and Evaluation
Built and evaluated multiple machine learning models, including:
- KNN
- Logistic Regression
- DecisionTreeClassifier
- RandomForestClassifier
- CatBoost

Achieved an **accuracy score of 99.5%**, demonstrating the high performance of the chosen model.

## Key Results
- **High Accuracy**: The model accurately predicts cancellations with 99.5% accuracy.
- **Insights**: Customers with longer lead times and fewer special requests are more likely to cancel.

## Visualizations
Key insights were visualized using:
- **Heatmaps**: Correlation between features.
- **Line Charts**: Booking trends over time.
- **Bar Plots**: Distribution of cancellations by hotel type.

## How to Use
### Prerequisites
Ensure you have Python 3.8+ installed along with the required libraries. Install dependencies using:
```bash
pip install -r requirements.txt
```

### Run the Project
1. Clone this repository:
   ```bash
   git clone https://github.com/iamabi30/Hotel-Booking-Analysis.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Hotel-Booking-Analysis
   ```
3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook notebooks/Hotel_Booking_Analysis.ipynb
   ```

## Dependencies
The project uses the following Python libraries:
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- catboost

Install them using:
```bash
pip install -r requirements.txt
```
## Contributions
Contributions are welcome! Feel free to fork the repository, create a branch, and submit a pull request.

