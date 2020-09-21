# ImageCaption
This is a small ImageCaption project I did when I was a undergraduate student.

# Brief Introduction of what I did.
<img src="https://github.com/Demoom/ImageCaption/blob/master/Image/result.jpg" width="40%" height="40%">
## Brief introduction of what I did
The data I use is Flickr8K, 8091 pictures and each picture has 5 manual descriptions.
I use pictures and their description to train models.<br>
Here is the whole model.<br>
<img src="https://github.com/Demoom/ImageCaption/blob/master/Image/model.png" width="40%" height="40%"><br>
Left is CNN model, which is used to get the features of pictures. Right is LSTM model, which is used to encode the description. Then, put the features and description into another network for final words predict.<br>
The way I train models like this, use previous description to predict next word, start with "<".<br>
<img src="https://github.com/Demoom/ImageCaption/blob/master/Image/train_method.PNG" width="40%" height="40%"><br>
After I training the whole model, here is best result of test data.<br>
<img src="https://github.com/Demoom/ImageCaption/blob/master/Image/result.jpg" width="40%" height="40%"><br>
And here are two bad results.<br>
<img src="https://github.com/Demoom/ImageCaption/blob/master/Image/result2.jpg" width="30%" height="30%">
<img src="https://github.com/Demoom/ImageCaption/blob/master/Image/result3.jpg" width="30%" height="30%"><br>
This may due to model not recognize this little girl well, and model also detect this grey road as a river.<br>
The model tell so many "is" is because "is" is a high frequency word, this can improve by using Beam Search.<br>

I can't find notebook of this project, upload it latter.<br>
