# Genre_classification

## Introduction
The main aim of this project is to classify music according to their genres.
It contains 10 music genres. 
The genres are - blues, classical, country, disco, pop, jazz, reggae, rock, metal

## Dataset
I gathered the dataset from GTZAN genre collection, link for the same is: http://marsyas.info/downloads/datasets.html
The dataset is approximately 1.2GB, each genre has 100 audio clips in .wav format, so the total is 10 x 100 i.e. 1000 audio set.

## Required Libraries 
The libraries required for this project are: </br>
librosa==0.7.1&nbsp; </br>
sklearn==0.21.3&nbsp; </br>
matplotlib==3.1.1&nbsp; </br>
keras==2.3.1&nbsp; </br>
pandas==0.25.3&nbsp; </br>
seaborn==0.9.0&nbsp; </br>

To install all files in the requirements.txt file:</br>
cd to the directory where requirements.txt is located.</br>
activate your virtualenv.</br>
run: pip install -r requirements.txt
  in your shell.</br>
Note: Librosa is used for audio data analysis.
  


## Preprocessing the dataset
preprocess.ipynb</br>
First the audio data is converted into spectrogram. Then the features of music is extracted such as MFCCs, Spectral centroid, spectral rolloff, chroma features, zero coefficient and rmse. </br>
This features are then appended into csv file with the labels/ genres list and the file name.

This csv file is analyzed using pandas, then we split the train and test data into 80% and 20% respectively.

## Creating the CNN model
model.ipynb </br>
At last, the CNN model is created. The batch size is 64 and number of epoch are 100.</br>
I have used adam optimizer for optimizing the model.

