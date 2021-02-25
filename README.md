# OVERVIEW

Automatic music classification is an area of research that has ben receiving a great deal of attention in recent years. Nowadays, the majority of music information is stored in online services (ex. Spotify). Thus, there is an increasing need to classify music track into specific music collections.
This project classifies music tracks based on their genre, using the GTZAN dataset.

# PROJECT

The first approach uses traditional machine learning techniques, following the methodology below.
- Feature extraction
- Preprocessing
- Feature selection/Feature engineering
- Classification

Results of first approach based on accuracy, where BFE(Backward feature elimination) and FFS(Forward feature selection).

![Screenshot 2021-02-25 143841](https://user-images.githubusercontent.com/26204902/109156254-4a865d80-7779-11eb-8070-4acac9c26c27.png)

The second approach uses early feature integration and fusion of the decisions of the classifier in each window, a method we can refer as late feature integration.

Confusion matrix of the second approach.

![Capture](https://user-images.githubusercontent.com/26204902/109155804-b0261a00-7778-11eb-9a8f-e2a2238c318a.PNG)
