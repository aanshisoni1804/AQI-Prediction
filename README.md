# AQI Prediction Using Machine Learning and Deep Learning

This project aims to predict the Air Quality Index (AQI) using various machine learning and deep learning models. It combines pollution-related features from multiple government-provided datasets and evaluates the performance of different regression models including CNN, XGBoost, and MLP.

## Models Used and Performance

| Model                   | Mean Absolute Error (MAE) | Root Mean Squared Error (RMSE) | R² Score |
|------------------------|---------------------------|----------------------------------|----------|
| 1D CNN (Convolutional Neural Network) | 45.38                        | 82.59                            | 0.68     |
| XGBoost Regressor      | 43.82                        | 75.53                            | 0.73     |
| MLP (Multi-Layer Perceptron) | 46.87                        | 81.82                            | 0.69     |

- **1D CNN**: Designed to capture spatial-temporal relationships by reshaping input features into a 3D format.
- **XGBoost**: GPU-accelerated tree-based ensemble method, showing the best performance in this project.
- **MLP**: Fully connected feedforward network used for basic regression.

## Dataset

The data was combined from the following four CSV files:

- `city_day.csv`
- `city_hour.csv`
- `station_day.csv`
- `station_hour.csv`

Each file includes pollution-related features such as PM2.5, PM10, NO, NO₂, NOx, NH₃, CO, SO₂, O₃, Benzene, Toluene, and Xylene. AQI is the target variable.

Due to file size limitations, the dataset is not included in this repository. You can [download the dataset here](https://www.kaggle.com/datasets/rohanrao/air-quality-data-in-india) and place the files under `AQIdataset/AQI_Prediction_Dataset/`.



