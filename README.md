# Mask Detection

This code creates a convolutional neural network (CNN) using the Keras library to classify images as either "masked" or "not masked." The CNN architecture consists of several convolutional layers followed by max pooling layers, a flattening layer, and fully connected dense layers. The model is then compiled with an Adam optimizer, binary cross-entropy loss, and accuracy as the evaluation metric. The training data is augmented using the ImageDataGenerator class and then used to train the model using the .fit() method. 

The model is then saved and used to classify images in the "testing" directory. The second part of the code loads the saved model and uses it to classify faces in a webcam video feed using the OpenCV library. It uses Haar cascades to detect faces and eyes in the video feed and then classifies the face as "masked" or "not masked" based on the output of the model.



## Dependencies

* Keras
* Tensorflow
* Numpy
* Matplotlib
* OpenCV
* Haarcascade_frontalface_default.xml and haarcascade_eye.xml
  
## Usage

* 1. Run the script
* 2. The model will train itself using augmented images
* 3. The model will be saved as "mask_detector_new_generated.h5"
* 4. The script will then use the model to classify images in the "testing" directory
* 5. The script will then use the saved model to classify faces in a webcam video feed.

## Resuts

The model should be able to classify images with an accuracy of about 80%.

## Future Work

* Increase the amount of training data
* Experiment with different CNN architectures
* Experiment with different image augmentation techniques

## Note

Please make sure that you have the necessary files (haarcascade_frontalface_default.xml and haarcascade_eye.xml) in the same directory as the script.

Please also make sure that the directory paths in the script point to the correct directories for your system.
