**CrimeSense:**

A Deep Learning Approach to Crime Classification

CrimeSense is a Python application that leverages deep learning to classify crime events in videos. 

It employs a pre-trained convolutional neural network (CNN) model, MobileNetV2, in conjunction with data augmentation to achieve robust video frame classification.

**Key Features**

**Trainable CNN Model:**

 1. Utilize a pre-trained MobileNetV2 model or explore alternative pre-trained CNNs for crime classification

 2. Video Frame Extraction: Extract frames efficiently from videos for classification.

 3. Data Augmentation: Enhance model generalization by applying data augmentation techniques like shear, zoom, flip, rotation, and shift.

 4. Customizable Crime Classes: Tailor the crime class labels to match your specific dataset and crime definitions.
       
**Clear Output:**
               Obtain predicted crime class and its percentage for each image in the video, along with a summary of class distributions.
**Getting Started**

**Prerequisites:**

Python 3.x (with necessary libraries: TensorFlow, Keras, OpenCV, etc.)

Install required libraries using pip install -r requirements.txt (assuming a requirements.txt file exists)

**Train Your Model:**

Prepare your training dataset with labeled folders (e.g., Abuse, Arrest, etc.) containing video files.

Modify training and validation paths (currently E://Train and E://Test) in crime_classification_model.py to match your dataset location.

Run python crime_classification_model.py to train the model.

The trained model will be saved as crime_detection_model_optimized_1.h5.

**Video Crime Classification:**

Place your test video in the video directory.

Run python crime_video_classification.py to analyze the video frames and provide predictions.

The script will extract frames, classify them using the saved model, and print the results.

**Customization**

**Crime Classes:**

Modify the crime_classes list in crime_video_classification.py to match your crime categories.

**Pre-trained Model:**

Experiment with different pre-trained CNN models (e.g., EfficientNetB0) in crime_classification_model.py by replacing MobileNetV2.
Data Augmentation:

Adjust data augmentation parameters (e.g., shear, zoom ranges) in crime_classification_model.py to optimize performance.
