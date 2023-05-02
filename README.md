# Smile-Detector: A ML and OpenCV Based System for Accurate Smile Detection 
### By [Steven Kam('25)](https://github.com/SKam23), [Shaheer Aslam('25)](https://github.com/shaheermaslam02),[Sajan Shah('25)](https://github.com/sajshah6)

The **Smile-Dectector** is an advanced machine learning project that uses computer vision techniques to accurately detect whether or not a person is smiling. Leveraging a dataset of 10,000 celebrity images, with 5,000 labeled as smiling and 5,000 labeled as not smiling, we trained a Convolutional Neural Network (CNN) using TensorFlow to classify images based on the presence of a smile. Our model was optimized using hyperparameter tuning and achieved an accuracy of over 95% on a holdout test set, making it highly accurate for practical applications.

## Dataset

To train our Smile Detection model, we utilized a subset of the CelebA Dataset which can be found [here](https://github.com/SKam23/SmileData). The repository contains 10,000 face images of various celebrities, with 5,000 images of smiling faces and 5,000 images of non-smiling faces. The dataset is partitioned into training, validation, and testing sets, and each image contains 40 attribute labels ranging from whether the celebrity is smiling, bold, has arched eyebrows, is young, and more. 

## Models

We experimented with different deep learning architectures, including Convolutional Neural Networks (CNN), Fully Convolutional Networks (FCN), and MobileNet models. We trained each model on the dataset and evaluated their accuracy on the testing set. After comparing the performance of the models, we selected the best performing model for live smile detection.

## Live Smile Detection

Smile Dectector utilized the trained CNN and MobleNet Models and the OpenCV computer vision library to accurately detect and enable real-time smile detection on live video feeds. Our system uses OpenCV to capture and process video frames, and then applies our pre-trained CNN model to classify each frame as "smiling" or "not smiling". This process is performed on the GPU for faster performance, allowing our system to achieve high throughput and low latency even on low-end hardware.


