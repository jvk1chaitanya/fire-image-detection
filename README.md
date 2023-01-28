# Fire Detection Project
This project is focused on detecting fire in images using a deep learning model. The aim of this project is to detect fire in images using a convolutional neural network (CNN) and to create a model that can be used to detect fire in real-time. The notebook for this project was created on Kaggle, an online platform for data science competitions, and the source of data used for this project is also from Kaggle. The programming language used for this project is Python and the following libraries are used:

OS: The os library is used to interact with the operating system. It provides functions for working with files, directories, and other aspects of the system. In this project, it is used to navigate and manipulate the file system to access the images used for training and testing.

Tensorflow: Tensorflow is an open-source library for machine learning and deep learning. It provides a framework for building and training neural networks. In this project, it is used to create and train the CNN model used for fire detection.

Numpy: Numpy is a library for working with arrays and matrices. It provides functions for performing mathematical operations on arrays, such as element-wise operations, linear algebra, and Fourier transforms. In this project, it is used to manipulate and process the images used for training and testing.

Matplotlib: Matplotlib is a library for creating visualizations. It provides functions for creating plots, histograms, and other types of figures. In this project, it is used to view the images used for training and testing.

## Data Exploration
The first step in creating a deep learning model is to explore the data that will be used to train the model. In this project, the sample images were viewed using the matplotlib.image library. This library allows us to view the images and get a sense of the data that we will be working with. The images were pre-processed using tensorflow's ImageDataGenerator, which includes functions such as rescaling, rotation, and other image preprocessing techniques. These techniques are used to enhance the images and make them more suitable for training the model.

## Model Creation
Once the data has been explored, the next step is to create the model. In this project, the model used is tensorflow's resnet-50 with a custom top layer. The resnet-50 model is a pre-trained model that has been trained on a large dataset of images and has been shown to be effective in image classification tasks. The custom top layer includes classes such as sequential, Dense, and dropout. These classes are used to create the structure of the model and to add additional layers to the model. The model was optimized using the Adam optimizer, which is a popular optimization algorithm used in deep learning. Tensorflow's LearningRateScheduler and ModelCheckpoint were used for better results. These functions are used to schedule the learning rate and to save the model's parameters at different stages of training.

## Model Evaluation
Once the model has been created and trained, it needs to be evaluated to see how well it performs. The model was primarily evaluated using validation loss, which measures the difference between the model's predictions and the true values. Additionally, the accuracy of the model was also used to view the results. The accuracy is a measure of how well the model is able to correctly classify theimages as fire or non-fire.

## Custom Functions
Two custom functions were created in this project to make it easier for users to work with the model. The first function is 'load_and_prep_image' which is used to resize an image and convert it to a tensor before the model does the prediction. This function takes in the path of an image and the size to which the image needs to be changed as parameters. The second function is 'pred_and_plot' which takes in the path of an image and the model as parameters and outputs the image and the predicted output. This function also uses the 'load_and_prep_image' function to resize and convert the image to a tensor before the model makes the prediction.

## Conclusion
This project demonstrates how to use a deep learning model to detect fire in images. The model created in this project can be used to detect fire in real-time and can be further improved by training it on a larger dataset. By using the custom functions created in this project, it becomes easier for users to work with the model and make predictions on new images.

One real-world use case of this project is in the field of wildfire detection. Wildfires can cause significant damage to both property and the environment, and early detection is crucial in preventing these fires from spreading. By using this model, a wildfire detection system could be implemented to automatically detect fires in remote or hard-to-reach areas, allowing for a faster response time and potentially saving lives and property.

Another real-world use case is in industrial environments where fire detection is critical for safety. This model could be integrated into existing fire detection systems to improve their accuracy and efficiency.

Overall, this project serves as a good starting point for anyone interested in creating a fire detection system using deep learning. With the right modifications and training, this model has the potential to make a real impact in various fields, including wildfire detection and industrial safety.

## Accessing the Code and Data
The notebook and data used in this project can be found in the following GitHub folder: link to the folder

In this folder, you will find the Jupyter notebook containing the code used in this project as well as the data used for training and testing the model. Feel free to use and modify the code as you see fit for your own projects.
