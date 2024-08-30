Delivery Time Prediction
A machine learning project to predict delivery durations based on features such as distance, delivery type, and weather conditions using a Random Forest Regressor.

Overview
This project aims to provide a solution for predicting delivery times for logistics services. The model is trained using a dataset containing information about previous deliveries, including start and end times, distances, delivery types, and weather conditions. By training a Random Forest Regressor, the model can accurately predict the duration of future deliveries.

Features
Predict delivery durations based on historical data
Use of Random Forest algorithm for better accuracy
Ability to calculate exact delivery dates based on current date and time
Dataset
The dataset used for this project (delivery2.csv) contains the following columns:

Start_Time: The start time of the delivery
End_Time: The end time of the delivery
Distance_km: The distance covered during the delivery
Delivery_Type: The type of delivery (e.g., Standard, Express)
Weather_Conditions: Weather conditions during the delivery (e.g., Sunny, Rainy)
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/delivery-time-prediction.git
cd delivery-time-prediction
Create and activate a virtual environment (optional but recommended):

bash
Copy code
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
Install the required dependencies:

bash
Copy code
pip install -r requirements.txt
Usage
Prepare your dataset: Ensure your dataset delivery2.csv is in the correct format and placed in the project directory.

Run the script:

bash
Copy code
python main.py
This script will train the model using the provided dataset and output the mean absolute error of the predictions.

Predict delivery time: You can use the predict_delivery_time function in main.py to predict the delivery duration for new inputs.

Example:

python
Copy code
predicted_duration = predict_delivery_time(10, 'Standard', 'Sunny')
print("Predicted delivery duration in days:", predicted_duration)
Calculate the delivery date: The script also provides a function to calculate the exact delivery date based on the predicted duration and the current date.
