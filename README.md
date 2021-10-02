# DeepLearning: Anime Character Detection and Facial Recognition
## Introduction
Japanese animation and manga illustrations has gained popularity in recent times around the globe. There exists many popular shows and within those shows many popular characters emerge. In this project we take a tour into a very unexplored area of face detection of japanese animated characters and classification
 
**Problem Statement:** As anime become more and more popular, the number of fans continue to grow. As a consequence more anime oriented businesses have started to pop up around the globe. With the amount of new anime shows coming out every year, it becomes increasingly difficult for business to keep track of characters in anime shows. Sometimes, customers will find an interesting anime character from an image without any identifying information and would like to see if any products in the store exists. As a business owner, it would be useful to have a detection system to get information from the image to see if they have such any such products. For this project, we train a convolutional neural network (CNN) model to identify anime characters by name. We then combine this model with a pretrained haar cascade face detection model to make a facial recognition model.

**What Data Will We Collect?:** We collect face images of various characters from the following
1. Google Image Scraper
2. DANBOORU2020
a. Over 2.9 Million Images of anime characters
b. With about n=300K labeled images
 
## Work Flow:
![](Images/workflow.png)
## Pretrained Haar Cascade Model
In order to detect faces on images, we use a pre-trained Haar Cascade Model (lbpcascade_animeface) which was obtained from https://github.com/nagadomi/lbpcascade_animeface. The model has an 82% detection rate for animated faces. The model does has some draw back by giving some false positives boundary boxes. But overall does a ok job at detecting faces.
 
## Road Map
We will present a total of four different models. We will
train on four different datasets:
1. Three characters 
2. Ten characters 
3. Twenty characters 
4. 113 characters
We try to see the performance of each model by keeping track validation metrics.
##  Three Character Model: Performance
For this first model we trained on three characters from the popular anime show Naruto:
1. Naruto Uzumaki, Sasuke Uchiha, Sakura Haruno.
2. 50-200 data samples for each character was obtained.
Below is the performance of the model
![](Images/Graph_1.png)
