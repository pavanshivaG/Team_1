CSV Column Classification and Normalization
Overview
This project focuses on a system that automatically classifies columns in a raw CSV file into predefined semantic categories. The goal is to preprocess and normalize the data to produce a structured CSV output. The system utilizes a machine learning model for classification and applies specific parsing rules to normalize key data types like phone numbers and company names.

Participants
This project was a collaborative effort by the following individuals:

Diya Waryani - Registration Number: 22BCB0105

Pavan Shiva - Registration Number: 22BCE3217

Arushi Parakh - Registration Number: 22BDS0176

System Architecture
1. Approach
The system's goal is to classify dataset columns into semantic categories: Phone Number, Company Name, Country, Date, and Other. This is achieved using a Logistic Regression (ML model) trained on labeled data with engineered features. Parsing and normalization rules are then applied to the output.

2. Workflow
Input: A raw CSV file with unknown columns.

Preprocessing & Feature Engineering: Features such as text length, digit count, letter count, special characters, and dictionary lookups are extracted from the data.

Model Prediction: The trained Logistic Regression model predicts the semantic type for each column.

Parsing & Normalization:

Phone Number: Split into Country and Number.

Company Name: Split into Name and Legal Entity.

Output: A processed CSV with structured fields.

3. Model Design
Model Used: Logistic Regression (Scikit-learn)

Training Data: phone.csv, company.csv, countries.txt, dates.csv

Output Classes: [Phone Number, Company Name, Country, Date, Other]

Performance: ~93% accuracy on a validation set.

Getting Started
To get a local copy up and running, follow these simple steps.

Prerequisites
Python 3.x

Scikit-learn

Pandas



License
Distributed under the [e.g., MIT License]. See LICENSE for more information.
