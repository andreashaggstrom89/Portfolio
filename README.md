# Portfolio

257 Things

This is an image classification project using transfer learning techniques. One of the top performing models in the Imagenet competition (ILSVRC) is used to classify images on new data and classes. The model is the convolutional neural network InceptionV3 with a fully connected layer with 2048 units and 50% dropout followed by an output layer with 257 units according to the new classes. The top layer is replaced and trained while remaining all other weights that was trained on Imagenet frozen. This method preserves the original model's strong ability to detect features in images and transfer the predictive power to new tasks, commonly known as transfer learning.

The new top layer only needed to be trained for 20 epochs on a little more than 27,000 images to reach an accuracy of 84%. This is a lot less computational time needed compared to training the model from scratch. Also, the training dataset did not need to be so large compared to Imagenet with millions of images that the base model was originally trained on.


NLP Sentiment

Sentiment analysis machines are increasingly popular since companies want to be able to track how customers perceive their products and brand in comment fields, Twitter etc. In this project, over 20,000 reviews from a fashion retail company is used to find the sentiment in the comment that made the customer also give a 5-star rating. 

The model is a recurrent neural network with LSTM cells that is capable of optimizing its predictions while remembering contexts from far earlier. The words are preprocessed with an embedding technique that connects words with similar meanings and contexts. After 40 epochs, it was able to predict the correct sentiment and corresponding number of stars with an accuracy of 81%. Compared to a simpler machine learning model (Random forest with 100 units) that only slightly predicted better than chance (average f1-score: 52%).


Time-series

The time-series project is a recurrent neural network predicting the opening OMXS30 Stock Index price five days ahead in time using inputs of 180 days of opening prices and variables such as high, low and volume to describe intra-day variations. The model outperformed conventional time-series forecasting (ARIMA) with lower RMSE and faster reaction to swift price changes.

