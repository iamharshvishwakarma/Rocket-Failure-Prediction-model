<h2>Table of Contents</h2>
<ul>
    <li><a href="#overview">Overview</a></li>
    <li><a href="#features">Features</a></li>
    <li><a href="#installation">Installation</a></li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#how-it-works">How It Works</a></li>
    <li><a href="#example">Example</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
</ul>

<h2 id="overview">Overview</h2>
<p>The goal of this project is to predict the success or failure of a rocket launch based on weather conditions.</p>
<ul>
    <li>Temperature (°F)</li>
    <li>Wind Speed (MPH)</li>
    <li>Humidity (%)</li>
</ul>

<h2 id="features">Features</h2>
<ul>
    <li><strong>User Input:</strong> The program takes temperature, wind speed, and humidity as input from the user.</li>
    <li><strong>Prediction:</strong> The trained decision tree model predicts the outcome of the rocket launch.</li>
    <li><strong>Output:</strong> The program displays the prediction result (Success or Failure) to the user.</li>
</ul>

<h2 id="installation">Installation</h2>
<h3>Clone the Repository:</h3>
<pre><code>git clone https://github.com/your-username/rocket-failure-prediction.git
cd rocket-failure-prediction
<h3>Install Required Libraries:</h3>
<pre><code>pip install pandas scikit-learn</code></pre>

<h2 id="usage">Usage</h2>
<h3>Run the Model:</h3>
<pre><code>python rocket_failure_prediction.py</code></pre>
<p>The program will prompt you to enter:</p>
<ul>
    <li>Temperature (°F)</li>
    <li>Wind Speed (MPH)</li>
    <li>Humidity (%)</li>
</ul>

<h2 id="how-it-works">How It Works</h2>
<ul>
    <li><strong>Data Preprocessing:</strong> The dataset is loaded and preprocessed to handle missing values.</li>
    <li><strong>Model Training:</strong> A Decision Tree Classifier is trained on the preprocessed data.</li>
    <li><strong>Prediction:</strong> The trained model takes user input and predicts the outcome.</li>
</ul>

<h2 id="example">Example</h2>
<pre><code>Enter Temperature (°F): 75
Enter Wind Speed (MPH): 10
Enter Humidity (%): 80
Prediction: Rocket Launch Success
<h2 id="contributing">Contributing</h2>
<p>Contributions are welcome! Follow these steps:</p>
<ol>
    <li>Fork the repository.</li>
    <li>Create a new branch for your feature or bugfix.</li>
    <li>Commit your changes.</li>
    <li>Push your changes to your fork.</li>
    <li>Submit a pull request.</li>
</ol>

<h2 id="license">License</h2>
<p>This project is licensed under the MIT License. See the <a href="LICENSE">LICENSE</a> file for details.</p>

<h2 id="acknowledgments">Acknowledgments</h2>
<ul>
    <li><strong>Dataset:</strong> Space Missions Dataset</li>
    <li><strong>Libraries:</strong> pandas, scikit-learn</li>
</ul>
