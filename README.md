# Signature Forgery Detection

## Abstract

The goal of this project is to build a model capable of identifying forged copies of already known signatures. The model will be built and trained using two different approaches: the Support Vector Machines (SVM) technique and a Convolutional Neural Network (CNN). 
In both cases, the dataset of choice will be the CEDAR signature dataset, a resource containing 2640 signatures from 55 people: 1320 real (24 each) and 1320 fake ones (again, 24 each).
Even when genuine and from the same person, two or more signatures will never be exactly identical: pre-processing will be necessary. Each signatures's image will need to go through steps such as noise-removal, resizing, gray-scaling to make the process easier. Then, for the SVM approach features will be "manually" extracted and used to train the model, while for the CNN this will be done "inside" the Network. Finally, the testing will be carried out and the results of the two approaches will be compared.

## Data

The data used can be downloaded from the following links:  
[CEDAR dataset](https://drive.google.com/file/d/1RY0nkJ7GV_B7Tm_8UxtNdeeDo3T3Y4My/view?usp=sharing): the original image dataset, used to generate image pairs;  
[Image pairs](https://drive.google.com/file/d/16eozvfDptosXc4CxUXoX2QXe2GwXzbj8/view?usp=sharing): image pairs and labels, divided into X(pairs) and y(labels). Stored as .npy files;  
[HOG Distances](https://drive.google.com/file/d/1-DnM0OEKO7OxW3sTMwWeAHgJM0jlY1dM/view?usp=sharing): HOG distances and labels, computed from the image pairs sets and divided into train and test sets. Stored as .npy files. To be used to run the SVM locally on machines with low resources, since loading the pairs and computing the distances from scratch can take lots of RAM and time.
