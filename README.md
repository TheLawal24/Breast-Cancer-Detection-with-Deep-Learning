# Breast-Cancer-Detection-with-Deep-Learning
Breast Cancer Detection with DL – Objective
Aim at building a breast cancer classifier on an IDC dataset that can accurately classify a histology image as benign or malignant.

Breast Cancer Detection – About the Python Project
In this project in python, we’ll build a classifier to train on 80% of a breast cancer histology image dataset. Of this, we’ll keep 10% of the data for validation. Using Keras, we’ll define a CNN (Convolutional Neural Network), call it CancerNet, and train it on our images. We’ll then derive a confusion matrix to analyze the performance of the model.

IDC is Invasive Ductal Carcinoma; cancer that develops in a milk duct and invades the fibrous or fatty breast tissue outside the duct; it is the most common form of breast cancer forming 80% of all breast cancer diagnoses. And histology is the study of the microscopic structure of tissues.
What is Deep Learning?
An intensive approach to Machine Learning, Deep Learning is inspired by the workings of the human brain and its biological neural networks. Architectures as deep neural networks, recurrent neural networks, convolutional neural networks, and deep belief networks are made of multiple layers for the data to pass through before finally producing the output. Deep Learning serves to improve AI and make many of its applications possible; it is applied to many such fields of computer vision, speech recognition, natural language processing, audio recognition, and drug design.

What is Keras?
Keras is an open-source neural-network library written in Python. It is a high-level API and can run on top of TensorFlow, CNTK, and Theano. Keras is all about enabling fast experimentation and prototyping while running seamlessly on CPU and GPU. It is user-friendly, modular, and extensible.

The Dataset?
We’ll use the IDC_regular dataset (the breast cancer histology image dataset) from Kaggle. This dataset holds 2,77,524 patches of size 50×50 extracted from 162 whole mount slide images of breast cancer specimens scanned at 40x. Of these, 1,98,738 test negative and 78,786 test positive with IDC. The dataset is available in public domain and you can download it here. You’ll need a minimum of 3.02GB of disk space for this.

Filenames in this dataset look like this:

8863_idx5_x451_y1451_class0

Here, 8863_idx5 is the patient ID, 451 and 1451 are the x- and y- coordinates of the crop, and 0 is the class label (0 denotes absence of IDC).

Blog Home
Data Science
Categories
Free Courses

Search for:
Search …
Project in Python – Breast Cancer Classification with Deep Learning

Free Machine Learning courses with 130+ real-time projects Start Now!!

If you want to master Python programming language then you can’t skip projects in Python. After publishing 4 advanced python projects, DataFlair today came with another one that is the Breast Cancer Classification project in Python. To crack your next Python Interview, practice these projects thoroughly and if you face any confusion, do comment, DataFlair is always ready to help you.


Before we begin this Breast Cancer Classification Project in Python, let me provide you the list of advanced python projects published by DataFlair:

Fake News Detection Python Project 
Parkinson’s Disease Detection Python Project 
Color Detection Python Project
Speech Emotion Recognition Python Project 
Breast Cancer Classification Python Project
Age and Gender Detection Python Project 
Handwritten Digit Recognition Python Project
Chatbot Python Project
Driver Drowsiness Detection Python Project
Traffic Signs Recognition Python Project
Image Caption Generator Python Project
Breast Cancer Classification Project in Python
Get aware with the terms used in Breast Cancer Classification project in Python

What is Deep Learning?
An intensive approach to Machine Learning, Deep Learning is inspired by the workings of the human brain and its biological neural networks. Architectures as deep neural networks, recurrent neural networks, convolutional neural networks, and deep belief networks are made of multiple layers for the data to pass through before finally producing the output. Deep Learning serves to improve AI and make many of its applications possible; it is applied to many such fields of computer vision, speech recognition, natural language processing, audio recognition, and drug design.

What is Keras?
Keras is an open-source neural-network library written in Python. It is a high-level API and can run on top of TensorFlow, CNTK, and Theano. Keras is all about enabling fast experimentation and prototyping while running seamlessly on CPU and GPU. It is user-friendly, modular, and extensible.

Breast Cancer Classification – Objective
To build a breast cancer classifier on an IDC dataset that can accurately classify a histology image as benign or malignant.
ad

Breast Cancer Classification – About the Python Project
In this project in python, we’ll build a classifier to train on 80% of a breast cancer histology image dataset. Of this, we’ll keep 10% of the data for validation. Using Keras, we’ll define a CNN (Convolutional Neural Network), call it CancerNet, and train it on our images. We’ll then derive a confusion matrix to analyze the performance of the model.

IDC is Invasive Ductal Carcinoma; cancer that develops in a milk duct and invades the fibrous or fatty breast tissue outside the duct; it is the most common form of breast cancer forming 80% of all breast cancer diagnoses. And histology is the study of the microscopic structure of tissues.

The Dataset

We’ll use the IDC_regular dataset (the breast cancer histology image dataset) from Kaggle. This dataset holds 2,77,524 patches of size 50×50 extracted from 162 whole mount slide images of breast cancer specimens scanned at 40x. Of these, 1,98,738 test negative and 78,786 test positive with IDC. The dataset is available in public domain and you can download it here. You’ll need a minimum of 3.02GB of disk space for this.

Filenames in this dataset look like this:

8863_idx5_x451_y1451_class0

Here, 8863_idx5 is the patient ID, 451 and 1451 are the x- and y- coordinates of the crop, and 0 is the class label (0 denotes absence of IDC).

Prerequisites:
We’ll need to install some python packages to be able to run this advanced python project. You can do this with pip-

pip install numpy opencv-python pillow tensorflow keras imutils scikit-learn matplotlib
Steps for Advanced Project in Python – Breast Cancer Classification
1. Download this zip. Unzip it at your preferred location, get there.
breast cancer detection python project
2. Now, inside the inner breast-cancer-classification directory, create directory datasets- inside this, create directory original:
mkdir datasets
mkdir datasets\original
3. Download the dataset.
4. Unzip the dataset in the original directory. To observe the structure of this directory, we’ll use the tree command:
cd breast-cancer-classification\breast-cancer-classification\datasets\original
tree
We have a directory for each patient ID. And in each such directory, we have the 0 and 1 directories for images with benign and malignant content.
by now, you should have declare the path to the input dataset (datasets/original), that for the new directory (datasets/idc), and the paths for the training, validation, and testing directories using the base path. We also declare that 80% of the entire dataset will be used for training, and of that, 10% will be used for validation.

build_dataset.py:
This will split our dataset into training, validation, and testing sets in the ratio mentioned above- 80% for training (of that, 10% for validation) and 20% for testing. With the ImageDataGenerator from Keras, we will extract batches of images to avoid making space for the entire dataset in memory at once.

DM or send me an Email for continuation.

To be continued...
