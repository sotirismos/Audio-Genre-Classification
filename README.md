# Audio Genre Classification

Automatic music classification is an area of research that has ben receiving a great deal of attention in recent years. Nowadays, the majority of music information is stored in online services (ex. Spotify). Thus, there is an increasing need to classify music track into specific music collections.
The research field of automatic music genre classification has got increasing importance in the last few years. The most significant proposal to specifically deal with this task was released in 2002 by Tzanetakis et al. Several strategies dealing with related problems have been proposed in research areas such as speech/music discriminators and classification of a variety of sounds.

## Overview

**The first approach uses traditional machine learning techniques**, following the methodology below.
- Feature extraction
- Preprocessing
- Feature selection/Feature engineering
- Classification

**The second approach uses early feature integration and fusion of the decisions of the classifier in each window**, a method we can refer as late feature integration.


###### Dataset

The GTZAN dataset is the most-used public dataset for evaluation in machine listening research for music genre recognition (MGR). The files were collected in 2000-2001 from a variety of sources including personal CDs, radio, microphone recordings, in order to represent a variety of recording conditions.
A collection of 10 genres with 100 audio files each, all having a length of 30 seconds are included in this dataset.

https://www.kaggle.com/andradaolteanu/gtzan-dataset-music-genre-classification

###### Feature extraction

The features that were extracted fall into the following categories:

- Time domain features 
- Frequency domain features
- Cepstral features
- Chroma features


###### Preprocessing

The techniques that were used for preprocessing fall into the following categories:

- Basic filter methods for discarding of constant, duplicate, quasi-constant features
- Kendall's correlation coefficient computed

###### Feature selection

The techniques that were used for feature selection fall into the following categories:

- Principal Component Analysis (PCA)
- Linear discriminant analysis (LDA)
- Sparse autoencoder
- Forward (floating) feature selection
- Backward (floating) feature elimination
- Exhaustive feature selection

###### Classification

- Random forest
- Neural network
- Support vector machines (SVM)

###### Early feature integration

Temporal feature integration is another approach to combine nformation. It uses a sequence of short-time feature vectors to reate a single new feature vector at a larger time scale. It assumes a minimal loss of the important temporal information for usic genre classification in the short-time feature extraction.

![Capture](https://user-images.githubusercontent.com/26204902/132348249-cf9d4245-7006-478c-af0e-93f3d0425b44.PNG)


###### Late feature integration/Fusion of decisions

Decision fusion is one form of data fusion that combines the decisions of multiple classifiers into a common decision about the activity that occurred.

![Capture](https://user-images.githubusercontent.com/26204902/132348732-2664a361-ab81-4ba7-8cf3-b02eb3b78ee8.PNG)

**Results of first approach based on accuracy, where BFE(Backward feature elimination) and FFS(Forward feature selection)**

![Screenshot 2021-02-25 143841](https://user-images.githubusercontent.com/26204902/109156254-4a865d80-7779-11eb-8070-4acac9c26c27.png)

The second approach uses early feature integration and fusion of the decisions of the classifier in each window, a method we can refer as late feature integration.

**Confusion matrix of the second approach**.

![Capture](https://user-images.githubusercontent.com/26204902/109155804-b0261a00-7778-11eb-9a8f-e2a2238c318a.PNG)

###### Librosa, pandas, keras, numpy, scipy, scikit learn were the python libraries used for this project.

###### This repo also contains the report in Greek.





