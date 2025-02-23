Rocket Failure Prediction Models
This repository contains two machine learning models for predicting rocket launch failures:

Weather-Based Model: Predicts rocket failure based on weather conditions (temperature, wind speed, and humidity).
Thrust-to-Weight Ratio Model: Predicts rocket failure based on the Thrust-to-Weight Ratio, calculated using Liftoff Thrust and Payload Mass.
Both models use a Decision Tree Classifier and are trained on historical rocket launch data.

Table of Contents

Overview
Features
Installation
Usage
Weather-Based Model
Thrust-to-Weight Ratio Model
How It Works
Example
Contributing
License
Overview

The goal of this project is to predict the success or failure of a rocket launch using two different approaches:

Weather-Based Model: Uses weather conditions (temperature, wind speed, and humidity) as input features.
Thrust-to-Weight Ratio Model: Uses the Thrust-to-Weight Ratio, calculated from Liftoff Thrust and Payload Mass, as the input feature.
Both models are implemented using a Decision Tree Classifier and can be used to make predictions for new inputs.

Features

Weather-Based Model:
Takes Temperature (°F), Wind Speed (MPH), and Humidity (%) as input.
Predicts whether the rocket launch will fail or succeed based on weather conditions.
Thrust-to-Weight Ratio Model:
Takes Liftoff Thrust (kN) and Payload Mass (kg) as input.
Calculates the Thrust-to-Weight Ratio and predicts the outcome of the rocket launch.
Installation

To use this project, follow these steps:

Clone the Repository:
bash
Copy
git clone https://github.com/your-username/rocket-failure-prediction.git
cd rocket-failure-prediction
Install Required Libraries:
Ensure you have the following Python libraries installed:
pandas
scikit-learn
numpy
You can install them using pip:
bash
Copy
pip install pandas scikit-learn numpy
Download the Dataset:
Place the SpaceMissions.csv file in the project directory. This dataset contains historical rocket launch data.
Usage

Weather-Based Model

Train the Model:
Run the script to train the weather-based model:
bash
Copy
python train_weather_model.py
Make Predictions:
After training the model, you can make predictions by running:
bash
Copy
python predict_weather.py
The program will prompt you to enter the following inputs:
Temperature (°F)
Wind Speed (MPH)
Humidity (%)
Based on the input, the model will predict whether the rocket launch will fail or succeed.
Thrust-to-Weight Ratio Model

Train the Model:
Run the script to train the Thrust-to-Weight Ratio model:
bash
Copy
python train_thrust_weight_model.py
Make Predictions:
After training the model, you can make predictions by running:
bash
Copy
python predict_thrust_weight.py
The program will prompt you to enter the following inputs:
Liftoff Thrust (kN)
Payload Mass (kg)
Based on the input, the model will predict whether the rocket launch will fail or succeed.
How It Works

Weather-Based Model

Data Preprocessing:
The dataset is loaded and preprocessed to handle missing values.
The target variable (Mission Status) is encoded as 0 for Success and 1 for Failure.
Model Training:
A Decision Tree Classifier is trained on the preprocessed data using weather features (Temperature, Wind Speed, Humidity).
Prediction:
The trained model takes user input for weather conditions and predicts the outcome of the rocket launch.
Thrust-to-Weight Ratio Model

Data Preprocessing:
The dataset is loaded and preprocessed to handle missing values.
The Thrust-to-Weight Ratio is calculated using the formula:
Thrust-to-Weight Ratio
=
Liftoff Thrust (kN)
Payload Mass (kg)
×
9.81
Thrust-to-Weight Ratio= 
Payload Mass (kg)×9.81
Liftoff Thrust (kN)
​	
 
The target variable (Mission Status) is encoded as 0 for Success and 1 for Failure.
Model Training:
A Decision Tree Classifier is trained on the preprocessed data using the Thrust-to-Weight Ratio as the input feature.
Prediction:
The trained model takes user input for Liftoff Thrust (kN) and Payload Mass (kg), calculates the Thrust-to-Weight Ratio, and predicts the outcome of the rocket launch.
Example

Weather-Based Model

bash
Copy
Enter Temperature (°F): 75
Enter Wind Speed (MPH): 10
Enter Humidity (%): 80
Prediction: Rocket Launch **Success**
Thrust-to-Weight Ratio Model

bash
Copy
Enter Liftoff Thrust (kN): 5000
Enter Payload Mass (kg): 10000
Prediction: Rocket Launch **Success**
Contributing

Contributions are welcome! If you'd like to contribute to this project, please follow these steps:

Fork the repository.
Create a new branch for your feature or bugfix.
Commit your changes.
Push your changes to your fork.
Submit a pull request.
License

This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments

Dataset: Space Missions Dataset
Libraries: pandas, scikit-learn, numpy
