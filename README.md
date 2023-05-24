
# Automated Crack Detection in Civil Structures
# Overview
In civil structures, cracks on concrete or infrastructure surfaces pose a significant threat as they compromise the rigidity and tensile strength of buildings. Building inspection plays a crucial role in evaluating the health of a structure, and crack detection is an essential part of this process. However, manual identification of cracks is time-consuming and prone to human error. To address this challenge, an automated system is required to accurately detect and classify cracks in concrete surfaces, enabling efficient building inspections and facilitating the assessment of building health.

This project aims to utilize deep learning image classification models to identify cracks in different types of material surfaces. Two datasets have been collected for this purpose, each with its own characteristics.

# Dataset I: Surface Photos for Single Material Cracks
This dataset consists of surface photos of cracks in a single material. The dataset is well-balanced, with an equal number of positive and negative cases.

__Dataset Details__
1. 20,000 images of surface cracks with dimensions 227 x 227 pixels and RGB channels
2. 20,000 images of non-cracked surfaces with dimensions 227 x 227 pixels and RGB channels
3. The surface cracks images are retrieved from various civil structures.

__Model Selection__

For Dataset I, a Convolutional Neural Network (CNN) has been chosen as the deep learning image classification model. The decision to use CNN is based on the following reasons:

1. High accuracy in detecting cracks
2. High precision, recall, and F1 score
3. Fast training time
4. Grey scale data is sufficient for this dataset

# Dataset II: Surface Photos for Multiple Materials
This dataset consists of surface photos of cracks in multiple materials, specifically concrete bridge walls, pavements, and decks. The dataset is characterized by extreme class imbalance and unclear labeling of positive and negative cases.

__Dataset Details__

1. Concrete Bridge Walls:
a) 3,851 cracked images
b) 143,000 non-cracked images

2. Concrete Bridge Pavements:
a) 2,608 cracked images
b) 217,000 non-cracked images

3. Concrete Bridge Decks:
a) 2,025 cracked images
b) 116,000 non-cracked images

__Model Selection__
For Dataset II, the VGG16 (Very Deep Convolutional Networks for Large-Scale Image Recognition) architecture has been chosen as the deep learning image classification model. The decision to use VGG16 is based on its superior capabilities due to its pre-trained nature. VGG16 has been pre-trained on large-scale image classification tasks, including the ImageNet dataset. This pre-training enables the network to learn general features from a diverse set of images, making it well-suited for crack detection in the multiple materials dataset.

# Conclusion
Automated crack detection in civil structures is essential for efficient building inspections and accurate assessment of building health. This project utilizes deep learning image classification models, specifically CNN for Dataset I and VGG16 for Dataset II, to detect and classify cracks in different types of material surfaces. By leveraging these models, it is possible to significantly improve the accuracy, speed, and reliability of crack detection processes, contributing to the overall safety and integrity of civil structures.
