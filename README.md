# Emotion and gender identification 
## Dataset
In this code, a large dataset collected from ordinary people has been used . In collection process, subjects were asked to say 10 different sentences in persian language with 4 different emotions(Sad,Happy,Angry, and Dispassionate), and then their voices were recorded. This dataset was collected in spring 2022 with the help of ECE students in the university of Tehran.

## Dataset Cleaning and Feature Extraction
Due to large number of data collected, the original dataset was not so clean.There were some faults in csv file(which is related to information of subjects and their voices). For example,There are some duplicated rows in csv file. After cleaning dataset, various kinds of features(Time and frequency domain features) from these audios were extracted using librosa library. All extracted features were saved in *.pickl* format for next operations. After extracting features, it was seen that there was some other faults in dataset. For example, instead of having two labels('f' and 'm') for gender, the original dataset had 6 labels('f','f ', 'F', 'm', 'M', 'w'). There were some other similar faults which all of them have been solved. I used *feature_extraction.ipynb* code for all of this part.

## Emotion and gender Classification 
Using extracted features, I classified emotions(4 classes) and genders(2 classes) using 5 different classifiers(MLP, SVC('rbf'), SVC('linear'), NaiveBayes, and KNN). I used *classification.ipynb* code for these classifications.    

## Clustering 
Finally I used different approaches to cluster these audios based on emotion. These approaches were Kmeans, Agglomerative, and Gaussian mixture. I used *clustering.ipynb* code for this purpose.      
