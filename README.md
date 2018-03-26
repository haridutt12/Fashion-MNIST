Fashion

Training AI machine learning models on the Fashion MNIST dataset.

Read the full article at Image Recognition for Fashion with Machine Learning

What is Fasion-MNIST?

Fashion-MNIST is a dataset consisting of 70,000 images (60k training and 10k test) of clothing objects, such as shirts, pants, shoes, and more. Each example is a 28x28 grayscale image, associated with a label from 10 classes. The 10 classes are listed below.

The dataset was designed as a plug-and-play replacement for the traditional MNIST handwritten digit recognizing dataset. Both datasets use the same scale and type of image files, along with the same number of classification labels (10), for usage with machine learning models.
The Dataset

Download the dataset as a series of 4 zipped files:

Train Images Train Labels Test Images Test Labels

The dataset can be loaded in R by using the same script for loading the traditional MNIST dataset. Additionally, images can be displayed in the same manner, by calling the showDigit method.
Labels

Each training and test example is assigned to one of the following labels:
Label 	Description
0 	T-shirt/top
1 	Trouser
2 	Pullover
3 	Dress
4 	Coat
5 	Sandal
6 	Shirt
7 	Sneaker
8 	Bag
9 	Ankle boot
Pre-trained Models

You can find a set of pre-trained models included in this repository for immediate loading into the R environment.
Loading Your Own Images

You can load your own (color) images of shirts, pants, or shoes by reading any 28x28 image, converting to grayscale, and extracting the single channel of bytes from grayscale. Once loaded, you can classify the result using a trained machine learning model, based on the fashion-mnist dataset.
Accuracy

The trained models have achieved the following accuracies (train/test) on 30k images as shown below. A detailed list of accuracies is also available.
Baseline Algorithm (always predicts the most frequently occurring clothing item)

12%/10%
Support Vector Machine (svmRadial)

91%/87%
Gradient Boosting Machine (gbm)

90%/85%
Neural Network (multinom)

84%/78%
LogitBoost

81%/75%
