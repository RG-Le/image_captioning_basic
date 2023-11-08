# image_captioning_basic

This repository contains an Image-Captioning model that uses Flicker8k dataset, to caption images. The archtitection is a Vision-Language one i.e CNN-LSTM. We have used VGG16 to extract features from the images and then mapped each images to possible captions, and then trained the Vision-Language model to predict best words that will deescribe the given images.

The current model uses VGG16, but we can use EfficientNet or anyother model. Also using Attention mechanism in language and vision tasks can improve the accuracy very efficiently.


# Basic Project Overview:
### 1. Feature Extraction
Extract Features from all the images using pretrained CNN
VGG16 in our case
Save it in a pickle file


### 2. Captions Preprocessing
Preprocess the text data for each image
i.e removal of punctuations, additional signs, numbers
Add start and end at the end of each sentence


### 3. Model Training 
Text Generation Model
This will take the captions for a single image and features
and give some text output that is similar to the captions
Briefly, from the given sequences of captions, it will try and
predict the next possible word.


### 4. Result and Analysis
Result Metric:
BLEU-Score: Metric used to check n-gram predictions for text generations
For this project:
BLEU-1 -> 0.56 and BLEU-2 -> 0.33
Favorable Range (above 30)
These are unigram and bigram scores.
Model is just decent for curr tasks.
