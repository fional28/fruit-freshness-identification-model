# fruit-freshness-identification-model iDTech-final-project

## Description
Due to a lack of efficient measures for dealing with food waste at many levels in the status quo, the world’s food supply is shrinking at an alarming pace. In both homes and restaurants, food spoilage is one of the key factors leading to the majority of food waste. In agriculture, the detection of rotting fruits is equally crucial. "Finding faults in fruits is a declared objective of the agricultural business in order to save labour, waste, manufacturing costs, and time spent on the process. An infected apple may infect a healthy one if the defects are not discovered. Food waste is more likely to occur as a consequence of this, which causes several problems" (Kumar et al 22). This model identifies fresh versus rotten apples and oranges using an imagenet Resnet-18 model trained on datasets of fresh and rotten apples and oranges. The intended purposes of this AI include ensuring higher food quality and filtering rotten fruit out of production lines before it is sold in stores, or being installed in smart fridges to facilitate reduced food waste by sending alerts when food is about to spoil.


## The Algorithm
This project was developed on Nvidia's Jetson Nano, using a retrained resnet18 model whose dataset consists of images of fruit from Kaggle, labelled with the classifications fresh or rotten. I then divided the data into three categories: test, train, and val (validation). Over the course of 34 epochs, the model learns to recognize distinctive features of deteriorating fruit using the train and val datasets. The principle behind this AI image recognition system is neural networks, where the machine learns based on patterns found in a large dataset of images. My algorithm uses the imagenet.py program paired with the trained model to determine whether an inputted image is fresh or rotten. 

## Running this project
1. Connect to your Jetson Nano.
2. Ensure all necessary files are installed (resnet18.onnx, labels.txt, etc.)
3. 

[View a video explanation here](video link)

## Sources
https://www.hindawi.com/journals/jfq/2022/4661108/#conclusion 
https://www.kaggle.com/datasets/swoyam2609/fresh-and-stale-classification
