# Traffic-Sign-Classification-Model

#  PROBLEM STATEMENT
- In this case study, you have been provided with images of traffic signs and the goal is to train a Deep Network to classify them
- The dataset contains 43 different classes of images. 
- Classes are as listed below: 

    - ( 0, b'Speed limit (20km/h)') ( 1, b'Speed limit (30km/h)')
    - ( 2, b'Speed limit (50km/h)') ( 3, b'Speed limit (60km/h)')
    - ( 4, b'Speed limit (70km/h)') ( 5, b'Speed limit (80km/h)')
    - ( 6, b'End of speed limit (80km/h)') ( 7, b'Speed limit (100km/h)')
    - ( 8, b'Speed limit (120km/h)') ( 9, b'No passing')
    - (10, b'No passing for vehicles over 3.5 metric tons')
    - (11, b'Right-of-way at the next intersection') (12, b'Priority road')
    - (13, b'Yield') (14, b'Stop') (15, b'No vehicles')
    - (16, b'Vehicles over 3.5 metric tons prohibited') (17, b'No entry')
    - (18, b'General caution') (19, b'Dangerous curve to the left')
    - (20, b'Dangerous curve to the right') (21, b'Double curve')
    - (22, b'Bumpy road') (23, b'Slippery road')
    - (24, b'Road narrows on the right') (25, b'Road work')
    - (26, b'Traffic signals') (27, b'Pedestrians') (28, b'Children crossing')
    - (29, b'Bicycles crossing') (30, b'Beware of ice/snow')
    - (31, b'Wild animals crossing')
    - (32, b'End of all speed and passing limits') (33, b'Turn right ahead')
    - (34, b'Turn left ahead') (35, b'Ahead only') (36, b'Go straight or right')
    - (37, b'Go straight or left') (38, b'Keep right') (39, b'Keep left')
    - (40, b'Roundabout mandatory') (41, b'End of no passing')
    - (42, b'End of no passing by vehicles over 3.5 metric tons')

# PROJECT OVERVIEW:
-- First of all,we need to check whether it is regression task or classifiction task...
        
    It is a classification task as we have to classify a sign into thier true classes.
-- Here,we are going to use LeNet-5 architecture, a classic Convolutional Neural Networks(CNNs) architecture, to get this task done.

Convolutional Neural Networks(CNNs) are extended version of Artifical neural netwroks (ANNs) which are predominantly used to extract the feature from grid like matrix. It is used in visual datasets like images or videos where data patterns play an extensive role.

# STEPS TAKEN:

So,here are the step I followed in this problem statement:

--> Step-1: Importing the libraries and Load the Dataset
- Import libraries like numpy(for basic calculations),pandas(for dataframes references),matplotlib(for graph plotting) and seaborn(for visualising the data) and pickle (for serializing and deserializing Python objects). This allows users to save complex data structures, like dictionaries, lists, and custom classes, to a file or send them to another program over a network.
- Now load all the three sets :test,train and validation set
- Put features of set in X and labels of set in y.

--> Step-2: Image Exploration
- Accesing image from a dataset on a specific index.

--> Step-3: Data Preparation
- Shuffle the dataset.
- Convert RGB (Red, Green, Blue) images to grayscale in a machine learning or computer vision context for each dataset.
- Now, do normalisation on grayscale images after converting them from RGB.
- Visualize the original RGB image, the corresponding grayscale image, and the normalized grayscale image for each dataset at specific index.

--> Step-4: Model Training
-  Import necessary modules for building a convolutional neural network (CNN) using the Keras library.
-  Construct LeNet-5 Architecure by adding all those layer using appropriate number of filters and kernel size.
-  Train the CNN Model using the training dataset and validate it to validation dataset.

--> Step-5: Model Evaluation
- Evaluate the trained CNN model on the test set and prints the test accuracy.
- Plot the training and validation accuracy over epochs.
- Plot the training and validation loss over epochs.
- Using scikit-learn library, generate and visualize a confusion matrix for evaluating the performance of a classification model.
- Create a grid of subplots to visualize a set of images from the test set along with their corresponding predictions and true labels.
