# FraudGuardian - Financial Analysis and Fraud Detection AI

FraudGuardian is an AI-based financial analysis and fraud detection system designed to assess the financial need of students applying for financial aid, specifically tailored for NSFAS data and university information. The system utilizes machine learning techniques, including a neural network classifier, to predict financial need based on various features. Additionally, it incorporates simulated SMS confirmation security techniques.

## Table of Contents

- [Overview](#overview)
- [Data](#data)
- [How to Use](#how-to-use)
- [Code Structure](#code-structure)
- [Results](#results)
- [Model Details](#model-details)
- [Note](#note)

## Overview

FraudGuardian addresses the challenge of identifying potential fraudulent activities within financial aid applications. It merges NSFAS data and University of Limpopo data, performs data preprocessing, feature engineering, and applies a neural network classifier for prediction. The model's performance is evaluated using metrics such as accuracy, precision, recall, and F1 score. Additionally, the system incorporates simulated SMS confirmation security techniques to enhance application verification.

## Data

### NSFAS Data

The NSFAS data includes the following columns:

- ID Number
- First Name
- Last Name
- Gender
- Date of Birth
- Email
- Phone Number
- Application Date
- Course
- Institution
- Financial Need

### University Data

The University of Limpopo data includes:

- Student ID
- First Name
- Last Name
- Gender
- Date of Birth
- Email
- Phone Number
- Course
- Course Year

## How to Use

### Prerequisites

- Python 3.x
- Libraries: pandas, scikit-learn, imbalanced-learn, keras

### Installation

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/your-username/FraudGuardian.git
   ```

2. Install the required Python libraries:

   ```bash
   pip install pandas scikit-learn imbalanced-learn keras
   ```

### Data Preparation

1. Replace the placeholder paths in the code with the actual paths to the `nsfas_data.csv` and `university_data.csv` files.

2. Ensure the necessary data files are available and correctly formatted.

### Running the Code

Execute the `FraudGuardian.py` script:

```bash
python FraudGuardian.py
```

### Results

After running the script, the model will be trained, and its performance will be evaluated using metrics such as accuracy, precision, recall, and F1 score. Additionally, a confirmation code will be generated and a simulated SMS will be sent for confirmation security.

## Code Structure

- `FraudGuardian.py`: Main script containing the entire workflow, including data loading, preprocessing, feature engineering, model training, evaluation, and SMS confirmation simulation.

## Model Details

The machine learning model selected for this application is a neural network implemented using the Keras library. The architecture includes an input layer with 64 neurons, a hidden layer with 32 neurons, and a single neuron output layer for binary classification. The model is trained using the Adam optimizer and binary crossentropy loss.

## Note

- The script currently uses simulated data and a random oversampling technique to address class imbalance. Adjustments may be needed for a real-world scenario.
- Ensure proper handling of sensitive information (e.g., actual phone numbers) and implement secure SMS confirmation techniques in a production environment.

Feel free to explore and modify the code to suit your specific use case or integrate it into a larger fraud detection system. If you encounter any issues or have suggestions for improvement, please open an issue on the repository. Happy coding!
