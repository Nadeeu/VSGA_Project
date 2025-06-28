## Project Overview
This project aims to predict weather types based on several features including temperature, humidity, wind speed, precipitation, cloud cover, atmospheric pressure, UV index, season, visibility, and location. The target variable is the weather type (e.g., Rainy, Cloudy, Sunny, Snowy). The project leverages machine learning techniques, specifically the Random Forest classifier, to build a predictive model.

## Dataset
The dataset used in this project is stored in `weather_data.csv` and contains the following variables:
- **Temperature (numeric)**: Temperature in degrees Celsius.
- **Humidity (numeric)**: Percentage of humidity, including outliers.
- **Wind Speed (numeric)**: Wind speed in kilometers per hour.
- **Precipitation (%) (numeric)**: Percentage of precipitation, including outliers.
- **Cloud Cover (categorical)**: Description of cloud cover.
- **Atmospheric Pressure (numeric)**: Pressure in hPa.
- **UV Index (numeric)**: Indicates the strength of ultraviolet radiation.
- **Season (categorical)**: Season when the data was recorded.
- **Visibility (km) (numeric)**: Visibility in kilometers.
- **Location (categorical)**: Type of location where the data was recorded.
- **Weather Type (categorical)**: Target variable indicating the type of weather.

## Exploratory Data Analysis (EDA)
The notebook includes an initial EDA to understand the dataset's characteristics:
- **Data Structure**: The dataset contains 13,200 entries with 11 columns.
- **Data Types**: A mix of numeric and categorical variables.
- **Target Distribution**: The weather types are evenly distributed (Rainy, Cloudy, Sunny, Snowy each with 3,300 entries).
- **Visualizations**: Histograms for numerical variables to understand their distributions.

## Preprocessing Steps
1. **Data Loading**: The dataset is loaded using pandas.
2. **Data Inspection**: Basic information about the dataset is displayed, including data types and missing values.
3. **Target Analysis**: The distribution of the target variable (`Weather Type`) is examined.
4. **Feature Engineering**: Further preprocessing steps (e.g., handling outliers, encoding categorical variables) are suggested but not fully implemented in the notebook.

## Model Building
- **Algorithm**: Random Forest Classifier is used due to its robustness and ability to handle mixed data types.
- **Train-Test Split**: The data is split into training and testing sets.
- **Model Evaluation**: The model's performance is evaluated using a classification report, which includes metrics like precision, recall, and F1-score.

## Usage
1. **Requirements**: Ensure you have the required libraries installed (NumPy, pandas, matplotlib, seaborn, scikit-learn).
2. **Data Preparation**: Place the `weather_data.csv` file in the same directory as the notebook.
3. **Execution**: Run the notebook cells sequentially to load the data, perform EDA, and train the model.

## Results
The model gets an accuracy of about ~97%, which indicates the model works well. for other metrics can be seen in the classification report
