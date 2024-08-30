# Image Classification Model and API

This project demonstrates how to build and deploy an image classification model using TensorFlow and serve predictions through a Flask API.

## Files

- `train_model.py`: Script to train and save the TensorFlow model.
- `app.py`: Flask application to serve the model and make predictions.
- `requirements.txt`: List of dependencies required for the project.
- `README.md`: Project documentation.

## Setup

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
Train and save the model:

python train_model.py
Run the Flask API:

python app.py
Send a POST request to /predict with an image file to get the classification result.

Example Usage
You can use tools like curl or Postman to send image files to the API:

Using curl:
curl -X POST -F "file=@path_to_your_image" http://localhost:5000/predict
Using Postman:
Open Postman.
Select POST as the request type.
Enter http://localhost:5000/predict as the request URL.
Go to the "Body" tab and select "form-data".
Add a key named file and select "File" as the type.
Choose an image file to upload.
Click "Send" to get the prediction result.
Notes
Ensure that TensorFlow and Flask are installed and that the model is correctly saved before running the Flask application.
Adjust the image preprocessing in app.py if using a different dataset or model architecture.

Feel free to modify any details based on your specific setup or needs!