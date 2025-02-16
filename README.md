Rocket Failure Prediction Using Weather Data
This project uses a Decision Tree Classifier to predict whether a rocket launch will fail or succeed based on weather conditions such as temperature, wind speed, and humidity. The model is trained on historical rocket launch data and can be used to make predictions for new inputs.

Table of Contents

Overview
Features
Installation
Usage
How It Works
Example
Contributing
License
Overview

The goal of this project is to predict the success or failure of a rocket launch based on weather conditions. The model is trained using a Decision Tree Algorithm and takes three inputs from the user:

Temperature (°F)
Wind Speed (MPH)
Humidity (%)
Based on these inputs, the model predicts whether the rocket launch will fail or succeed.

Features

User Input: The program takes temperature, wind speed, and humidity as input from the user.
Prediction: The trained decision tree model predicts the outcome of the rocket launch.
Output: The program displays the prediction result (Success or Failure) to the user.
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
You can install them using pip:
bash
Copy
pip install pandas scikit-learn
Download the Dataset:
Place the SpaceMissions.csv file in the project directory. This dataset contains historical rocket launch data.
Usage

Train the Model:
Run the script to train the decision tree model:
bash
Copy
python train_model.py
Make Predictions:
After training the model, you can make predictions by running:
bash
Copy
python predict.py
The program will prompt you to enter the following inputs:
Temperature (°F)
Wind Speed (MPH)
Humidity (%)
Based on the input, the model will predict whether the rocket launch will fail or succeed.
How It Works

Data Preprocessing:
The dataset is loaded and preprocessed to handle missing values.
The target variable (Mission Status) is encoded as 0 for Success and 1 for Failure.
Model Training:
A Decision Tree Classifier is trained on the preprocessed data using weather features (Temperature, Wind Speed, Humidity).
Prediction:
The trained model takes user input for weather conditions and predicts the outcome of the rocket launch.
Example

Here’s an example of how the program works:

bash
Copy
Enter Temperature (°F): 75
Enter Wind Speed (MPH): 10
Enter Humidity (%): 80
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
Libraries: pandas, scikit-learn
