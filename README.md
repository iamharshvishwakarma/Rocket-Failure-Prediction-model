# Rocket Failure Prediction Models

This repository contains two machine learning models for predicting rocket launch failures:

- **Weather-Based Model:** Predicts rocket failure based on weather conditions (temperature, wind speed, and humidity).
- **Thrust-to-Weight Ratio Model:** Predicts rocket failure based on the Thrust-to-Weight Ratio, calculated using Liftoff Thrust and Payload Mass.

Both models use a Decision Tree Classifier and are trained on historical rocket launch data.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
  - [Weather-Based Model](#weather-based-model)
  - [Thrust-to-Weight Ratio Model](#thrust-to-weight-ratio-model)
- [How It Works](#how-it-works)
- [Example](#example)
- [Contributing](#contributing)
- [Acknowledgments](#acknowledgments)

## Overview

The goal of this project is to predict the success or failure of a rocket launch using two different approaches:

1. **Weather-Based Model:** Uses weather conditions (temperature, wind speed, and humidity) as input features.
2. **Thrust-to-Weight Ratio Model:** Uses the Thrust-to-Weight Ratio, calculated from Liftoff Thrust and Payload Mass, as the input feature.

Both models are implemented using a Decision Tree Classifier and can be used to make predictions for new inputs.

## Features

### Weather-Based Model:
- Takes Temperature (°F), Wind Speed (MPH), and Humidity (%) as input.
- Predicts whether the rocket launch will fail or succeed based on weather conditions.

### Thrust-to-Weight Ratio Model:
- Takes Liftoff Thrust (kN) and Payload Mass (kg) as input.
- Calculates the Thrust-to-Weight Ratio and predicts the outcome of the rocket launch.

## Installation

To use this project, follow these steps:

1. Clone the Repository:
    ```bash
    git clone https://github.com/your-username/rocket-failure-prediction.git
    cd rocket-failure-prediction
    ```

2. Install Required Libraries:
    ```bash
    pip install pandas scikit-learn numpy
    ```

3. Download the Dataset:
    - Place the `SpaceMissions.csv` file in the project directory. This dataset contains historical rocket launch data.

## Usage

### Weather-Based Model

**Train the Model:**
```bash
python train_weather_model.py
```

**Make Predictions:**
```bash
python predict_weather.py
```
The program will prompt you to enter:
- Temperature (°F)
- Wind Speed (MPH)
- Humidity (%)

Based on the input, the model will predict whether the rocket launch will fail or succeed.

### Thrust-to-Weight Ratio Model

**Train the Model:**
```bash
python train_thrust_weight_model.py
```

**Make Predictions:**
```bash
python predict_thrust_weight.py
```
The program will prompt you to enter:
- Liftoff Thrust (kN)
- Payload Mass (kg)

Based on the input, the model will predict whether the rocket launch will fail or succeed.

## How It Works

### Weather-Based Model
1. **Data Preprocessing:**
    - The dataset is loaded and preprocessed to handle missing values.
    - The target variable (`Mission Status`) is encoded as 0 for Success and 1 for Failure.
2. **Model Training:**
    - A Decision Tree Classifier is trained on the preprocessed data using weather features (Temperature, Wind Speed, Humidity).
3. **Prediction:**
    - The trained model takes user input for weather conditions and predicts the outcome of the rocket launch.

### Thrust-to-Weight Ratio Model
1. **Data Preprocessing:**
    - The dataset is loaded and preprocessed to handle missing values.
    - The Thrust-to-Weight Ratio is calculated using the formula:
      ```
      Thrust-to-Weight Ratio = Liftoff Thrust (kN) / (Payload Mass (kg) × 9.81)
      ```
    - The target variable (`Mission Status`) is encoded as 0 for Success and 1 for Failure.
2. **Model Training:**
    - A Decision Tree Classifier is trained on the preprocessed data using the Thrust-to-Weight Ratio as the input feature.
3. **Prediction:**
    - The trained model takes user input for Liftoff Thrust (kN) and Payload Mass (kg), calculates the Thrust-to-Weight Ratio, and predicts the outcome of the rocket launch.

## Example

### Weather-Based Model
```bash
Enter Temperature (°F): 75
Enter Wind Speed (MPH): 10
Enter Humidity (%): 80
Prediction: Rocket Launch Success
```

### Thrust-to-Weight Ratio Model
```bash
Enter Liftoff Thrust (kN): 5000
Enter Payload Mass (kg): 10000
Prediction: Rocket Launch Success
```

## Contributing

Contributions are welcome! If you'd like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Commit your changes.
4. Push your changes to your fork.
5. Submit a pull request.

## Acknowledgments

- **Dataset:** Space Missions Dataset
- **Libraries:** pandas, scikit-learn, numpy

