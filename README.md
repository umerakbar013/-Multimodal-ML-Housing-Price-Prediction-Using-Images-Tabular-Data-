# -Multimodal-ML-Housing-Price-Prediction-Using-Images-Tabular-Data-
internship project

 Multimodal Housing Price Prediction
This project demonstrates a Multimodal Machine Learning approach for predicting housing prices using both tabular data (like number of rooms, income, etc.) and images of houses. A custom deep learning model combines features extracted via a CNN from house images with structured numerical features.

Dataset Overview
The housing.csv file contains columns such as:

Avg. Area Number of Bedrooms

Avg. Area Number of Rooms

Avg. Area Income

Price (target variable)

Each row corresponds to an image named as {index}.jpg (e.g., 0.jpg, 1.jpg, etc.).

Model Architecture
Image Branch (CNN):

Convolution + MaxPooling layers

Dense layers for learned image features

Tabular Branch:

Dense layers on scaled numerical features

Fusion:

Concatenated feature vector from both branches

Fully connected layers for final prediction

 Dependencies


Install all required libraries with:

bash
Copy
Edit
pip install numpy pandas opencv-python scikit-learn tensorflow keras

Training
Loss Function: Mean Squared Error (MSE)

Optimizer: Adam

Epochs: 10

Batch Size: 16

Train/Validation Split: 90/10

 Evaluation
Evaluated on test data using:

MAE (Mean Absolute Error)

RMSE (Root Mean Squared Error)

Sample Output:

makefile
Copy
Edit
MAE: 275413.90
RMSE: 346417.91
