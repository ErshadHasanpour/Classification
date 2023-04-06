# Emotion and gender identification 
## Dataset
In this code I used a dataset which was collected from ordinary people. In collection process, subjects were asked to say 10 different sentences in persian language with 4 different emotions(Sad,Happy,Angry, and dispassionate), and then recorded their voices. this dataset was collected in spring 2022 with the help of ECE students of university of Tehran.

## Dataset Cleaning 
our original dataset was not clean due to large number of data collector. there was some faults in csv file(which is related to information of subjects and their voices). 
in file 'cleaning.ipynb' we have cleaned our dataset.

# Emotion and gender identification
first of all we extract various kinds of features(Time and frequency domain features) from these audios using librosa library. 

