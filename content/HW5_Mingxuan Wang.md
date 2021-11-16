Title: Assignment 5 Description
Slug: Assignment 5 Description
Date: 11/15/2021
Category: Assignment 5
Author: Mingxuan Wang
Summary: Description of Assignment 5

I uploaded the zip picture file into the container and extract them with "zipfile". 
Then, I load the training and testing set using "tf.keras.utils.image_dataset_from_directory" and convert pictures to arrays using "np.concatenate". 
In order to train a cnn model, I normalize the X_train and X_test.

To have a look at a single picture and its lable in the dataset, I write a function called "plot_sample" using matplotlib.

Then, train the convolutional neural network to classify the images. Using two convolution and two max pooling layers. 
The number of output filters in the convolution is set to be 32 and 64. Kernel size is 3 by 3. Using 'relu' as the activation function. 
For the dense layer, 'relu' and 'softmax' are used as the activation function. 
Then compile the cnn using 'sparse_categorical_crossentropy' as loss.

Then, fit the model on the training set, set epochs to be 10.
The accuracy is 99.9%. According to the confusion matrix, all the 180 samples are classified correctly.

Using SHAP to explain the deep learning model. Select 4 background examples and explain the predictions of model by plotting the feature attributions.


