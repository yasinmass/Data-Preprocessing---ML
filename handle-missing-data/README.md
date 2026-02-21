📊Retail Data Analysis – Handling Missing Values & Clustering
📌 Project Overview

This project shows how to:

Find missing values in a dataset

Handle missing values using different methods

Predict missing values using Machine Learning

Apply clustering to group similar products

The dataset contains retail product information such as Category, Price, Rating, Stock, and Discount.

📂 Dataset Columns

Category – Product category (A, B, C, D)

Price – Product price

Rating – Customer rating (1 to 5)

Stock – In Stock / Out of Stock

Discount – Discount percentage

Some values are missing, and we handle them using different techniques.

🔎 Step 1: Analyze Missing Data

We checked:

Total missing values

Percentage of missing values

Duplicate records

Basic statistics

This helps us understand the dataset before cleaning it.

🧹 Step 2: Handle Missing Values (Statistical Methods)

Different methods were used based on column type:

🔹 Categorical Columns

Category → Filled using Mode

Stock → Filled using Mode

(Mode = Most frequent value)

🔹 Numerical Columns

Discount → Filled using Mean

Rating → Filled using Mean

Price → Filled using Median

(Median is used for Price because it may be skewed.)

🤖 Step 3: Predict Missing Values Using Machine Learning

Instead of using mean, we can also predict missing values.

We used:

RandomForestRegressor

Steps:

Convert categorical columns into numbers using LabelEncoder

Separate rows with known and unknown Rating

Train the model using known data

Predict missing Rating values

This method is more intelligent than simply using mean.

📊 Step 4: Apply KMeans Clustering (Unsupervised Learning)

After cleaning the data, we applied:

KMeans Clustering

Used features:

Price

Rating

Discount

Before applying KMeans, we scaled the data using StandardScaler (important for distance-based algorithms).

The clustering groups similar products together.

📈 Result

The clustering mainly grouped products based on Rating levels.

This shows that Rating has stronger natural grouping compared to Price.

🛠 Tools Used

Python

Pandas

NumPy

Matplotlib

Scikit-learn

🎯 What I Learned

How to analyze missing values

When to use mean, median, or mode

How to use RandomForest for prediction

Importance of scaling before clustering

How to interpret clustering results

🚀 Conclusion

This project demonstrates basic data cleaning, machine learning, and clustering techniques in a simple and practical way.

It is a beginner-friendly end-to-end ML preprocessing workflow.