# Elevatelabs-task2
📊 Diamond Price Analysis & Exploratory Data Analysis (EDA)

This project performs a detailed Exploratory Data Analysis (EDA) on the well-known Diamonds Dataset, with a strong focus on understanding how various diamond characteristics influence their price.

🎯 Project Goals

The primary objectives of this project are to:

Clean and preprocess the raw diamond dataset

Perform a comprehensive EDA using histograms and distribution plots

Understand relationships between diamond features such as carat, cut, color, clarity, and dimensions

Extract insights related to diamond pricing patterns

📁 Dataset Information

The dataset used is the Diamonds Dataset from the seaborn-data repository, containing nearly 54,000 diamonds with detailed attributes.

Dataset Features
Feature	Description
carat	Weight of the diamond (0.2 to 5.01)
cut	Quality of cut — Fair, Good, Very Good, Premium, Ideal
color	Color grade from J (worst) to D (best)
clarity	Clarity grade — I1 (worst), SI2, SI1, VS2, VS1, VVS2, VVS1, IF (best)
depth	Total depth percentage
table	Width of top of diamond relative to widest point
price	Price in USD (326 to 18,823)
x	Length (mm)
y	Width (mm)
z	Depth (mm)
🔧 Methodology

All analysis was performed in Google Colab using Python libraries such as Pandas, Seaborn, Matplotlib, and Scikit-learn.

1. Data Cleaning & Preprocessing

✔ Loaded dataset into a Pandas DataFrame
✔ Checked data structure, types, and missing values (info(), isnull())
✔ Removed diamonds with impossible dimensions (x = 0, y = 0, z = 0)
✔ Removed duplicate rows
✔ Performed One-Hot Encoding on categorical features (cut, color, clarity)
✔ Normalized numerical features using MinMaxScaler

2. Exploratory Data Analysis (EDA)

EDA focused primarily on histograms to visually understand frequency distributions.

📌 Techniques Used:

Summary statistics for numerical features

Value counts for categorical features

Histograms for:

Carat

Depth

Table

Price

Dimensions (x, y, z)

Price distribution by Cut

Carat distribution by Clarity

Overall price histogram

Grouped Means:

Average Price by Cut

Average Carat by Clarity

🔍 Key Insights

🔹 The dataset was already clean with no missing values, but further refined by removing invalid entries and duplicates
🔹 Price and Carat distributions are right-skewed, showing more low-priced and small diamonds
🔹 Different cut and clarity categories show distinct distribution behaviors
🔹 For example:

Ideal cuts show concentrated price ranges

I1 clarity diamonds often have higher average carat weights
🔹 Preprocessing (encoding + scaling) prepares the dataset for future machine learning models

▶️ How to Run

Open the diamond_eda.ipynb file in Google Colab

Run all cells sequentially

The dataset downloads automatically

EDA visualizations and preprocessing steps execute without additional setup

🧩 Dependencies

Make sure the following Python libraries are installed:

pandas
matplotlib
seaborn
scikit-learn
