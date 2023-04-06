# Emotion and gender identification 
## Dataset
In this code I used a dataset which was collected from ordinary people. In collection process, subjects were asked to say 10 different sentences in persian language with 4 different emotions(Sad,Happy,Angry, and dispassionate), and then their voices were recorded.This dataset was collected in spring 2022 with the help of ECE students of university of Tehran.

## Dataset Cleaning 
Due to large number of data collector, Our original dataset was not so clean.There were some faults in csv file(which is related to information of subjects and their voices). For example, instead of having two labels('f' and 'm') for gender, our original dataset had 6 labels('f','f ', 'F', 'm', 'M', 'w'). There were some other simillar faults which all of them have been solved by *cleaning.ipynb* code. 

## Feature Extraction
After cleaning dataset, we extracted various kinds of features(Time and frequency domain features) from these audios using librosa library. We used *feat_extraction.ipynb* code for this part.    

## Emotion and gender Classification 
Using extracted features, we classify emotions and genders using 5 different classifiers(MLP, SVC('rbf'), SVC('linear'), NaiveBayes, and KNN). We used *classification.ipynb* code for this part.    

## Clustering 
Finally we used different approaches to cluster our audios based on emotion. Our approaches were Kmeans, Agglomerative, and Gaussian mixture. We used *clustering.ipynb* code for this part.      
