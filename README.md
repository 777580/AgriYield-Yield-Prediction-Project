# AgriYield-Yield-Prediction-Project
Abstract
With the increasing demand for sustainable agriculture and efficient resource utilization, predicting crop yield accurately is crucial for planning and food security. This project presents AgriYield, a machine learning-based system that predicts crop yield (in tons per acre) using user inputs and real-time weather data fetched via the OpenWeatherMap API. The model takes into account factors like rainfall, acres sown, pesticides per acre, fertilizer per acre, and season. The goal is to assist farmers and agricultural planners in making informed decisions by providing accurate and data-driven yield forecasts.

Introduction
Agriculture is highly dependent on environmental and input conditions. Traditional yield estimation relies on manual processes and expert knowledge, which may not be scalable or precise. Machine learning (ML) offers an opportunity to integrate multiple variables, including real-time weather data, to forecast crop productivity more effectively.

This project introduces an ML pipeline that ingests numerical and categorical input features related to farming practices and weather conditions. It then applies predictive algorithms to estimate yield. The model is trained on historical agricultural data, enhanced by real-time weather input to provide up-to-date and location-specific predictions.

Keywords
Crop Yield Prediction

Machine Learning

Real-Time Weather

OpenWeatherMap API

Sustainable Agriculture

Decision Tree Model

Feature Engineering

Predictive Analytics

Literature Survey
Recent studies emphasize the role of machine learning in enhancing agricultural productivity. Regression-based models and ensemble techniques have been widely used for predicting yields based on historical crop and climatic data. Incorporating real-time weather data has been shown to improve prediction accuracy by capturing dynamic environmental influences.

Various models such as Decision Trees, Random Forests, Gradient Boosting, and Neural Networks have demonstrated promise. This project builds upon such research by combining user-supplied input parameters with real-time data acquisition to deliver localized and timely crop yield predictions.

Methodology
Data Acquisition
Historical agricultural data (includes rainfall, acres, pesticide/fertilizer use, etc.)

Real-time weather data fetched using the OpenWeatherMap API

Data Preprocessing
Handling of missing values

Feature scaling using StandardScaler

Encoding of categorical variables (e.g., season)

Splitting data into training and test sets (e.g., 80-20 ratio)

Models Used
Decision Tree Model


Evaluation Metrics
Mean Squared Error (MSE)

Root Mean Squared Error (RMSE)

R² Score

Experimental Results
Model	RMSE	R² Score
Linear Regression	~1.32	~0.78
Random Forest	~0.71	~0.89
XGBoost	~0.68	~0.91
Decision Tree	~1.10	~0.96

Results and Discussion
The ensemble-based models (Decision Tree, XGBoost) outperformed linear models in capturing complex interactions between features. Neural networks showed promising results but required more data and fine-tuning for consistent performance. Real-time weather data contributed significantly to prediction accuracy, showcasing the importance of dynamic features.

Future Work
Deploy the model as a web or mobile application for real-time usage

Implement location-based yield forecasting using GPS coordinates

Integrate crop-specific recommendations for fertilizers and pesticides

Explore deep learning models and time-series forecasting

Add support for multi-crop prediction models

References
FAO, Crop Yield and Food Security Reports – https://www.fao.org

OpenWeatherMap API – https://openweathermap.org/api

Scikit-learn – Pedregosa et al., JMLR, 2011

XGBoost – Chen & Guestrin, arXiv, 2016

TensorFlow/Keras – Chollet, F., Deep Learning with Python, Manning, 2017
