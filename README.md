# Computer_Vision
This project uses Microsoft Azure Custom Vision to train images and afterwards expose a prediction API. This API is called from a client e.g. a notebook to get the predictions.

# Steps to Set up the model
Create a Custom Vision resource in Azure Portal.
Create a new project in the Custom Vision web portal.
Choose the classification type (Multilabel or Multiclass) and domain (Generic or Food).
Upload your training images in .jpg, .png, .bmp, or .gif format no greater than 6MB in size (4MB for prediction images) no less than 256 pixels on the shortest edge.
Train your model.
Test your model with new images.
Integrate your model into your own image recognition app.

