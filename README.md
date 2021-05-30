# Deep Learning Experiments: Style Transfer, Image Captioning

## Style Transfer 
Implemented the style transfer technique from "Image Style Transfer Using Convolutional Neural Networks" (Gatys et al., CVPR 2015). The general idea is to take two images, and produce a new image that reflects the content of one but the artistic "style" of the other. 


<img width="285" height="822" alt="Screen Shot 2021-05-30 at 12 12 39 AM" src="https://user-images.githubusercontent.com/47619897/120091712-c0cd8f80-c0db-11eb-8456-1360cd5ce85b.png">   <img width="285" alt="Screen Shot 2021-05-30 at 12 13 09 AM" src="https://user-images.githubusercontent.com/47619897/120091722-d2af3280-c0db-11eb-8a3a-6fe07d9ee737.png"> <img width="285"  height="822" alt="Screen Shot 2021-05-30 at 12 14 54 AM" src="https://user-images.githubusercontent.com/47619897/120091759-1144ed00-c0dc-11eb-8eb1-1c184ab2d0b1.png">





## RNN & LSTM Captioning 
Vanilla recurrent neural networks to train a model that can generate novel captions for images. Used the 2014 release of the Microsoft COCO dataset for image captioning, which consists of 80,000 training images and 40,000 validation images, each annotated with 5 captions. 

<img width="435" alt="Screen Shot 2021-05-30 at 12 02 09 AM" src="https://user-images.githubusercontent.com/47619897/120091571-494b3080-c0da-11eb-845d-9614cb175902.png"> <img width="480" alt="Screen Shot 2021-05-30 at 12 03 06 AM" src="https://user-images.githubusercontent.com/47619897/120091583-6b44b300-c0da-11eb-9d10-a7ad868321b5.png">

Vanilla RNNs can be tough to train on long sequences due to vanishing and exploding gradiants caused by repeated matrix multiplication. LSTMs solve this problem by replacing the simple update rule of the vanilla RNN with a gating mechanism as follows.

<img width="455" alt="Screen Shot 2021-05-30 at 12 04 09 AM" src="https://user-images.githubusercontent.com/47619897/120091592-90392600-c0da-11eb-8866-459668225d44.png"> <img width="455" alt="Screen Shot 2021-05-30 at 12 04 55 AM" src="https://user-images.githubusercontent.com/47619897/120091605-ac3cc780-c0da-11eb-809e-31ac8de07ddc.png">
