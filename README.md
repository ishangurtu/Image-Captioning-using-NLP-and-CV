# Image-Captioning-using-NLP-and-CV

This project performs Image Captioning using both NLP and CV techniques in Python having a fair accuracy. Flicker 8K Dataset was used and trained using Inception V3, my model and Glove vectors.

This code packet contains a python executable file and a saved model.h5 file that was trained and worked best for this dataset. This project is executed in Python Programming language.

Image captioning is converting or translating the contents of an image in a written sentence format in a specific language (English in this case).

The Flicker 8K Dataset used here consists of 8000 images of different sizes with 5 captions for each image present in text data. 6000 images are used for training, 1000 for testing, and the rest to randomly select the images to check the accuracy and practicality of our model.

Inception V3 architecture by Google is used to extract Image features and reduce training time. Glove vectors which are a set of NLP common word vectors.

 

The broad sequence of how this task was achieved using Google Colaboratory is :

Importing necessary libraries and defining basic variables.
Load and clean the data from extra white spaces and punctuations etc.
Load glove embeddings.
Reading the data and segregating it into test and train lists.
Defining start/stop sequence.
Loading Inception V3 model and defining image and output layer dimensions.
Encoding test and train images into a pickle to reduce time and create test and training data
Separate test and train captions.
Including words that occur only beyond a certain threshold value to avoid misleading by NN.
Make two tables (Dictionaries) one to convert word to index and vice versa.
We create a data generator function to create data when the Network needs rather than providing all beforehand. We are training the model on 2 captions rather than 5.
Loading glove embeddings and inserting it into the glove embedding matrix.
Creating our model and training it.
Define the caption generating function and test it on 10 random images.
 

Link for Flicker 8k image data, text data, and glove:

 

Images and Text

https://www.kaggle.com/shadabhussain/flickr8k/download (Use Only Images and Text Data, not the trained model)

Glove 200d.txt data(Glove Vectors)

https://www.kaggle.com/incorpes/glove6b200d/download
