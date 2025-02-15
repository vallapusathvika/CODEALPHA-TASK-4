# CODEALPHA-TASK-4
### SALES PREDICTION USING PYTHON ###
This code snippet demonstrates a simple linear regression analysis performed in a Jupyter Notebook. It uses libraries like pandas, numpy, matplotlib, and scikit-learn to analyze and predict sales based on marketing budgets (TV, Radio, and Newspaper). Here's an explanation of each step:

1. **Imports:**
   - The code imports several libraries: pandas for data manipulation, numpy for numerical operations, matplotlib for visualization, and scikit-learn for machine learning tasks. These libraries are essential for reading data, training the model, evaluating performance, and visualizing results.

2. **Loading the Dataset:**
   - The dataset is loaded using pandas' `read_csv()` function, which reads a CSV file containing sales data. This data is assumed to include columns for TV, Radio, Newspaper marketing expenditures, and the corresponding sales data.

3. **Exploring the Dataset:**
   - The first few rows of the dataset are printed to give an overview of its structure. This helps ensure that the data is loaded correctly and provides insights into its contents.
   - Missing values are checked using the `isnull().sum()` function, which returns the count of missing values in each column. Handling missing data is a crucial step in preparing the data for analysis.

4. **Preparing Data:**
   - The independent variables (features) for the model are selected as the columns `TV`, `Radio`, and `Newspaper`, while the dependent variable (target) is `Sales`. These features will be used to predict sales.

5. **Splitting Data:**
   - The dataset is split into training and testing sets using `train_test_split()`. 80% of the data is used for training the model, and the remaining 20% is used for testing its performance. This ensures that the model can generalize well to unseen data.

6. **Training the Model:**
   - A linear regression model is created and trained using the training data (`X_train`, `y_train`). The model learns the relationship between marketing expenditures and sales during this step.

7. **Making Predictions:**
   - Once trained, the model makes predictions on the test set (`X_test`). These predictions are compared to the actual sales (`y_test`) to evaluate the model's performance.

8. **Model Evaluation:**
   - The performance of the model is evaluated using three metrics:
     - **Mean Absolute Error (MAE)**: This measures the average of the absolute differences between predicted and actual values.
     - **Mean Squared Error (MSE)**: This calculates the average of the squared differences between the predicted and actual values.
     - **R-squared (R²)**: This indicates how well the independent variables explain the variation in the dependent variable.
   - These metrics give an idea of how accurately the model is predicting sales.

9. **Visualizing Results:**
   - A scatter plot is created to visualize the relationship between the actual and predicted sales. Ideally, the points on this plot should align closely with the 45-degree line, indicating that the predictions are close to the actual values.

10. **Making Predictions for New Data:**
    - The model is also used to predict sales for new input values (TV=100, Radio=50, Newspaper=30). This demonstrates how the model can be applied to new, unseen data.

In summary, this code demonstrates how to train a linear regression model to predict sales based on marketing expenditures. It involves loading and exploring the data, preparing it for training, evaluating the model’s performance, visualizing the results, and making predictions for new data. This process is commonly used for predictive analytics in business contexts, and Jupyter Notebooks are ideal for such tasks due to their interactive nature and ability to combine code, visualizations, and explanations in one document.
