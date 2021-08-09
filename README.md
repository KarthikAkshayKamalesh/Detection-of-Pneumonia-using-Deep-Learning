# Detection of Pneumonia using Deep Learning
## Description of the project
Pneumonia is an infectious and fatal respiratory infection caused by bacteria, fungus, or viruses that infect the human lung air sacs and fill them with fluid or pus. Pneumonia is one of the main reasons for death among children and the elderly in the world. Chest X-rays are the most systematic approach for diagnosing pneumonia, and the results must be evaluated by a medical professional.The inconvenient technique of detecting pneumonia resulted in the death of a person owing to incorrect diagnosis and treatment. With the advancement of computer technology, it is now feasible to build an autonomous system for detecting pneumonia and treating the disease, especially if the patient is in a remote region with limited medical resources. So, this is the primary motivation behind this project.

In this project, we are going to detect the Pneumonia using Deep Learning Algorithms. There are many ways to detect Pneumonia using Chest X-Ray images, but here we are going to compare different algorithms test accuracy and choose the best algorithm for detecting Pneumonia. After choosing the best algorithm from the pretrained ones, we will develop a Webapp to view the result of it using Flask and HTML.The Dataset that we used in this project is from the open source Kaggle.The dataset is organized into 3 folders (train, test, val) and contains subfolders for each image category (Pneumonia/Normal). There are 5,863 X-Ray images (JPEG) and 2 categories (Pneumonia/Normal). Chest X-ray images (anterior-posterior) were selected from retrospective cohorts of pediatric patients of one to five years old from Guangzhou Women and Children’s Medical Center, Guangzhou.

Download the Dataset from this link : https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia. 
### Model used :
**Here is a small comparison of all the models tested in the project:**

The Different Deep Learning Models used in comparing and detecting Pnemounia are CNN_1, CNN_2, DenseNet121, VGG16, ResNet50, InceptionV3.
```
Models         Test Accuracy
CNN1            80.77
CNN2            95.70
DenseNet        87.66
VGG16           62.50
ResNet          62.50
InceptionNet    71.47
dtype: float64

```
- ### Convolutional Neural Network

<p align="center"><img height="350" width="700" src="Assests/cnn.png"></p>

```
624/624 [==============================] - 40s 65ms/step
Test Accuracy: 80.77%
652/652 [==============================] - 365s 560ms/step
Train Accuracy: 92.87%
```

- ### Convolutional Neural Network(Different approach) :

```
Test loss is ===>  18.18680614233017 %
Test accuracy is ===>  95.70205211639404 %
```

- ### DenseNet :

<p align="center"><img height="350" width="700" src="Assests/densenet.png"></p>

```
624/624 [==============================] - 654s 1s/step
Test Accuracy: 87.66%
652/652 [==============================] - 2598s 4s/step
Train Accuracy: 93.00%
```
- ### VGG16 :

<p align="center"><img height="350" width="700" src="Assests/vgg16.png"></p>

```
624/624 [==============================] - 116s 186ms/step
Test Accuracy: 62.50%
652/652 [==============================] - 859s 1s/step
Train Accuracy: 74.31%
```


- ### ResNet :

<p align="center"><img height="350" width="700" src="Assests/resnet_arch.png"></p>

```
624/624 [==============================] - 115s 184ms/step
Test Accuracy: 62.50%
652/652 [==============================] - 827s 1s/step
Train Accuracy: 74.19%
```

- ### InceptionNet :
<p align="center"><img height="350" width="700" src="Assests/inceptionnet.png"></p>

```
624/624 [==============================] - 119s 191ms/step
Test Accuracy: 71.47%
652/652 [==============================] - 468s 719ms/step
Train Accuracy: 88.40%
```
### Front-End
Creating a Front-end using Flask and Html to display the results of the image that we can upload in the webapp.

<p align="center"><img height="350" width="700" src="Assests/webapp.png"></p>

## Installation

1. Download the Dataset from the link given below. This is a open source dataset from Kaggle.
   https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia
2. Download and Install Git on your computer. Click the link below to download the Git.  The installation process is straightforward and brings you through a lot of boilerplate    information. The one thing you want to be careful with is that you allow Git to be used from the command line.
   https://git-scm.com/download/
3. Open the Command Prompt (on Windows) or whichever terminal you happen to be using on your computer.
4. In the terminal, navigate to the location in which you would like to store the repo. You can do so by typing the following command:

   $ cd <directory>


