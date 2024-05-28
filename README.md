# Daily Weather Data Analysis Using Decision Tree Classification

This project analyzes daily weather data to classify high-humidity days using a decision tree classifier implemented with scikit-learn.

## Project Description

This project utilizes a decision tree algorithm to predict whether a day will have high humidity based on morning weather sensor readings. The data is from a weather station and includes measurements like air pressure, temperature, wind speed, and rain accumulation.

## Data

The data for this project is stored in a CSV file named `data/data_weather.csv`. This file contains weather data collected over a three-year period.

##  Steps

1. **Import Libraries:** Necessary libraries like pandas and scikit-learn are imported for data manipulation and machine learning tasks.
2. **Load Data:** The `data_weather.csv` file is loaded into a pandas DataFrame.
3. **Data Exploration:** The DataFrame is analyzed to understand its structure, columns, and potential missing values.
4. **Data Cleaning:** 
    - The `'number'` column, which is not required for analysis, is removed.
    - Missing values are handled using the pandas `dropna` function.
5. **Classification Task:**
    - The relative humidity at 3 pm is converted into a binary classification label (high humidity or not) based on a threshold.
6. **Feature Selection:** Morning sensor readings (9 am) are chosen as features to predict afternoon (3 pm) humidity.
7. **Train-Test Split:** The data is split into training and testing sets using `train_test_split` from scikit-learn.
8. **Model Training:** A decision tree classifier is trained on the training data using `DecisionTreeClassifier` from scikit-learn.
9. **Prediction:** The trained model is used to predict humidity labels for the testing data.
10. **Evaluation:** The accuracy of the model is evaluated using `accuracy_score` from scikit-learn.

## Running the Project

1. Ensure you have Python and the required libraries (pandas, scikit-learn) installed.
2. Clone or download this repository.
3. Navigate to the project directory in your terminal.
4. Run the script using `python DAILY WEATHER DATA ANALYSIS USING DECISION TREE CLASSIFICATION.ipynb`.

## Additional Notes

* This is a basic example of using a decision tree for weather classification. 
* More advanced techniques and feature engineering could be explored for better performance.

## Future Improvements

* Implement hyperparameter tuning to optimize the decision tree model.
* Explore other classification algorithms for comparison.
* Visualize the decision tree to understand its decision-making process.

I hope this README provides a clear and informative overview of the project!
