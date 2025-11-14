# Colorado Motor Vehicle Sales Analysis & Prediction

## Project Description 📊

This project analyzes historical motor vehicle sales data from various counties in Colorado (sourced from `colorado_motor_vehicle_sales.csv`). It performs Exploratory Data Analysis (EDA) to uncover trends over time and across different counties. Finally, it builds a predictive model using Ridge Regression to forecast sales based on year, quarter, and county.

## Key Steps ⚙️

1.  **Import Libraries:** Essential Python libraries like pandas, numpy, matplotlib, seaborn, scikit-learn, and plotly are imported.
2.  **Load Data:** The `colorado_motor_vehicle_sales.csv` dataset is loaded into a pandas DataFrame.
3.  **Data Preprocessing:**
    * Checked for and handled missing values (though none were found in this dataset).
    * Created a combined `period` column (e.g., "2008 Q1") for easier time-series analysis.
    * Sorted the data by year and quarter.
4.  **Exploratory Data Analysis (EDA):**
    * Visualized total sales trends over time using a line plot (aggregated quarterly). 
    * Displayed sales distribution by county using a bar plot for the top 15 counties. 
    * Created an interactive Plotly line plot to compare sales trends for the top 5 counties over time.
5.  **Predictive Modeling:**
    * Prepared data for modeling using one-hot encoding for the `county` feature and standard scaling for numerical features (`year`, `quarter`).
    * Split the data into training and testing sets.
    * Trained a **Ridge Regression** model to predict `sales`.
6.  **Model Evaluation:**
    * Evaluated the Ridge Regression model using standard metrics: Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R-squared (R2).
    * Visualized the model's performance by plotting actual vs. predicted sales using a regression plot. 

## Technologies Used 🛠️

* Python 3
* pandas
* numpy
* matplotlib
* seaborn
* plotly
* scikit-learn

## How to Run 🚀

1.  Ensure you have Python and the required libraries installed (`pip install pandas numpy matplotlib seaborn plotly scikit-learn`).
2.  Download the `Colorado_Motor_Vehicle_Sales_Data.ipynb` notebook and the `colorado_motor_vehicle_sales.csv` file.
3.  Place the CSV file in the expected path (e.g., `/content/` if using Google Colab, or adjust the path in the notebook).
4.  Open and run the Jupyter Notebook.

## Findings 📈

The EDA revealed distinct quarterly sales patterns and significant variations in sales volumes across different counties. The Ridge Regression model achieved an R-squared score of approximately **0.93** on the test set, indicating a good fit for predicting sales based on the selected features.

Made By: Pranav Ghadge
