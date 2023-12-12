# Computer_Vision
This project uses the Microsoft Azure Custom Vision to train images and afterwards exposes a prediction API. This API is called from a client e.g. a notebook to get the predictions.

# Steps to Set up the model
Create a Custom Vision resource in Azure Portal.
Create a new project in the Custom Vision web portal.
Choose the classification type (Multilabel or Multiclass) and domain (Generic or Food).
Upload your training images in .jpg, .png, .bmp, or .gif format no greater than 6MB in size (4MB for prediction images) no less than 256 pixels on the shortest edge.
Train your model.
Test your model with new images.
Integrate your model into your own image recognition app.

# Steps to Call the Prediction API

How to use the Prediction API
If you have an image URL:
https://createml-prediction.cognitiveservices.azure.com/customvision/v3.0/Prediction/cdc5c8e7-8d21-4ca6-95ca-0fff94a53a85/classify/iterations/Cat%20Detection/url
Set Prediction-Key Header to : 17cfd001ecaa4341b776ac53ae73eb61
Set Content-Type Header to : application/json
Set Body to : {"Url": "https://example.com/image.png"}
If you have an image file:
https://createml-prediction.cognitiveservices.azure.com/customvision/v3.0/Prediction/cdc5c8e7-8d21-4ca6-95ca-0fff94a53a85/classify/iterations/Cat%20Detection/image
Set Prediction-Key Header to : 17cfd001ecaa4341b776ac53ae73eb61
Set Content-Type Header to : application/octet-stream
Set Body to : <image file>

