# ImageCaption
This is a small ImageCaption project I did when I was a undergraduate student.

# Brief Introduction of what I did.
![image](https://github.com/Demoom/ImageCaption/tree/master/Image/result.jpg)<br>
## Brief introduction of what I did
The data I use is Flickr8K, 8091 pictures and each picture has 5 manual descriptions.
I use pictures and their description to train models.<br>
Here is the whole model.<br>
![image](https://github.com/Demoom/ImageCaption/tree/master/Image/model.png)<br>
Left is CNN model, which is used to get the features of pictures. Right is LSTM model, which is used to encode the description. Then, put the features and description into another network for final words predict.<br>
The way I train models like this, use previous description to predict next word, start with "<".<br>
![image](https://github.com/Demoom/ImageCaption/tree/master/Image/train_method.PNG)<br>
After I training the whole model, here is best result of test data.<br>
![image](https://github.com/Demoom/ImageCaption/tree/master/Image/result.jpg)<br>
And here are two bad results.<br>
![image](https://github.com/Demoom/ImageCaption/tree/master/Image/result2.jpg)
![image](https://github.com/Demoom/ImageCaption/tree/master/Image/result3.jpg)<br>
This may due to model not recognize this little girl well, and model also detect this grey road as a river.<br>
The model tell so many "is" is because "is" is a high frequency word, this can improve by using Beam Search.<br>

I can't find notebook of this project, upload it latter.<br>
