# Deep-Learning-CNN-based-X-ray-diagnosis-of-lung-effusion
In this project, Convolutional Neural Networks (CNNs) have been used to analyse chest X-ray images of patients to detect presence of "effusion". This is a classification problem, where we will be dealing with two classes - 'effusion' and 'nofinding'. Here, the latter represents a "normal" X-ray image.

# Data set
The data is in the form of grayscale (black and white) images of chest x-rays. Some of the images have presence of effusion whereas others are normal chest x-rays. All images are labelled as 'effusion' or 'nofinding'.

# Data pre-processing
Data pre-processing is done by normalising the images, centering it, scaling it to the same size etc. Further, data augmentation is done by applying random transformations to the image for training purposes. This is done by extending the ImageDataGenerator() sub-class of Keras.

# Model building
The resnet architecture for CNNs is used to build the model. The code for resnet architecture is present in a separate resnet.py file. 
This model is trained only for 10 epochs due to computational limitations

# Model evaluation
The resnet based model is able to achieve a 63.5% accuracy of correctly predicting presence of effusion in the x-ray image. This accuracy can be significantly improved if the number of training epochs is increased.
