# Analyzing Bias Towards Women in Banking Data

This project aims to detect potential bias towards women in banking data using a machine learning model. It follows a structured approach involving data preprocessing, sampling, prediction, grouping, and statistical analysis.

## Steps Involved

1. **Preprocessing**
   - Reads the banking data from a CSV file.
   - Sets 'CustomerID' as the index for efficient data manipulation.
   - Encodes categorical columns to numerical values for model compatibility.

2. **Sampling**
   - Randomly samples 10% of the records from the dataset.
   - Swaps genders (males to females and vice versa) in the sampled data to simulate gender-specific biases.

3. **Prediction**
   - Utilizes K-Nearest Neighbors (KNN) algorithm to predict the decision labels for the modified (swapped gender) data.
   - Decision labels indicate the outcome or decision made by the banking system for each customer.

4. **Grouping**
   - Groups all male and female customers from both the original and modified datasets.
   - This step facilitates comparative analysis between genders across different scenarios.

5. **T-test**
   - Conducts a two-sample t-test to compare the means of decision labels between males and females.
   - Evaluates whether there are statistically significant differences in decision outcomes, which could indicate potential bias towards males or females in the banking data.
