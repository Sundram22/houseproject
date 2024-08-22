# House Price Prediction API
This project provides a RESTful API for predicting house prices using a machine learning model. The API is built with FastAPI and utilizes a pre-trained model loaded with pickle.

## Project Structure
main.py: The main FastAPI application file. It defines the API endpoints and handles model predictions.
para.py: Contains the Pydantic model for request validation.
regressor.pkl: The pre-trained machine learning model used for predictions.
## Installation
To get started, you'll need Python 3.7+ and pip. First, clone the repository:



#### curl -X POST "http://127.0.0.1:8000/predict" -H "Content-Type: application/json" -d '{
  "MedInc": 3.0,
  "HouseAge": 25.0,
  "AveRooms": 6.0,
  "AveBedrms": 1.0,
  "Population": 1000.0,
  "AveOccup": 2.0,
  "Latitude": 37.5,
  "Longitude": -122.0
}'

### Files
main.py: Contains the FastAPI application and prediction logic.
para.py: Defines the Pydantic model house_data used for request validation.
regressor.pkl: Serialized machine learning model for prediction.
Model
The machine learning model used for predictions is a pre-trained model serialized with pickle. Ensure that regressor.pkl is in the correct directory for the application to load the model successfully.


### Acknowledgements
FastAPI for building high-performance APIs.
scikit-learn for providing powerful machine learning tools.
