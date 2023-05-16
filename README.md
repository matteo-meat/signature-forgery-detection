# Signature Forgery Detection

The goal of this project is to build a model capable of identifying forged copies of already known signatures. The model will be built and trained using two different approaches: the Support Vector Machines (SVM) technique and a Convolutional Neural Network (CNN). 
In both cases, the dataset of choice will be the CEDAR signature dataset, a resource containing 2640 signatures from 55 people: 1320 real (24 each) and 1320 fake ones (again, 24 each).
Even when genuine and from the same person, two or more signatures will never be exactly identical: pre-processing will be necessary. Each signatures's image will need to go through steps such as noise-removal, resizing, gray-scaling to make the process easier. Then, for the SVM approach features will be "manually" extracted and used to train the model, while for the CNN this will be done "inside" the Network. Finally, the testing will be carried out and the results of the two approaches will be compared.
